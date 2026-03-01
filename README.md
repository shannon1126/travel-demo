<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ココロココ - Hero Section</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@400;500;700&family=Noto+Serif+JP:wght@500;700&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'brand-green': '#2fa84b',
                        'bg-gray': '#fafafa',
                        'text-main': '#333333',
                    },
                    fontFamily: {
                        sans: ['"Noto Sans JP"', 'sans-serif'],
                        serif: ['"Noto Serif JP"', 'serif'],
                    }
                }
            }
        }
    </script>
    <style>
        body { background-color: #fafafa; color: #333333; }
        /* 左側垂直文字特效 */
        .vertical-text { writing-mode: vertical-rl; text-orientation: mixed; }
    </style>
</head>
<body class="font-sans antialiased pb-20">

    <header class="max-w-[1400px] mx-auto px-6 py-6 flex justify-between items-center">
        <div class="text-3xl font-bold tracking-widest flex items-center gap-1">
            ココ<span class="w-6 h-6 border-4 border-brand-green rounded-sm block inline-block"></span>ココ
        </div>
        
        <div class="hidden lg:flex items-center bg-white rounded-full shadow-sm pr-6 border border-gray-100">
            <button class="bg-brand-green text-white px-6 py-3 rounded-full font-bold text-sm mr-4 hover:bg-green-700 transition">
                記事検索
            </button>
            <div class="flex gap-4 text-sm font-medium text-gray-700">
                <a href="#" class="hover:text-brand-green">▤ 都道府県</a> <span class="text-gray-300">|</span>
                <a href="#" class="hover:text-brand-green">▤ テーマ</a> <span class="text-gray-300">|</span>
                <a href="#" class="hover:text-brand-green">▤ 地図</a> <span class="text-gray-300">|</span>
                <a href="#" class="hover:text-brand-green">▤ キーワード</a>
            </div>
        </div>

        <button class="bg-brand-green text-white w-16 h-16 rounded-full flex flex-col items-center justify-center shadow-md hover:scale-105 transition">
            <span class="block w-6 h-[2px] bg-white mb-1"></span>
            <span class="block w-6 h-[2px] bg-white mb-1"></span>
            <span class="text-[10px] font-bold mt-1">MENU</span>
        </button>
    </header>

    <main class="max-w-[1400px] mx-auto px-6 mt-8 flex flex-col lg:flex-row gap-12 relative">
        
        <div class="hidden xl:block absolute left-0 top-20">
            <div class="bg-gray-100 text-brand-green py-8 px-2 rounded-full vertical-text text-sm font-bold tracking-widest">
                人と風土の物語を編む
            </div>
        </div>

        <section class="lg:w-3/5 xl:ml-16">
            <div class="relative group cursor-pointer">
                <div class="overflow-hidden rounded-[2.5rem] shadow-sm">
                    <img src="https://images.unsplash.com/photo-1542640244-7e672d6cb466?auto=format&fit=crop&q=80&w=1200" alt="五ヶ瀬町" class="w-full h-[400px] object-cover transition duration-500 group-hover:scale-105">
                </div>
                
                <div class="absolute -top-4 right-8 bg-white text-gray-800 font-bold px-6 py-3 rounded-2xl shadow-md text-lg">
                    宮崎
                </div>
                
                <div class="absolute bottom-10 left-10 text-white drop-shadow-lg">
                    <h2 class="text-4xl font-bold leading-snug">小さく始めて、<br>大きく咲かせる<br>五ヶ瀬町</h2>
                </div>
            </div>

            <div class="mt-6 px-2">
                <div class="text-sm text-brand-green font-medium mb-3">
                    2024年9月17日 <span class="text-gray-300 mx-2">|</span> <span class="text-gray-600">甲斐かおり</span>
                </div>
                <h3 class="text-2xl font-serif font-bold text-gray-800 mb-6 hover:text-brand-green transition cursor-pointer">
                    【風土をめぐる旅】小さく始めて、大きく咲かせる　五ヶ瀬町
                </h3>
                
                <div class="flex justify-between items-center border-t border-gray-200 pt-4">
                    <div class="flex gap-2">
                        <span class="bg-green-100 text-brand-green text-xs px-3 py-1.5 rounded text-sm font-medium">伝統をつなぐ</span>
                        <span class="bg-green-100 text-brand-green text-xs px-3 py-1.5 rounded text-sm font-medium">農林漁業</span>
                        <span class="bg-green-100 text-brand-green text-xs px-3 py-1.5 rounded text-sm font-medium">里山暮らし</span>
                    </div>
                    <div class="text-sm font-bold text-gray-800">
                        連載: 風土をめぐる旅
                    </div>
                </div>
            </div>
        </section>

        <section class="lg:w-2/5 flex flex-col pt-4">
            <div class="text-center mb-10">
                <h1 class="text-4xl font-serif font-bold leading-loose text-gray-800">
                    人と風土の<br>
                    <span class="border-b-4 border-brand-green pb-2">物語を編む</span>
                </h1>
            </div>

            <div class="flex justify-center mb-8">
                <svg width="200" height="100" viewBox="0 0 200 100" fill="none" stroke="#333" stroke-width="2">
                    <path d="M20,80 L80,30 L140,80 M60,50 L100,20 L180,80" stroke-linecap="round" stroke-linejoin="round"/>
                    <rect x="65" y="45" width="30" height="35" fill="white"/>
                    <rect x="120" y="50" width="40" height="30" fill="white"/>
                </svg>
            </div>

            <div class="relative mt-auto px-4">
                <button class="absolute left-0 top-1/2 -translate-y-1/2 -ml-4 w-10 h-10 bg-white border-2 border-brand-green text-brand-green rounded-full flex items-center justify-center z-10 hover:bg-brand-green hover:text-white transition">
                    ❮
                </button>
                
                <div class="overflow-hidden rounded-3xl shadow-sm cursor-pointer">
                    <img src="https://images.unsplash.com/photo-1500382017468-9049fed747ef?auto=format&fit=crop&q=80&w=800" alt="田園風景" class="w-full h-[220px] object-cover hover:scale-105 transition duration-500">
                </div>

                <button class="absolute right-0 top-1/2 -translate-y-1/2 -mr-4 w-10 h-10 bg-white border-2 border-brand-green text-brand-green rounded-full flex items-center justify-center z-10 hover:bg-brand-green hover:text-white transition">
                    ❯
                </button>
            </div>
        </section>

    </main>

</body>
</html>
