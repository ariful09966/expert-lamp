<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AniStream - Preview</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        background: '#0a0a0f',
                        surface: '#14141e',
                        primary: '#8b5cf6', // Purple
                    }
                }
            }
        }
    </script>
    <style>
        body { background-color: #0a0a0f; color: white; font-family: sans-serif; }
        .glass { background: rgba(20, 20, 30, 0.8); backdrop-filter: blur(10px); border-bottom: 1px solid rgba(255, 255, 255, 0.05); }
    </style>
</head>
<body>
    <div id="root"></div>

    <!-- React & Babel -->
    <script src="https://unpkg.com/react@18/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>

    <script type="text/babel">
        const animes = [
            { id: 1, title: "Solo Leveling", img: "https://s4.anilist.co/file/anilistcdn/media/anime/cover/large/bx162235-ZIt2Hq22nO2r.jpg", tag: "Action" },
            { id: 2, title: "Jujutsu Kaisen", img: "https://s4.anilist.co/file/anilistcdn/media/anime/cover/large/bx113415-bbBWj4pEFseh.jpg", tag: "Supernatural" },
            { id: 3, title: "Demon Slayer", img: "https://s4.anilist.co/file/anilistcdn/media/anime/cover/large/bx101922-PEn1CTc93DQl.jpg", tag: "Action" },
            { id: 4, title: "Attack on Titan", img: "https://s4.anilist.co/file/anilistcdn/media/anime/cover/large/bx104578-laZZlCbQDOvY.jpg", tag: "Dark Fantasy" },
            { id: 5, title: "One Piece", img: "https://s4.anilist.co/file/anilistcdn/media/anime/cover/large/bx21-YCDignzx8rL3.jpg", tag: "Adventure" }
        ];

        function App() {
            return (
                <div>
                    {/* Navbar */}
                    <nav className="fixed w-full top-0 z-50 glass h-16 flex items-center px-8 justify-between">
                        <div className="flex items-center gap-2 text-primary font-bold text-2xl">
                            ▶ AniStream
                        </div>
                        <div className="flex gap-6 text-sm font-medium text-gray-300">
                            <span className="hover:text-primary cursor-pointer">Home</span>
                            <span className="hover:text-primary cursor-pointer">Popular</span>
                            <span className="bg-primary text-white px-4 py-2 rounded-full cursor-pointer hover:bg-purple-400">Login</span>
                        </div>
                    </nav>

                    {/* Hero Banner */}
                    <div className="relative w-full h-[60vh] mt-16">
                        <img src="https://s4.anilist.co/file/anilistcdn/media/anime/banner/162235-1BfCIfiY3p9m.jpg" className="w-full h-full object-cover opacity-50" />
                        <div className="absolute inset-0 bg-gradient-to-t from-background to-transparent" />
                        <div className="absolute bottom-0 left-0 p-16 max-w-2xl">
                            <h1 className="text-6xl font-bold text-white mb-4">Solo Leveling</h1>
                            <p className="text-gray-300 mb-6">They say whatever doesn't kill you makes you stronger, but that's not the case for the world's weakest hunter Sung Jinwoo...</p>
                            <button className="bg-primary text-white px-8 py-3 rounded-full font-bold shadow-lg hover:scale-105 transition-transform">
                                Watch Episode 1
                            </button>
                        </div>
                    </div>

                    {/* Grid Section */}
                    <div className="max-w-7xl mx-auto px-8 py-8">
                        <h2 className="text-2xl font-bold text-white mb-6 border-l-4 border-primary pl-3">Recently Updated</h2>
                        <div className="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-5 gap-6">
                            {animes.map(anime => (
                                <div key={anime.id} className="group cursor-pointer bg-surface rounded-xl overflow-hidden shadow-lg hover:ring-2 hover:ring-primary transition-all">
                                    <div className="aspect-[3/4] overflow-hidden relative">
                                        <img src={anime.img} className="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500" />
                                        <div className="absolute top-2 left-2 bg-primary text-xs font-bold px-2 py-1 rounded shadow">HD</div>
                                    </div>
                                    <div className="p-4">
                                        <h3 className="font-semibold truncate">{anime.title}</h3>
                                        <p className="text-xs text-gray-400 mt-1">{anime.tag}</p>
                                    </div>
                                </div>
                            ))}
                        </div>
                    </div>
                </div>
            );
        }

        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(<App />);
    </script>
</body>
</html>
