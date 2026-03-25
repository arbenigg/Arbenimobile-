#   
<!DOCTYPE html>  
<html lang="sq">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>ArbeniMobile - Sistemi i Riparimeve</title>  
    <script src="https://cdn.tailwindcss.com"></script>  
    <script src="https://unpkg.com/lucide@latest"></script>  
    <style>  
        @import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;600;800&display=swap');  
          
        :root {  
            --primary: #3b82f6;  
            --bg: #050505;  
        }  
  
        body {  
            font-family: 'Plus Jakarta Sans', sans-serif;  
            background-color: var(--bg);  
            color: white;  
            margin: 0;  
            -webkit-tap-highlight-color: transparent;  
        }  
  
        .glass {  
            background: rgba(255, 255, 255, 0.03);  
            backdrop-filter: blur(20px);  
            border: 1px solid rgba(255, 255, 255, 0.08);  
        }  
  
        .input-field {  
            background: rgba(255, 255, 255, 0.05);  
            border: 1px solid rgba(255, 255, 255, 0.1);  
            border-radius: 1rem;  
            padding: 1rem 1.5rem;  
            width: 100%;  
            outline: none;  
            transition: all 0.3s;  
        }  
  
        .input-field:focus {  
            border-color: var(--primary);  
            box-shadow: 0 0 0 4px rgba(59, 130, 246, 0.1);  
        }  
  
        .btn-primary {  
            background: var(--primary);  
            color: white;  
            font-weight: 700;  
            padding: 1rem;  
            border-radius: 1rem;  
            width: 100%;  
            transition: all 0.2s;  
            box-shadow: 0 10px 20px rgba(59, 130, 246, 0.2);  
        }  
  
        .btn-primary:active {  
            transform: scale(0.98);  
        }  
  
        .step-dot {  
            width: 10px;  
            height: 10px;  
            border-radius: 50%;  
            background: rgba(255,255,255,0.1);  
        }  
  
        .step-dot.active {  
            background: var(--primary);  
            box-shadow: 0 0 10px var(--primary);  
        }  
    </style>  
</head>  
<body>  
  
    <div id="app" class="min-h-screen max-w-md mx-auto p-6 flex flex-col">  
          
        <!-- Header -->  
        <header class="flex justify-between items-center py-6 mb-8">  
            <div>  
                <h1 class="text-2xl font-black tracking-tighter text-blue-500">ArbeniMobile</h1>  
                <p class="text-[10px] uppercase tracking-[0.3em] text-gray-500 font-bold">Teknologji & Servis</p>  
            </div>  
            <button id="navToggle" class="p-3 glass rounded-2xl">  
                <i data-lucide="settings" id="navIcon" class="w-5 h-5 text-gray-400"></i>  
            </button>  
        </header>  
  
        <!-- Main Content Area -->  
        <main class="flex-grow">  
              
            <!-- PAMJA E KLIENTIT -->  
            <section id="clientSection" class="space-y-8 animate-in fade-in duration-500">  
                <div class="text-center">  
                    <h2 class="text-xl font-bold mb-2">Gjeni statusin e telefonit</h2>  
                    <p class="text-gray-500 text-sm">Shkruani kodin e servisit për të parë progresin</p>  
                </div>  
  
                <div class="relative">  
                    <input type="text" id="trackInput" placeholder="Psh: AM-102" class="input-field text-lg font-bold uppercase">  
                    <button id="trackBtn" class="absolute right-2 top-2 bg-blue-600 p-3 rounded-xl">  
                        <i data-lucide="search" class="w-5 h-5"></i>  
                    </button>  
                </div>  
  
                <div id="statusResult" class="hidden glass rounded-[2rem] p-8 space-y-6">  
                    <!-- Dinamike -->  
                </div>  
            </section>  
  
            <!-- PAMJA E ADMINIT -->  
            <section id="adminSection" class="hidden space-y-6 animate-in fade-in duration-500">  
                <div class="flex items-center gap-3 mb-4">  
                    <div class="p-3 bg-blue-600/10 rounded-xl">  
                        <i data-lucide="plus" class="text-blue-500"></i>  
                    </div>  
                    <h2 class="text-xl font-bold">Menaxho Riparimet</h2>  
                </div>  
  
                <div class="glass rounded-2xl p-6 space-y-4">  
                    <input type="text" id="adminId" placeholder="ID (Kodi)" class="input-field">  
                    <input type="text" id="adminDevice" placeholder="Modeli (p.sh iPhone 14)" class="input-field">  
                    <select id="adminStatus" class="input-field appearance-none">  
                        <option value="Në Pritje">Në Pritje</option>  
                        <option value="Duke u Punuar">Duke u Punuar</option>  
                        <option value="Gati">Gati për Dorëzim</option>  
                        <option value="U Dorëzua">U Dorëzua</option>  
                    </select>  
                    <div class="flex items-center justify-between px-2">  
                        <span class="text-xs font-bold text-gray-400">Progresi (%)</span>  
                        <span id="progVal" class="text-blue-500 font-bold">50%</span>  
                    </div>  
                    <input type="range" id="adminProgress" class="w-full h-2 bg-gray-800 rounded-lg appearance-none cursor-pointer accent-blue-500">  
                      
                    <button id="saveOrderBtn" class="btn-primary mt-4">Ruaj të Dhënat</button>  
                </div>  
            </section>  
  
        </main>  
  
        <!-- Footer -->  
        <footer class="py-10 text-center">  
            <div class="flex justify-center gap-6 mb-4 opacity-20">  
                <i data-lucide="shield-check"></i>  
                <i data-lucide="cpu"></i>  
                <i data-lucide="smartphone"></i>  
            </div>  
            <p class="text-[9px] uppercase tracking-[0.4em] text-gray-600">ArbeniMobile Precision Quality</p>  
        </footer>  
  
    </div>  
  
    <!-- Firebase Integrated Logic -->  
    <script type="module">  
        import { initializeApp } from "https://www.gstatic.com/firebasejs/11.4.0/firebase-app.js";  
        import { getFirestore, doc, setDoc, getDoc, serverTimestamp } from "https://www.gstatic.com/firebasejs/11.4.0/firebase-firestore.js";  
        import { getAuth, signInAnonymously } from "https://www.gstatic.com/firebasejs/11.4.0/firebase-auth.js";  
  
        // Konfigurimi i sistemit  
        const firebaseConfig = JSON.parse(__firebase_config);  
        const app = initializeApp(firebaseConfig);  
        const db = getFirestore(app);  
        const auth = getAuth(app);  
        const appId = typeof __app_id !== 'undefined' ? __app_id : 'arbenimobile-official';  
  
        // Autentikimi i heshtur  
        signInAnonymously(auth).catch(err => console.error("Auth Error", err));  
  
        // Icons  
        lucide.createIcons();  
  
        // Navigimi  
        const navToggle = document.getElementById('navToggle');  
        const clientSection = document.getElementById('clientSection');  
        const adminSection = document.getElementById('adminSection');  
        const navIcon = document.getElementById('navIcon');  
  
        navToggle.onclick = () => {  
            const isAdmin = adminSection.classList.contains('hidden');  
            adminSection.classList.toggle('hidden', !isAdmin);  
            clientSection.classList.toggle('hidden', isAdmin);  
            navIcon.setAttribute('data-lucide', isAdmin ? 'chevron-left' : 'settings');  
            lucide.createIcons();  
        };  
  
        // Admin Slider Progress  
        const progSlider = document.getElementById('adminProgress');  
        const progVal = document.getElementById('progVal');  
        progSlider.oninput = () => progVal.innerText = `${progSlider.value}%`;  
  
        // SAVE DATA (Për Arbenin)  
        document.getElementById('saveOrderBtn').onclick = async () => {  
            const id = document.getElementById('adminId').value.trim().toUpperCase();  
            const device = document.getElementById('adminDevice').value.trim();  
            const status = document.getElementById('adminStatus').value;  
            const progress = progSlider.value;  
  
            if (!id || !device) return alert("Ju lutem mbushni ID dhe Modelin!");  
  
            const btn = document.getElementById('saveOrderBtn');  
            btn.innerText = "Duke ruajtur...";  
            btn.disabled = true;  
  
            try {  
                const docRef = doc(db, 'artifacts', appId, 'public', 'data', 'repairs', id);  
                await setDoc(docRef, {  
                    id, device, status, progress,   
                    lastUpdate: serverTimestamp()  
                });  
                alert(`Riparimi ${id} u ruajt me sukses!`);  
                document.getElementById('adminId').value = "";  
                document.getElementById('adminDevice').value = "";  
            } catch (e) {  
                alert("Gabim gjatë ruajtjes. Provoni përsëri.");  
                console.error(e);  
            } finally {  
                btn.innerText = "Ruaj të Dhënat";  
                btn.disabled = false;  
            }  
        };  
  
        // TRACK DATA (Për Klientin)  
        document.getElementById('trackBtn').onclick = async () => {  
            const id = document.getElementById('trackInput').value.trim().toUpperCase();  
            const resultBox = document.getElementById('statusResult');  
  
            if (!id) return;  
  
            resultBox.innerHTML = `<div class="flex justify-center p-4"><div class="animate-spin h-6 w-6 border-2 border-blue-500 border-t-transparent rounded-full"></div></div>`;  
            resultBox.classList.remove('hidden');  
  
            try {  
                const docRef = doc(db, 'artifacts', appId, 'public', 'data', 'repairs', id);  
                const snap = await getDoc(docRef);  
  
                if (snap.exists()) {  
                    const data = snap.data();  
                    resultBox.innerHTML = `  
                        <div class="flex justify-between items-start">  
                            <div>  
                                <h3 class="text-2xl font-black">${data.device}</h3>  
                                <p class="text-blue-500 text-[10px] font-bold uppercase tracking-widest mt-1">Statusi Aktual</p>  
                            </div>  
                            <span class="bg-blue-500/10 text-blue-400 px-3 py-1 rounded-lg text-[10px] font-bold uppercase tracking-tighter">  
                                ${data.status}  
                            </span>  
                        </div>  
                          
                        <div class="space-y-3">  
                            <div class="flex justify-between text-[10px] font-bold text-gray-500 uppercase">  
                                <span>Progresi i punës</span>  
                                <span>${data.progress}%</span>  
                            </div>  
                            <div class="h-3 bg-white/5 rounded-full overflow-hidden border border-white/5">  
                                <div class="h-full bg-blue-500 rounded-full" style="width: ${data.progress}%"></div>  
                            </div>  
                        </div>  
  
                        <div class="pt-6 border-t border-white/5 flex items-center justify-between opacity-30">  
                            <div class="flex items-center gap-2">  
                                <i data-lucide="clock" class="w-3 h-3"></i>  
                                <span class="text-[9px] font-bold uppercase">Kodi: ${data.id}</span>  
                            </div>  
                            <div class="flex items-center gap-2 text-green-500">  
                                <i data-lucide="check-circle" class="w-3 h-3"></i>  
                                <span class="text-[9px] font-bold uppercase">I Konfirmuar</span>  
                            </div>  
                        </div>  
                    `;  
                    lucide.createIcons();  
                } else {  
                    resultBox.innerHTML = `<p class="text-center text-red-400 text-sm font-bold">Kodi nuk u gjet! Kontrolloni saktësinë.</p>`;  
                }  
            } catch (e) {  
                resultBox.innerHTML = `<p class="text-center text-red-400 text-sm">Ndodhi një gabim gjatë kërkimit.</p>`;  
            }  
        };  
    </script>  
</body>  
</html>  
  
