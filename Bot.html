# Yatchomrong-
www.yatchomrong.com
<!DOCTYPE html>
<html lang="km">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>ChomrongOS v4.0 - Desktop Edition</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <style>
        /*
         * ChomrongOS v4.0 Stylesheet - Desktop Edition
         * Architecture: Window-based Desktop Environment
         * Author: Yorth Chomrong (Re-architected by Gemini)
         * Date: 2025-08-08
         */

        /* --- CSS Variables & Themes --- */
        :root {
            --primary-color: #00ff41;
            --secondary-color: #00ffae;
            --accent-color: #ff00ff;
            --dark-bg: #0a0a0a;
            --bg-transparent: rgba(20, 20, 30, 0.75);
            --border-color: rgba(0, 255, 65, 0.3);
            --text-color: #e0e0e0;
            --window-bg: rgba(15, 15, 25, 0.85);
            --title-bar-bg: linear-gradient(90deg, var(--primary-color), var(--secondary-color));
        }

        /* --- Base & Desktop --- */
        * { box-sizing: border-box; margin: 0; padding: 0; }
        html, body { height: 100%; width: 100%; overflow: hidden; }
        body {
            font-family: 'Courier New', Courier, monospace;
            background-color: var(--dark-bg);
            color: var(--text-color);
            background-image:
                linear-gradient(var(--border-color) 1px, transparent 1px),
                linear-gradient(to right, var(--border-color) 1px, var(--dark-bg) 1px);
            background-size: 40px 40px;
            position: relative;
        }
        #desktop {
            width: 100%;
            height: calc(100% - 40px); /* Full height minus taskbar */
            position: relative;
            overflow: hidden;
        }
        .desktop-icon {
            color: white;
            text-align: center;
            width: 80px;
            padding: 10px 5px;
            cursor: pointer;
            border-radius: 5px;
        }
        .desktop-icon:hover {
            background: rgba(255, 255, 255, 0.1);
        }
        .desktop-icon i {
            font-size: 32px;
            margin-bottom: 5px;
        }
        .desktop-icon span {
            display: block;
            font-size: 12px;
            text-shadow: 1px 1px 2px black;
        }

        /* --- Taskbar --- */
        #taskbar {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 40px;
            background: var(--bg-transparent);
            backdrop-filter: blur(10px);
            border-top: 1px solid var(--border-color);
            display: flex;
            align-items: center;
            z-index: 10000;
        }
        #start-button {
            width: 40px;
            height: 40px;
            background: var(--primary-color);
            color: var(--dark-bg);
            border: none;
            font-size: 20px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        #start-button:hover { background: var(--secondary-color); }
        #taskbar-apps {
            flex-grow: 1;
            display: flex;
            height: 100%;
        }
        .taskbar-item {
            padding: 0 15px;
            height: 100%;
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 14px;
            cursor: pointer;
            border-right: 1px solid var(--border-color);
            transition: background-color 0.2s;
        }
        .taskbar-item:hover { background: rgba(255, 255, 255, 0.1); }
        .taskbar-item.active { background: var(--primary-color); color: var(--dark-bg); }
        .taskbar-item.minimized { background: rgba(255, 255, 255, 0.2); }
        #system-tray {
            padding: 0 15px;
            height: 100%;
            display: flex;
            align-items: center;
        }
        #clock { font-size: 14px; }

        /* --- Start Menu --- */
        #start-menu {
            position: absolute;
            bottom: 40px;
            left: 0;
            width: 250px;
            height: 300px;
            background: var(--bg-transparent);
            backdrop-filter: blur(15px);
            border: 1px solid var(--border-color);
            border-bottom: none;
            border-radius: 5px 5px 0 0;
            z-index: 9999;
            display: none;
            flex-direction: column;
            padding: 10px;
            animation: slideUp 0.3s ease-out;
        }
        @keyframes slideUp { from { transform: translateY(50px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
        .start-menu-item {
            padding: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
            cursor: pointer;
            border-radius: 3px;
            transition: background-color 0.2s;
        }
        .start-menu-item:hover { background: var(--primary-color); color: var(--dark-bg); }

        /* --- Windowing System --- */
        .window {
            position: absolute;
            border: 1px solid var(--border-color);
            border-radius: 8px;
            background: var(--window-bg);
            backdrop-filter: blur(10px);
            box-shadow: 0 0 20px rgba(0,0,0,0.5);
            min-width: 300px;
            min-height: 200px;
            display: flex;
            flex-direction: column;
            transition: opacity 0.2s, transform 0.2s;
        }
        .window.minimized-state {
            opacity: 0;
            transform: scale(0.8);
            pointer-events: none;
        }
        .title-bar {
            height: 30px;
            background: var(--title-bar-bg);
            color: var(--dark-bg);
            display: flex;
            align-items: center;
            padding: 0 10px;
            cursor: move;
            border-radius: 7px 7px 0 0;
            flex-shrink: 0;
        }
        .title-bar-text { flex-grow: 1; font-weight: bold; }
        .title-bar-controls { display: flex; gap: 5px; }
        .title-bar-btn {
            width: 20px; height: 20px; border: none; border-radius: 50%;
            background: rgba(0,0,0,0.2); color: var(--dark-bg);
            cursor: pointer; display: flex; justify-content: center; align-items: center;
            font-size: 12px;
        }
        .title-bar-btn.minimize-btn:hover { background: #ffc107; }
        .title-bar-btn.close-btn:hover { background: #dc3545; }
        .window-body {
            flex-grow: 1;
            padding: 10px;
            overflow: auto;
        }
        .window-resize-handle {
            position: absolute;
            width: 10px;
            height: 10px;
            right: 0;
            bottom: 0;
            cursor: se-resize;
        }

        /* --- App Specific Styles --- */
        /* File Explorer */
        .file-explorer-body { display: flex; height: 100%; }
        .fe-sidebar { width: 150px; border-right: 1px solid var(--border-color); padding: 5px; flex-shrink: 0; }
        .fe-main { flex-grow: 1; padding: 10px; display: flex; flex-wrap: wrap; align-content: flex-start; gap: 15px; }
        .fe-item { width: 80px; text-align: center; cursor: pointer; padding: 5px; border-radius: 3px; }
        .fe-item:hover { background: rgba(0, 255, 65, 0.2); }
        .fe-item i { font-size: 32px; color: var(--secondary-color); margin-bottom: 5px; }
        .fe-item span { font-size: 12px; word-wrap: break-word; }
        
        /* Code Editor */
        .code-editor-textarea {
            width: 100%; height: 100%; background: #050505; border: none;
            color: #f0f0f0; font-family: 'Courier New', monospace; font-size: 14px;
            line-height: 1.5; resize: none; outline: none; padding: 10px;
        }
        
        /* Terminal */
        .terminal-body { padding: 0 !important; background: rgba(0,0,0,0.8); }
        .terminal-output { padding: 10px; white-space: pre-wrap; height: calc(100% - 30px); overflow-y: auto; }
        .terminal-input-line { display: flex; height: 30px; padding: 0 10px; align-items: center; border-top: 1px solid var(--border-color); }
        .terminal-prompt { color: var(--primary-color); }
        .terminal-input { background: transparent; border: none; color: var(--primary-color); flex-grow: 1; outline: none; font-family: inherit; }
        .ai-response { border-left: 3px solid var(--primary-color); padding-left: 10px; margin-top: 5px; display: block; }
        
        /* Music Player */
        .music-player-body { text-align: center; }
        #track-info { margin-bottom: 20px; }
        #track-title { font-size: 1.5em; color: var(--primary-color); }
        #music-controls button { background: none; border: 1px solid var(--border-color); color: var(--text-color); font-size: 20px; width: 50px; height: 50px; border-radius: 50%; margin: 0 10px; cursor: pointer; }
        #music-controls button:hover { background: var(--primary-color); color: var(--dark-bg); }
        #playlist { list-style: none; text-align: left; margin-top: 20px; height: 150px; overflow-y: auto; border: 1px solid var(--border-color); padding: 5px;}
        #playlist li { padding: 8px; cursor: pointer; }
        #playlist li:hover { background: rgba(0, 255, 65, 0.2); }
        #playlist li.playing { color: var(--primary-color); }

        /* AI Assistant */
        .ai-assistant-body { display: flex; flex-direction: column; height: 100%; }
        .chat-window { flex-grow: 1; overflow-y: auto; padding: 10px; }
        .chat-message { max-width: 85%; margin-bottom: 10px; display: flex; align-items: flex-start; gap: 10px; }
        .chat-message.user { margin-left: auto; flex-direction: row-reverse; }
        .chat-avatar { font-size: 1.2rem; color: var(--primary-color); border: 1px solid var(--border-color); border-radius: 50%; width: 35px; height: 35px; display: flex; justify-content: center; align-items: center; flex-shrink: 0; }
        .chat-bubble { background: rgba(0,0,0,0.4); padding: 10px; border-radius: 10px; }
        .chat-message.user .chat-bubble { background: rgba(0, 255, 65, 0.1); }
        .chat-form { display: flex; gap: 5px; border-top: 1px solid var(--border-color); padding-top: 10px; }
        .chat-input { flex-grow: 1; background: transparent; border: 1px solid var(--border-color); border-radius: 5px; padding: 8px; color: var(--text-color); }
        .chat-submit-btn { background: var(--primary-color); border: none; color: var(--dark-bg); padding: 0 15px; border-radius: 5px; cursor: pointer; }
        .loading-dots span { display: inline-block; width: 8px; height: 8px; border-radius: 50%; background-color: var(--primary-color); margin: 0 2px; animation: bounce 1.4s infinite ease-in-out both; }
        .loading-dots span:nth-child(1) { animation-delay: -0.32s; }
        .loading-dots span:nth-child(2) { animation-delay: -0.16s; }
        @keyframes bounce { 0%, 80%, 100% { transform: scale(0); } 40% { transform: scale(1.0); } }
        .generated-image { max-width: 100%; border-radius: 5px; margin-top: 10px; border: 1px solid var(--border-color); }

    </style>
</head>
<body>
    <div id="desktop">
        <!-- Desktop icons will be rendered here -->
    </div>
    <div id="taskbar">
        <button id="start-button"><i class="fa-solid fa-bars"></i></button>
        <div id="taskbar-apps"></div>
        <div id="system-tray">
            <div id="clock"></div>
        </div>
    </div>
    <div id="start-menu">
        <!-- Start menu items will be rendered here -->
    </div>
    
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/tone/14.7.77/Tone.js"></script>

    <script>
    document.addEventListener('DOMContentLoaded', () => {
        console.log("Booting ChomrongOS v4.0...");

        // =================================================================================
        // --- VIRTUAL FILE SYSTEM (VFS) ---
        // =================================================================================
        const VFS = {
            _data: {
                'home': {
                    type: 'dir',
                    children: {
                        'user': {
                            type: 'dir',
                            children: {
                                'Desktop': { type: 'dir', children: {} },
                                'Documents': {
                                    type: 'dir',
                                    children: {
                                        'readme.txt': { type: 'file', content: 'សូមស្វាគមន៍មកកាន់ ChomrongOS v4.0!' },
                                        'projects.txt': { type: 'file', content: '1. Portfolio OS\n2. E-commerce Site\n3. Telegram Bot' }
                                    }
                                },
                                'Music': {
                                    type: 'dir',
                                    children: {
                                        'track1.mp3': { type: 'file', content: 'C4' },
                                        'track2.mp3': { type: 'file', content: 'E4' },
                                        'track3.mp3': { type: 'file', content: 'G4' }
                                    }
                                },
                                'code.js': { type: 'file', content: 'console.log("Hello, ChomrongOS!");' }
                            }
                        }
                    }
                },
                'bin': {
                    type: 'dir',
                    children: {
                        'terminal': { type: 'file', content: 'executable' },
                        'explorer': { type: 'file', content: 'executable' },
                        'sysmon': { type: 'file', content: 'executable' }
                    }
                },
                'etc': {
                    type: 'dir',
                    children: {
                        'os.conf': { type: 'file', content: 'OS_VERSION=4.0\nAI_CORE=gemini-2.5-flash' }
                    }
                }
            },

            resolvePath(path) {
                const parts = path.split('/').filter(p => p);
                let current = this._data;
                for (const part of parts) {
                    if (current[part] && current[part].type === 'dir') {
                        current = current[part].children;
                    } else if (current[part] && current[part].type === 'file') {
                        return current[part];
                    } else {
                        return null; // Path not found or not a directory
                    }
                }
                return current;
            },

            list(path) {
                const node = this.resolvePath(path);
                return node ? Object.keys(node).map(key => ({ name: key, type: node[key].type })) : null;
            },

            read(path) {
                const node = this.resolvePath(path);
                return (node && node.type === 'file') ? node.content : null;
            },

            write(path, content) {
                const parts = path.split('/').filter(p => p);
                const filename = parts.pop();
                const dirPath = parts.join('/');
                const dir = this.resolvePath(dirPath);
                if (dir && dir[filename] && dir[filename].type === 'file') {
                    dir[filename].content = content;
                    return true;
                }
                return false;
            },

            create(path, type = 'file') {
                const parts = path.split('/').filter(p => p);
                const name = parts.pop();
                const dirPath = parts.join('/');
                const dir = this.resolvePath(dirPath);
                if (dir && !dir[name]) {
                    dir[name] = { type, content: type === 'file' ? '' : undefined };
                    if (type === 'dir') dir[name].children = {};
                    return true;
                }
                return false;
            }
        };


        // =================================================================================
        // --- API SERVICE ---
        // =================================================================================
        const ApiService = {
            async callGemini(prompt) {
                const apiKey = ""; // Canvas provides this
                const url = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-05-20:generateContent?key=${apiKey}`;
                const payload = { contents: [{ role: "user", parts: [{ text: prompt }] }] };

                try {
                    const response = await fetch(url, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });
                    if (!response.ok) throw new Error(`HTTP error! status: ${response.status}`);
                    const result = await response.json();
                    return result?.candidates?.[0]?.content?.parts?.[0]?.text || "មិនអាចទទួលបានចម្លើយទេ។";
                } catch (error) {
                    console.error("Gemini API Error:", error);
                    return "មានបញ្ហាក្នុងការភ្ជាប់ទៅកាន់ AI Core។";
                }
            },
            async generateImage(prompt) {
                const apiKey = ""; // Canvas provides this
                const url = `https://generativelanguage.googleapis.com/v1beta/models/imagen-3.0-generate-002:predict?key=${apiKey}`;
                const payload = { instances: [{ prompt }], parameters: { "sampleCount": 1 } };

                try {
                    const response = await fetch(url, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });
                    if (!response.ok) throw new Error(`HTTP error! status: ${response.status}`);
                    const result = await response.json();
                    if (result.predictions && result.predictions[0]?.bytesBase64Encoded) {
                        return `data:image/png;base64,${result.predictions[0].bytesBase64Encoded}`;
                    }
                    return null;
                } catch (error) {
                    console.error("Imagen API Error:", error);
                    return null;
                }
            }
        };

        // =================================================================================
        // --- WINDOW MANAGER ---
        // =================================================================================
        const WindowManager = {
            windows: new Map(),
            activeWindow: null,
            zIndexCounter: 100,
            taskbarEl: document.getElementById('taskbar-apps'),

            create(app) {
                if (this.windows.has(app.id)) {
                    this.focus(app.id);
                    return;
                }

                const winEl = document.createElement('div');
                winEl.className = 'window';
                winEl.id = `win-${app.id}`;
                winEl.style.width = app.width || '500px';
                winEl.style.height = app.height || '400px';
                winEl.style.left = `${Math.random() * (window.innerWidth - 500)}px`;
                winEl.style.top = `${Math.random() * (window.innerHeight - 400 - 40)}px`;

                winEl.innerHTML = `
                    <div class="title-bar">
                        <span class="title-bar-text"><i class="${app.icon} fa-fw"></i> ${app.title}</span>
                        <div class="title-bar-controls">
                            <button class="title-bar-btn minimize-btn" data-id="${app.id}"><i class="fa-solid fa-window-minimize"></i></button>
                            <button class="title-bar-btn close-btn" data-id="${app.id}"><i class="fa-solid fa-xmark"></i></button>
                        </div>
                    </div>
                    <div class="window-body" id="body-${app.id}"></div>
                    <div class="window-resize-handle"></div>
                `;

                document.getElementById('desktop').appendChild(winEl);
                app.render(document.getElementById(`body-${app.id}`));

                const taskbarItem = document.createElement('div');
                taskbarItem.className = 'taskbar-item';
                taskbarItem.id = `task-${app.id}`;
                taskbarItem.innerHTML = `<i class="${app.icon} fa-fw"></i> ${app.title}`;
                this.taskbarEl.appendChild(taskbarItem);

                const windowState = { el: winEl, taskbarEl: taskbarItem, app: app, minimized: false };
                this.windows.set(app.id, windowState);

                this.setupEvents(windowState);
                this.focus(app.id);
            },

            setupEvents(winState) {
                const { el, app } = winState;
                const titleBar = el.querySelector('.title-bar');
                const closeBtn = el.querySelector('.close-btn');
                const minimizeBtn = el.querySelector('.minimize-btn');
                const resizeHandle = el.querySelector('.window-resize-handle');

                // Focus
                el.addEventListener('mousedown', () => this.focus(app.id));
                winState.taskbarEl.addEventListener('click', () => this.toggleMinimize(app.id));

                // Close
                closeBtn.addEventListener('click', (e) => {
                    e.stopPropagation();
                    this.close(app.id);
                });

                // Minimize
                minimizeBtn.addEventListener('click', (e) => {
                    e.stopPropagation();
                    this.minimize(app.id);
                });

                // Dragging
                let isDragging = false, dragOffsetX, dragOffsetY;
                titleBar.addEventListener('mousedown', (e) => {
                    isDragging = true;
                    dragOffsetX = e.clientX - el.offsetLeft;
                    dragOffsetY = e.clientY - el.offsetTop;
                });
                document.addEventListener('mousemove', (e) => {
                    if (isDragging) {
                        el.style.left = `${e.clientX - dragOffsetX}px`;
                        el.style.top = `${e.clientY - dragOffsetY}px`;
                    }
                });
                document.addEventListener('mouseup', () => { isDragging = false; });

                // Resizing
                let isResizing = false, resizeStartX, resizeStartY, startWidth, startHeight;
                resizeHandle.addEventListener('mousedown', (e) => {
                    isResizing = true;
                    resizeStartX = e.clientX;
                    resizeStartY = e.clientY;
                    startWidth = parseInt(document.defaultView.getComputedStyle(el).width, 10);
                    startHeight = parseInt(document.defaultView.getComputedStyle(el).height, 10);
                    e.preventDefault();
                });
                document.addEventListener('mousemove', (e) => {
                    if (isResizing) {
                        const newWidth = startWidth + e.clientX - resizeStartX;
                        const newHeight = startHeight + e.clientY - resizeStartY;
                        el.style.width = `${newWidth}px`;
                        el.style.height = `${newHeight}px`;
                    }
                });
                document.addEventListener('mouseup', () => { isResizing = false; });
            },

            focus(id) {
                if (this.activeWindow) {
                    this.windows.get(this.activeWindow)?.taskbarEl.classList.remove('active');
                }
                const winState = this.windows.get(id);
                if (winState) {
                    winState.el.style.zIndex = ++this.zIndexCounter;
                    winState.taskbarEl.classList.add('active');
                    this.activeWindow = id;
                    if (winState.minimized) {
                        this.restore(id);
                    }
                }
            },
            
            toggleMinimize(id) {
                const winState = this.windows.get(id);
                if (!winState) return;

                if (winState.minimized) {
                    this.focus(id); // focus will restore it
                } else {
                    if (this.activeWindow === id) {
                        this.minimize(id);
                    } else {
                        this.focus(id);
                    }
                }
            },

            minimize(id) {
                const winState = this.windows.get(id);
                if (winState && !winState.minimized) {
                    winState.el.classList.add('minimized-state');
                    winState.taskbarEl.classList.add('minimized');
                    winState.taskbarEl.classList.remove('active');
                    winState.minimized = true;
                    this.activeWindow = null;
                }
            },

            restore(id) {
                const winState = this.windows.get(id);
                if (winState && winState.minimized) {
                    winState.el.classList.remove('minimized-state');
                    winState.taskbarEl.classList.remove('minimized');
                    winState.minimized = false;
                    this.focus(id);
                }
            },

            close(id) {
                const winState = this.windows.get(id);
                if (winState) {
                    winState.el.remove();
                    winState.taskbarEl.remove();
                    this.windows.delete(id);
                    if (this.activeWindow === id) {
                        this.activeWindow = null;
                    }
                }
            }
        };

        // =================================================================================
        // --- APPLICATIONS ---
        // =================================================================================
        const Apps = {
            'terminal': {
                id: 'terminal', title: 'ស្ថានីយ', icon: 'fa-solid fa-terminal', width: '600px', height: '400px',
                render(container) {
                    container.classList.add('terminal-body');
                    container.innerHTML = `
                        <div class="terminal-output">ChomrongOS Terminal v4.0 - Type 'help' for commands.</div>
                        <div class="terminal-input-line">
                            <span class="terminal-prompt">user@chomrongos:~$</span>
                            <input type="text" class="terminal-input" autofocus>
                        </div>`;
                    
                    const outputEl = container.querySelector('.terminal-output');
                    const inputEl = container.querySelector('.terminal-input');
                    const commandHistory = [];
                    let historyIndex = 0;

                    inputEl.addEventListener('keydown', e => {
                        if (e.key === 'Enter' && inputEl.value) {
                            const command = inputEl.value;
                            outputEl.innerHTML += `\n<span class="terminal-prompt">user@chomrongos:~$</span> ${command}`;
                            commandHistory.push(command);
                            historyIndex = commandHistory.length;
                            this.execute(command, outputEl);
                            inputEl.value = '';
                            outputEl.scrollTop = outputEl.scrollHeight;
                        } else if (e.key === 'ArrowUp') {
                            if (historyIndex > 0) {
                                historyIndex--;
                                inputEl.value = commandHistory[historyIndex];
                            }
                        } else if (e.key === 'ArrowDown') {
                            if (historyIndex < commandHistory.length - 1) {
                                historyIndex++;
                                inputEl.value = commandHistory[historyIndex];
                            } else {
                                inputEl.value = '';
                            }
                        }
                    });
                },
                async execute(command, outputEl) {
                    const [cmd, ...args] = command.split(' ');
                    const scroll = () => outputEl.scrollTop = outputEl.scrollHeight;
                    switch(cmd.toLowerCase()) {
                        case 'help': outputEl.innerHTML += '\nAvailable: help, ls, cat, clear, whoami, ps, kill, ask, neofetch'; break;
                        case 'ls': outputEl.innerHTML += '\n' + (VFS.list(args[0] || 'home/user').map(f => f.name).join('  ')); break;
                        case 'cat': outputEl.innerHTML += '\n' + (VFS.read(`home/user/${args[0]}`) || 'File not found.'); break;
                        case 'clear': outputEl.innerHTML = ''; break;
                        case 'whoami': outputEl.innerHTML += '\nuser: chomrong'; break;
                        case 'ps': 
                            let processes = 'PID\tAPP\n---\t---\n';
                            WindowManager.windows.forEach((win, id) => {
                                processes += `${id.substring(0,4)}\t${win.app.title}\n`;
                            });
                            outputEl.innerHTML += `\n<pre>${processes}</pre>`;
                            break;
                        case 'kill':
                            const winToKill = Array.from(WindowManager.windows.keys()).find(k => k.startsWith(args[0]));
                            if (winToKill) {
                                WindowManager.close(winToKill);
                                outputEl.innerHTML += `\nProcess ${args[0]} terminated.`;
                            } else {
                                outputEl.innerHTML += `\nProcess not found.`;
                            }
                            break;
                        case 'ask':
                            const question = args.join(' ');
                            if (!question) { outputEl.innerHTML += '\nUsage: ask <your question>'; break; }
                            outputEl.innerHTML += '\n<span class="ai-response">AI is thinking...</span>';
                            scroll();
                            const response = await ApiService.callGemini(question);
                            outputEl.querySelector('.ai-response').innerHTML = response;
                            break;
                        case 'neofetch':
                            outputEl.innerHTML += `\n<pre>
    .--.      user: chomrong
   |o_o |     os: ChomrongOS v4.0
   |:_/ |     kernel: 8.0-gemini
  //   \\ \\    shell: ysh
 (|     | )   theme: matrix
/'_   _'\`/    ai_core: gemini-2.5-flash
\\___)=(___/
</pre>`;
                            break;
                        default: outputEl.innerHTML += `\nCommand not found: ${cmd}`;
                    }
                    scroll();
                }
            },
            'explorer': {
                id: 'explorer', title: 'File Explorer', icon: 'fa-solid fa-folder-open', width: '600px', height: '450px',
                currentPath: 'home/user/Desktop',
                render(container) {
                    container.classList.add('file-explorer-body');
                    container.innerHTML = `<div class="fe-sidebar"></div><div class="fe-main"></div>`;
                    this.renderContent(container);
                },
                renderContent(container) {
                    const mainEl = container.querySelector('.fe-main');
                    mainEl.innerHTML = '';
                    const items = VFS.list(this.currentPath);
                    if (items) {
                        items.forEach(item => {
                            const itemEl = document.createElement('div');
                            itemEl.className = 'fe-item';
                            const icon = item.type === 'dir' ? 'fa-folder' : 'fa-file';
                            itemEl.innerHTML = `<i class="fa-solid ${icon}"></i><span>${item.name}</span>`;
                            if (item.type === 'dir') {
                                itemEl.addEventListener('dblclick', () => {
                                    this.currentPath += `/${item.name}`;
                                    this.renderContent(container);
                                });
                            } else {
                                itemEl.addEventListener('dblclick', () => {
                                    AppLauncher.launch('editor', { filePath: `${this.currentPath}/${item.name}` });
                                });
                            }
                            mainEl.appendChild(itemEl);
                        });
                    }
                }
            },
            'editor': {
                id: 'editor', title: 'Code Editor', icon: 'fa-solid fa-file-code', width: '700px', height: '500px',
                render(container, options) {
                    const filePath = options?.filePath || 'home/user/code.js';
                    const fileContent = VFS.read(filePath);
                    container.innerHTML = `<textarea class="code-editor-textarea"></textarea>`;
                    const textarea = container.querySelector('textarea');
                    textarea.value = fileContent;
                    // In a real scenario, a library like CodeMirror or Monaco would be used here.
                    // This is a simple simulation.
                }
            },
            'music': {
                id: 'music', title: 'Music Player', icon: 'fa-solid fa-music', width: '350px', height: '400px',
                synth: null,
                playlist: VFS.list('home/user/Music'),
                currentTrack: 0,
                render(container) {
                    container.classList.add('music-player-body');
                    container.innerHTML = `
                        <div id="track-info">
                            <h3 id="track-title">Select a Track</h3>
                            <p id="track-artist">ChomrongOS Synth</p>
                        </div>
                        <div id="music-controls">
                            <button id="prev-btn"><i class="fa-solid fa-backward-step"></i></button>
                            <button id="play-btn"><i class="fa-solid fa-play"></i></button>
                            <button id="next-btn"><i class="fa-solid fa-forward-step"></i></button>
                        </div>
                        <ul id="playlist"></ul>
                    `;
                    this.synth = new Tone.Synth().toDestination();
                    const playlistEl = container.querySelector('#playlist');
                    this.playlist.forEach((track, index) => {
                        const li = document.createElement('li');
                        li.textContent = track.name;
                        li.dataset.index = index;
                        playlistEl.appendChild(li);
                    });
                    
                    container.querySelector('#play-btn').addEventListener('click', () => this.play(container));
                    container.querySelector('#prev-btn').addEventListener('click', () => this.prev(container));
                    container.querySelector('#next-btn').addEventListener('click', () => this.next(container));
                    playlistEl.addEventListener('click', (e) => {
                        if(e.target.tagName === 'LI') {
                            this.currentTrack = parseInt(e.target.dataset.index);
                            this.play(container);
                        }
                    });
                },
                play(container) {
                    const track = this.playlist[this.currentTrack];
                    const note = VFS.read(`home/user/Music/${track.name}`);
                    this.synth.triggerAttackRelease(note, "8n");
                    container.querySelector('#track-title').textContent = track.name;
                    const playlistItems = container.querySelectorAll('#playlist li');
                    playlistItems.forEach(li => li.classList.remove('playing'));
                    playlistItems[this.currentTrack].classList.add('playing');
                },
                next(container) {
                    this.currentTrack = (this.currentTrack + 1) % this.playlist.length;
                    this.play(container);
                },
                prev(container) {
                    this.currentTrack = (this.currentTrack - 1 + this.playlist.length) % this.playlist.length;
                    this.play(container);
                }
            },
            'ai_assistant': {
                id: 'ai_assistant', title: 'AI Assistant', icon: 'fa-solid fa-brain', width: '550px', height: '600px',
                render(container) {
                    container.classList.add('ai-assistant-body');
                    container.innerHTML = `
                        <div class="chat-window">
                            <div class="chat-message ai">
                                <div class="chat-avatar"><i class="fas fa-brain"></i></div>
                                <div class="chat-bubble">សួស្តី! ខ្ញុំជាជំនួយការ AI។ តើខ្ញុំអាចជួយអ្វីបាន? សាកល្បងសួរអ្វីមួយ ឬវាយ 'image: a cat in space' ដើម្បីបង្កើតរូបភាព។</div>
                            </div>
                        </div>
                        <form class="chat-form">
                            <input type="text" class="chat-input" placeholder="សួរសំណួរ ឬស្នើសុំរូបភាព...">
                            <button type="submit" class="chat-submit-btn"><i class="fa-solid fa-paper-plane"></i></button>
                        </form>
                    `;
                    const form = container.querySelector('form');
                    const input = container.querySelector('input');
                    const chatWindow = container.querySelector('.chat-window');

                    form.addEventListener('submit', async (e) => {
                        e.preventDefault();
                        const prompt = input.value.trim();
                        if (!prompt) return;
                        
                        this.addMessage(chatWindow, 'user', prompt);
                        input.value = '';
                        this.addMessage(chatWindow, 'ai', '<div class="loading-dots"><span></span><span></span><span></span></div>');

                        let responseContent;
                        if (prompt.toLowerCase().startsWith('image:')) {
                            const imagePrompt = prompt.substring(6).trim();
                            const imageUrl = await ApiService.generateImage(imagePrompt);
                            responseContent = imageUrl 
                                ? `<img src="${imageUrl}" alt="Generated Image" class="generated-image">`
                                : 'ขออภัย ไม่สามารถสร้างรูปภาพได้ในขณะนี้';
                        } else {
                            responseContent = await ApiService.callGemini(prompt);
                        }
                        
                        chatWindow.querySelector('.loading-dots').parentElement.parentElement.remove();
                        this.addMessage(chatWindow, 'ai', responseContent);
                    });
                },
                addMessage(chatWindow, sender, content) {
                    const msgEl = document.createElement('div');
                    msgEl.className = `chat-message ${sender}`;
                    const icon = sender === 'user' ? 'fa-user' : 'fa-brain';
                    msgEl.innerHTML = `<div class="chat-avatar"><i class="fas ${icon}"></i></div><div class="chat-bubble">${content}</div>`;
                    chatWindow.appendChild(msgEl);
                    chatWindow.scrollTop = chatWindow.scrollHeight;
                }
            }
        };

        // =================================================================================
        // --- OS CORE & INITIALIZATION ---
        // =================================================================================
        const AppLauncher = {
            launch(appId, options = {}) {
                if (Apps[appId]) {
                    WindowManager.create(Apps[appId], options);
                } else {
                    console.error(`App not found: ${appId}`);
                }
            }
        };

        const ChomrongOS = {
            init() {
                this.setupClock();
                this.setupStartMenu();
                this.setupDesktopIcons();
            },
            setupClock() {
                const clockEl = document.getElementById('clock');
                const updateClock = () => {
                    clockEl.textContent = new Date().toLocaleTimeString('km-KH', { hour: '2-digit', minute: '2-digit' });
                };
                updateClock();
                setInterval(updateClock, 1000);
            },
            setupStartMenu() {
                const startBtn = document.getElementById('start-button');
                const startMenu = document.getElementById('start-menu');
                Object.values(Apps).forEach(app => {
                    const itemEl = document.createElement('div');
                    itemEl.className = 'start-menu-item';
                    itemEl.innerHTML = `<i class="${app.icon} fa-fw"></i> ${app.title}`;
                    itemEl.addEventListener('click', () => {
                        AppLauncher.launch(app.id);
                        startMenu.style.display = 'none';
                    });
                    startMenu.appendChild(itemEl);
                });

                startBtn.addEventListener('click', (e) => {
                    e.stopPropagation();
                    startMenu.style.display = startMenu.style.display === 'flex' ? 'none' : 'flex';
                });
                document.addEventListener('click', () => {
                    startMenu.style.display = 'none';
                });
            },
            setupDesktopIcons() {
                const desktop = document.getElementById('desktop');
                const desktopApps = ['terminal', 'explorer', 'ai_assistant'];
                desktopApps.forEach(appId => {
                    const app = Apps[appId];
                    const iconEl = document.createElement('div');
                    iconEl.className = 'desktop-icon';
                    iconEl.innerHTML = `<i class="${app.icon}"></i><span>${app.title}</span>`;
                    iconEl.addEventListener('dblclick', () => AppLauncher.launch(app.id));
                    desktop.appendChild(iconEl);
                });
            }
        };

        ChomrongOS.init();
        AppLauncher.launch('ai_assistant'); // Launch AI on startup
    });
    </script>
</body>
</html>
