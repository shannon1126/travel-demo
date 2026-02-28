<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TravelLink AI - PDF 轉網頁 Demo</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@400;500;700&display=swap');
        body { font-family: 'Noto Sans TC', sans-serif; }
        .scrollbar-hide::-webkit-scrollbar { display: none; }
        .iphone-x {
            width: 375px;
            height: 812px;
            border: 8px solid #1a1a1a;
            border-radius: 40px;
            position: relative;
            background: white;
            overflow: hidden;
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.5);
        }
    </style>
</head>
<body class="bg-slate-100 min-h-screen">

    <header class="bg-white border-b p-4 sticky top-0 z-50">
        <div class="max-w-7xl mx-auto flex justify-between items-center">
            <div class="flex items-center gap-2">
                <div class="bg-blue-600 p-2 rounded-lg text-white">
                    <i class="fas fa-magic"></i>
                </div>
                <h1 class="text-xl font-bold text-slate-800">TravelLink AI <span class="text-sm font-normal text-slate-400">v1.0 Demo</span></h1>
            </div>
            <div class="flex gap-3">
                <button class="text-slate-500 hover:text-slate-800 px-3">保存草稿</button>
                <button class="bg-blue-600 text-white px-5 py-2 rounded-full font-medium hover:bg-blue-700 transition">發佈網頁</button>
            </div>
        </div>
    </header>

    <main class="max-w-7xl mx-auto p-6 grid grid-cols-1 lg:grid-cols-12 gap-8">
        
        <div class="lg:col-span-7 space-y-6">
            <div class="bg-white p-8 rounded-2xl shadow-sm">
                <h2 class="text-lg font-bold mb-6 text-slate-800 border-l-4 border-blue-600 pl-3">第一區塊：行程基礎資訊</h2>
                
                <div class="mb-8 border-2 border-dashed border-blue-200 bg-blue-50/50 rounded-xl p-10 text-center">
                    <i class="fas fa-file-pdf text-4xl text-blue-400 mb-4"></i>
                    <p class="text-blue-700 font-medium">已成功解析 PDF：<span class="underline">日本長野冬季行程.pdf</span></p>
                    <p class="text-xs text-slate-400 mt-2">AI 已自動完成 85% 的資料填寫</p>
                </div>

                <div class="grid gap-4">
                    <div>
                        <label class="text-sm text-slate-500 mb-1 block">行程標題</label>
                        <input type="text" class="w-full border-slate-200 border p-3 rounded-lg" value="日本長野親子客製化冬日夢幻之旅｜和紙、料理、滑雪全體驗">
                    </div>
                    <div class="grid grid-cols-2 gap-4">
                        <div>
                            <label class="text-sm text-slate-500 mb-1 block">出團日期</label>
                            <input type="text" class="w-full border-slate-200 border p-3 rounded-lg" value="2026/02/03">
                        </div>
                        <div>
                            <label class="text-sm text-slate-500 mb-1 block">行程天數</label>
                            <input type="text" class="w-full border-slate-200 border p-3 rounded-lg" value="7天">
                        </div>
                    </div>
                </div>
            </div>

            <div class="bg-white p-8 rounded-2xl shadow-sm">
                <h2 class="text-lg font-bold mb-6 text-slate-800 border-l-4 border-orange-500 pl-3">第二區塊：費用與促銷</h2>
                <div class="space-y-4">
                    <div class="bg-orange-50 p-4 rounded-xl border border-orange-100">
                        <label class="text-sm text-orange-700 font-bold mb-1 block">業務推薦：限時優惠價</label>
                        <input type="text" class="w-full border-orange-200 border p-3 rounded-lg text-lg font-bold text-orange-600" value="NT$ 88,000 起">
                    </div>
                    <div class="grid grid-cols-2 gap-4">
                        <div>
                            <label class="text-sm text-slate-500 mb-1 block">費用包含 (AI 自動辨識)</label>
                            <textarea class="w-full border-slate-200 border p-3 rounded-lg text-xs" rows="3">全程舒適專車、和紙手作體驗、北山料理教室、三晚星野飯店</textarea>
                        </div>
                        <div>
                            <label class="text-sm text-slate-500 mb-1 block">費用不含</label>
                            <textarea class="w-full border-slate-200 border p-3 rounded-lg text-xs" rows="3">個人消費、部分午餐、滑雪裝備租借</textarea>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="lg:col-span-5 flex justify-center items-start pt-4">
            <div class="sticky top-24">
                <p class="text-center text-sm text-slate-400 mb-4 italic"><i class="fas fa-mobile-alt mr-2"></i> 客人看到的樣子 (手機版預覽)</p>
                <div class="iphone-x">
                    <div class="h-full overflow-y-auto scrollbar-hide">
                        <div class="h-56 bg-cover bg-center" style="background-image: url('https://images.unsplash.com/photo-1483110322179-de6801981282?q=80&w=800&auto=format&fit=crop');">
                            <div class="h-full w-full bg-gradient-to-t from-black/80 to-transparent flex items-end p-5">
                                <div>
                                    <span class="bg-orange-500 text-white text-[10px] px-2 py-0.5 rounded-full font-bold">精選推薦</span>
                                    <h3 class="text-white font-bold text-lg mt-1 leading-tight">日本長野親子客製化冬日夢幻之旅</h3>
                                </div>
                            </div>
                        </div>

                        <div class="p-5 border-b">
                            <div class="flex gap-4 overflow-x-auto pb-2 scrollbar-hide">
                                <div class="flex-shrink-0 text-center">
                                    <div class="w-10 h-10 bg-blue-50 rounded-full flex items-center justify-center mb-1">
                                        <i class="fas fa-car text-blue-500 text-xs"></i>
                                    </div>
                                    <span class="text-[10px] text-slate-500">專車接送</span>
                                </div>
                                <div class="flex-shrink-0 text-center">
                                    <div class="w-10 h-10 bg-green-50 rounded-full flex items-center justify-center mb-1">
                                        <i class="fas fa-utensils text-green-500 text-xs"></i>
                                    </div>
                                    <span class="text-[10px] text-slate-500">道地料理</span>
                                </div>
                                <div class="flex-shrink-0 text-center">
                                    <div class="w-10 h-10 bg-purple-50 rounded-full flex items-center justify-center mb-1">
                                        <i class="fas fa-home text-purple-500 text-xs"></i>
                                    </div>
                                    <span class="text-[10px] text-slate-500">星野飯店</span>
                                </div>
                            </div>
                        </div>

                        <div class="p-5">
                            <h4 class="font-bold text-slate-800 text-sm mb-4">行程內容</h4>
                            <div class="space-y-6 border-l-2 border-slate-100 ml-2 pl-4">
                                <div class="relative">
                                    <div class="absolute -left-[25px] top-0 w-4 h-4 rounded-full bg-blue-500 border-4 border-white"></div>
                                    <p class="text-blue-600 font-bold text-[10px]">DAY 01</p>
                                    <p class="font-bold text-xs text-slate-700">抵達成田機場 - 專車前往長野</p>
                                </div>
                                <div class="relative">
                                    <div class="absolute -left-[25px] top-0 w-4 h-4 rounded-full bg-slate-300 border-4 border-white"></div>
                                    <p class="text-slate-400 font-bold text-[10px]">DAY 02</p>
                                    <p class="font-bold text-xs text-slate-700">松本城巡禮 - 蕎麥麵手作</p>
                                </div>
                            </div>
                        </div>

                        <div class="p-5 bg-slate-50">
                            <div class="bg-white p-4 rounded-xl shadow-sm border border-orange-100">
                                <p class="text-[10px] text-slate-400">專屬優惠價</p>
                                <p class="text-xl font-bold text-orange-600">NT$ 88,000 <span class="text-xs text-slate-400 font-normal">/人</span></p>
                                <button class="w-full bg-blue-600 text-white font-bold py-3 rounded-lg mt-3 text-sm shadow-lg shadow-blue-200">
                                    立即詢問早鳥優惠
                                </button>
                                <p class="text-center text-[10px] text-slate-400 mt-3 italic text-xs">已有 12 人諮詢此行程</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>
</body>
</html>
