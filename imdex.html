<!DOCTYPE html>
<html lang="sq">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Sniper Pro - Bitget & MEXC</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { 
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            background: #0a0e17; 
            color: #e6edf3; 
            padding: 15px;
            min-height: 100vh;
        }
        .header { 
            background: linear-gradient(135deg, #1a1f2e 0%, #0d1117 100%);
            padding: 20px; 
            border-radius: 15px; 
            margin-bottom: 20px;
            border: 2px solid #f0b90b;
            text-align: center;
        }
        .header h1 { color: #f0b90b; font-size: 26px; margin-bottom: 5px; }
        .status { 
            display: inline-block; 
            padding: 5px 15px; 
            border-radius: 20px; 
            font-size: 14px; 
            font-weight: bold;
            margin-top: 10px;
        }
        .active { background: #238636; color: white; }
        .inactive { background: #da3633; color: white; }
        .waiting { background: #f0b90b; color: black; }
        
        .card { 
            background: #161b22; 
            border: 1px solid #30363d; 
            border-radius: 12px; 
            padding: 20px; 
            margin-bottom: 15px;
        }
        .card-title { 
            color: #f0b90b; 
            font-size: 16px; 
            margin-bottom: 15px; 
            font-weight: bold;
            border-bottom: 1px solid #30363d;
            padding-bottom: 10px;
        }
        
        label { 
            display: block; 
            font-size: 12px; 
            color: #8b949e; 
            margin-bottom: 5px;
            margin-top: 12px;
            text-transform: uppercase;
        }
        input, select { 
            width: 100%; 
            padding: 15px; 
            background: #0d1117; 
            border: 1px solid #30363d; 
            border-radius: 8px; 
            color: #e6edf3; 
            font-size: 16px;
        }
        input:focus, select:focus { border-color: #f0b90b; outline: none; }
        
        .grid-2 { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; }
        
        .exchange-tabs {
            display: flex;
            gap: 10px;
            margin-bottom: 15px;
        }
        .tab-btn {
            flex: 1;
            padding: 12px;
            border: 2px solid #30363d;
            background: #0d1117;
            color: #8b949e;
            border-radius: 8px;
            font-weight: bold;
            cursor: pointer;
            text-align: center;
        }
        .tab-btn.active-tab {
            background: #f0b90b;
            color: black;
            border-color: #f0b90b;
        }
        
        .btn { 
            width: 100%; 
            padding: 20px; 
            border: none; 
            border-radius: 12px; 
            font-size: 20px; 
            font-weight: bold; 
            margin: 10px 0;
            cursor: pointer;
        }
        .btn-arm { background: linear-gradient(135deg, #f0b90b 0%, #d4a009 100%); color: #000; }
        .btn-disarm { background: #da3633; color: white; }
        .btn-test { background: #1f6feb; color: white; font-size: 14px; padding: 12px; }
        
        .countdown { 
            font-size: 42px; 
            font-weight: bold; 
            color: #00ff00; 
            text-align: center; 
            font-family: monospace;
            margin: 20px 0;
            text-shadow: 0 0 20px #00ff0055;
        }
        
        .position-info {
            background: #0d1117;
            border: 1px solid #30363d;
            border-radius: 8px;
            padding: 15px;
            margin: 10px 0;
            font-family: monospace;
            font-size: 14px;
        }
        .profit-positive { color: #3fb950; }
        .profit-negative { color: #f85149; }
        
        .log { 
            max-height: 250px; 
            overflow-y: auto; 
            font-family: monospace; 
            font-size: 12px; 
            background: #0a0e17; 
            padding: 10px; 
            border-radius: 8px;
            line-height: 1.6;
        }
        .log-entry { 
            margin-bottom: 5px; 
            padding: 8px; 
            border-left: 3px solid #30363d;
            background: rgba(255,255,255,0.02);
        }
        .success { border-left-color: #3fb950; color: #3fb950; }
        .error { border-left-color: #f85149; color: #f85149; }
        .info { border-left-color: #58a6ff; color: #58a6ff; }
        .warning { border-left-color: #f0b90b; color: #f0b90b; }
        
        .hidden { display: none; }
    </style>
</head>
<body>
    <div class="header">
        <h1>🎯 SNIPER PRO</h1>
        <div>Bitget + MEXC | Auto TP/SL</div>
        <span id="statusBadge" class="status inactive">● Ndalur</span>
    </div>

    <!-- Zgjedh Exchange -->
    <div class="card">
        <div class="card-title">🏦 Zgjedh Exchange</div>
        <div class="exchange-tabs">
            <div class="tab-btn active-tab" id="tabBitget" onclick="switchExchange('bitget')">🟡 Bitget</div>
            <div class="tab-btn" id="tabMexc" onclick="switchExchange('mexc')">🟢 MEXC</div>
        </div>
    </div>

    <!-- API Configuration -->
    <div class="card" id="bitgetConfig">
        <div class="card-title">🔑 Bitget API</div>
        <label>API Key</label>
        <input type="password" id="bitgetKey" placeholder="bg_..." autocomplete="off">
        <label>Secret Key</label>
        <input type="password" id="bitgetSecret" placeholder="..." autocomplete="off">
        <label>Passphrase</label>
        <input type="password" id="bitgetPass" placeholder="..." autocomplete="off">
    </div>

    <div class="card hidden" id="mexcConfig">
        <div class="card-title">🔑 MEXC API</div>
        <label>API Key</label>
        <input type="password" id="mexcKey" placeholder="mx0..." autocomplete="off">
        <label>Secret Key</label>
        <input type="password" id="mexcSecret" placeholder="..." autocomplete="off">
        <div style="background: #1f6feb22; padding: 10px; border-radius: 6px; margin-top: 10px; font-size: 12px; color: #58a6ff;">
            ℹ️ MEXC nuk ka Passphrase - vetëm Key dhe Secret
        </div>
    </div>

    <!-- Telegram -->
    <div class="card">
        <div class="card-title">💬 Telegram (Opsionale)</div>
        <div class="grid-2">
            <div>
                <label>Bot Token</label>
                <input type="text" id="tgToken" placeholder="123456:ABC...">
            </div>
            <div>
                <label>Chat ID</label>
                <input type="text" id="tgChat" placeholder="123456789">
            </div>
        </div>
        <button class="btn btn-test" onclick="testTelegram()">🧪 Testo Telegram</button>
    </div>

    <!-- Sniper Settings -->
    <div class="card">
        <div class="card-title">🎯 Sniper Settings</div>
        <label>Coin Symbol (p.sh. PEPEUSDT)</label>
        <input type="text" id="symbol" placeholder="PEPEUSDT" style="text-transform: uppercase;" autocomplete="off">
        
        <div class="grid-2">
            <div>
                <label>Ora e Listimit</label>
                <input type="time" id="listTime" value="14:00">
            </div>
            <div>
                <label>Shuma (USDT)</label>
                <input type="number" id="amount" value="10" min="1" step="1">
            </div>
        </div>
        
        <div class="grid-2" style="margin-top: 10px;">
            <div>
                <label>Max Buy Price</label>
                <input type="number" id="maxPrice" value="0.001" step="0.000001">
            </div>
            <div>
                <label>Check Interval</label>
                <select id="checkInterval">
                    <option value="500">500ms (e shpejtë)</option>
                    <option value="1000" selected>1 sekondë</option>
                    <option value="2000">2 sekonda</option>
                </select>
            </div>
        </div>
    </div>

    <!-- TP/SL Settings -->
    <div class="card">
        <div class="card-title">📊 Auto TP/SL</div>
        <div class="grid-2">
            <div>
                <label>🎯 TP1 (%)</label>
                <input type="number" id="tp1" value="150" step="10">
                <small style="color: #8b949e;">Shit 50%</small>
            </div>
            <div>
                <label>🚀 TP2 (%)</label>
                <input type="number" id="tp2" value="250" step="10">
                <small style="color: #8b949e;">Shit 100%</small>
            </div>
        </div>
        <div class="grid-2" style="margin-top: 10px;">
            <div>
                <label>🛑 Stop Loss (%)</label>
                <input type="number" id="sl" value="-20" step="5">
            </div>
            <div>
                <label>Trailing SL</label>
                <select id="trailingSL">
                    <option value="false">Jo</option>
                    <option value="true">Po (-10% nga max)</option>
                </select>
            </div>
        </div>
    </div>

    <!-- Control -->
    <div class="card">
        <div class="countdown hidden" id="countdown">00:00:00</div>
        <button class="btn btn-arm" id="btnArm" onclick="armSniper()">🎯 ARM SNIPER</button>
        <button class="btn btn-disarm hidden" id="btnDisarm" onclick="disarm()">⏹️ DISARM</button>
        
        <div id="positionCard" class="hidden" style="margin-top: 20px;">
            <div class="position-info">
                <div style="display: flex; justify-content: space-between; margin-bottom: 10px;">
                    <strong id="posSymbol">--</strong>
                    <span id="posExchange" style="color: #f0b90b;">--</span>
                </div>
                <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 10px; font-size: 13px;">
                    <div>Entry: <span id="posEntry">--</span></div>
                    <div>Current: <span id="posCurrent">--</span></div>
                    <div>P&L: <span id="posPnl" class="profit-positive">--</span></div>
                    <div>Size: <span id="posSize">--</span></div>
                </div>
            </div>
        </div>
    </div>

    <!-- Log -->
    <div class="card">
        <div class="card-title">📋 Log</div>
        <div class="log" id="log"></div>
    </div>

    <script>
        // ==================== CORS PROXY CONFIGURATION ====================
        const CORS_PROXY = 'https://api.allorigins.win/raw?url=';
        
        // ==================== STATE ====================
        let armed = false;
        let targetTime = null;
        let countdownInterval = null;
        let positionMonitor = null;
        let currentPosition = null;
        let currentExchange = 'bitget';
        let audioCtx = null;

        // ==================== EXCHANGE SWITCH ====================
        function switchExchange(ex) {
            currentExchange = ex;
            if (ex === 'bitget') {
                document.getElementById('tabBitget').classList.add('active-tab');
                document.getElementById('tabMexc').classList.remove('active-tab');
                document.getElementById('bitgetConfig').classList.remove('hidden');
                document.getElementById('mexcConfig').classList.add('hidden');
            } else {
                document.getElementById('tabMexc').classList.add('active-tab');
                document.getElementById('tabBitget').classList.remove('active-tab');
                document.getElementById('mexcConfig').classList.remove('hidden');
                document.getElementById('bitgetConfig').classList.add('hidden');
            }
            log(`🏦 U zgjodh: ${ex === 'bitget' ? 'Bitget' : 'MEXC'}`, 'info');
        }

        // ==================== AUDIO ====================
        function playAlert(freq = 800, duration = 200) {
            try {
                if (!audioCtx) audioCtx = new (window.AudioContext || window.webkitAudioContext)();
                const osc = audioCtx.createOscillator();
                const gain = audioCtx.createGain();
                osc.connect(gain);
                gain.connect(audioCtx.destination);
                osc.frequency.value = freq;
                gain.gain.value = 0.3;
                osc.start();
                setTimeout(() => osc.stop(), duration);
            } catch(e) {}
        }

        // ==================== LOG ====================
        function log(msg, type = 'info') {
            const logDiv = document.getElementById('log');
            const time = new Date().toLocaleTimeString();
            const entry = document.createElement('div');
            entry.className = `log-entry ${type}`;
            entry.innerHTML = `<span style="color: #666;">[${time}]</span> ${msg}`;
            logDiv.insertBefore(entry, logDiv.firstChild);
            while (logDiv.children.length > 50) logDiv.removeChild(logDiv.lastChild);
        }

        // ==================== TELEGRAM ====================
        async function sendTelegram(msg) {
            const token = document.getElementById('tgToken').value;
            const chatId = document.getElementById('tgChat').value;
            if (!token || !chatId) return;
            
            try {
                await fetch(`https://api.telegram.org/bot${token}/sendMessage`, {
                    method: 'POST',
                    headers: {'Content-Type': 'application/json'},
                    body: JSON.stringify({chat_id: chatId, text: msg, parse_mode: 'HTML'})
                });
            } catch(e) {}
        }

        async function testTelegram() {
            const btn = event.target;
            btn.textContent = 'Duke dërguar...';
            await sendTelegram('✅ <b>Test i suksesshëm!</b>\nSniper Pro është gati.');
            btn.textContent = '🧪 Testo Telegram';
            log('Mesazh testi u dërgua', 'success');
        }

        // ==================== BITGET API (with CORS Proxy) ====================
        async function bitgetRequest(endpoint, method = 'GET', body = null) {
            const apiKey = document.getElementById('bitgetKey').value;
            const secret = document.getElementById('bitgetSecret').value;
            const passphrase = document.getElementById('bitgetPass').value;
            
            const timestamp = Date.now().toString();
            const bodyStr = body ? JSON.stringify(body) : '';
            
            const msg = timestamp + method + endpoint + bodyStr;
            const encoder = new TextEncoder();
            const key = await crypto.subtle.importKey('raw', encoder.encode(secret), 
                {name: 'HMAC', hash: 'SHA-256'}, false, ['sign']);
            const sig = await crypto.subtle.sign('HMAC', key, encoder.encode(msg));
            const signature = btoa(String.fromCharCode(...new Uint8Array(sig)));
            
            const headers = {
                'ACCESS-KEY': apiKey,
                'ACCESS-SIGN': signature,
                'ACCESS-TIMESTAMP': timestamp,
                'ACCESS-PASSPHRASE': passphrase,
                'Content-Type': 'application/json'
            };
            
            const targetUrl = `https://api.bitget.com${endpoint}`;
            const proxyUrl = CORS_PROXY + encodeURIComponent(targetUrl);
            
            const opts = { method, headers };
            if (body) opts.body = bodyStr;
            
            const res = await fetch(proxyUrl, opts);
            return await res.json();
        }

        async function getBitgetPrice(symbol) {
            try {
                const targetUrl = `https://api.bitget.com/api/spot/v1/market/ticker?symbol=${symbol}`;
                const proxyUrl = CORS_PROXY + encodeURIComponent(targetUrl);
                const res = await fetch(proxyUrl);
                const data = await res.json();
                return parseFloat(data.data.last);
            } catch(e) { 
                log('CORS Error: Provo me WiFi ose rifresko', 'error');
                return null; 
            }
        }

        async function buyBitget(symbol, amount) {
            const price = await getBitgetPrice(symbol);
            const maxPrice = parseFloat(document.getElementById('maxPrice').value);
            
            if (!price) return {error: 'Nuk u mor çmimi (CORS?)'};
            if (price > maxPrice) return {error: `Çmimi ${price} > Max ${maxPrice}`, skipped: true};
            
            const size = (amount / price).toFixed(8);
            const body = {symbol, orderType: 'market', side: 'buy', size, force: 'normal'};
            const result = await bitgetRequest('/api/spot/v1/trade/placeOrder', 'POST', body);
            
            if (result.code === '00000') {
                return {success: true, price, size: parseFloat(size), orderId: result.data.orderId};
            }
            return {success: false, error: result.msg};
        }

        async function sellBitget(symbol, size) {
            const body = {symbol, orderType: 'market', side: 'sell', size: size.toFixed(8), force: 'normal'};
            return await bitgetRequest('/api/spot/v1/trade/placeOrder', 'POST', body);
        }

        // ==================== MEXC API (with CORS Proxy) ====================
        async function mexcRequest(endpoint, method = 'GET', params = {}) {
            const apiKey = document.getElementById('mexcKey').value;
            const secret = document.getElementById('mexcSecret').value;
            
            const timestamp = Date.now();
            params.timestamp = timestamp;
            
            const query = Object.keys(params).sort()
                .map(k => `${k}=${params[k]}`).join('&');
            
            const encoder = new TextEncoder();
            const key = await crypto.subtle.importKey('raw', encoder.encode(secret),
                {name: 'HMAC', hash: 'SHA-256'}, false, ['sign']);
            const sig = await crypto.subtle.sign('HMAC', key, encoder.encode(query));
            const sigHex = Array.from(new Uint8Array(sig))
                .map(b => b.toString(16).padStart(2, '0')).join('');
            
            const targetUrl = `https://api.mexc.com${endpoint}?${query}&signature=${sigHex}`;
            const proxyUrl = CORS_PROXY + encodeURIComponent(targetUrl);
            
            const res = await fetch(proxyUrl, {
                method,
                headers: {'X-MEXC-APIKEY': apiKey, 'Content-Type': 'application/json'}
            });
            return await res.json();
        }

        async function getMexcPrice(symbol) {
            try {
                const targetUrl = `https://api.mexc.com/api/v3/ticker/price?symbol=${symbol}`;
                const proxyUrl = CORS_PROXY + encodeURIComponent(targetUrl);
                const res = await fetch(proxyUrl);
                const data = await res.json();
                return parseFloat(data.price);
            } catch(e) { 
                log('CORS Error: Provo me WiFi ose rifresko', 'error');
                return null; 
            }
        }

        async function buyMexc(symbol, amount) {
            const price = await getMexcPrice(symbol);
            const maxPrice = parseFloat(document.getElementById('maxPrice').value);
            
            if (!price) return {error: 'Nuk u mor çmimi (CORS?)'};
            if (price > maxPrice) return {error: `Çmimi ${price} > Max ${maxPrice}`, skipped: true};
            
            const params = {
                symbol: symbol,
                side: 'BUY',
                type: 'MARKET',
                quoteOrderQty: amount
            };
            
            const result = await mexcRequest('/api/v3/order', 'POST', params);
            
            if (result.orderId) {
                const size = amount / price;
                return {success: true, price, size, orderId: result.orderId};
            }
            return {success: false, error: result.msg || 'Gabim'};
        }

        async function sellMexc(symbol, quantity) {
            const params = {
                symbol: symbol,
                side: 'SELL',
                type: 'MARKET',
                quantity: quantity
            };
            return await mexcRequest('/api/v3/order', 'POST', params);
        }

        // ==================== SNIPER LOGIC ====================
        function armSniper() {
            const symbol = document.getElementById('symbol').value.toUpperCase();
            const timeStr = document.getElementById('listTime').value;
            const amount = parseFloat(document.getElementById('amount').value);
            
            if (!symbol) { alert('Vendos simbolin!'); return; }
            if (!timeStr) { alert('Vendos orën!'); return; }
            
            let targetHours, targetMinutes;
            if (timeStr.includes('AM') || timeStr.includes('PM') || timeStr.includes('am') || timeStr.includes('pm')) {
                const match = timeStr.match(/(\d+):(\d+)\s*(AM|PM|am|pm)/);
                if (match) {
                    let hours = parseInt(match[1]);
                    const minutes = parseInt(match[2]);
                    const period = match[3].toUpperCase();
                    if (period === 'PM' && hours !== 12) hours += 12;
                    if (period === 'AM' && hours === 12) hours = 0;
                    targetHours = hours;
                    targetMinutes = minutes;
                }
            } else {
                const parts = timeStr.split(':');
                targetHours = parseInt(parts[0]);
                targetMinutes = parseInt(parts[1]);
            }
            
            const now = new Date();
            targetTime = new Date();
            targetTime.setHours(targetHours, targetMinutes, 0, 0);
            if (targetTime < now) targetTime.setDate(targetTime.getDate() + 1);
            
            armed = true;
            
            document.getElementById('btnArm').classList.add('hidden');
            document.getElementById('btnDisarm').classList.remove('hidden');
            document.getElementById('countdown').classList.remove('hidden');
            document.getElementById('statusBadge').className = 'status waiting';
            document.getElementById('statusBadge').textContent = '● Armed';
            
            const exName = currentExchange === 'bitget' ? 'Bitget' : 'MEXC';
            log(`🎯 <b>SNIPER ARMED</b> në ${exName}`, 'warning');
            log(`📊 Coin: ${symbol} | Amount: ${amount} USDT`, 'info');
            
            sendTelegram(`🎯 <b>SNIPER ARMED (${exName})</b>\nCoin: <code>${symbol}</code>\nTime: ${targetHours}:${targetMinutes.toString().padStart(2,'0')}`);
            
            updateCountdown();
            countdownInterval = setInterval(updateCountdown, 100);
            
            const delay = targetTime - new Date();
            setTimeout(() => executeBuy(symbol, amount), delay);
        }

        function updateCountdown() {
            if (!armed) return;
            const diff = targetTime - new Date();
            if (diff <= 0) {
                document.getElementById('countdown').textContent = '00:00:00.000';
                return;
            }
            const h = Math.floor(diff / 3600000);
            const m = Math.floor((diff % 3600000) / 60000);
            const s = Math.floor((diff % 60000) / 1000);
            const ms = diff % 1000;
            document.getElementById('countdown').textContent = 
                `${h.toString().padStart(2,'0')}:${m.toString().padStart(2,'0')}:${s.toString().padStart(2,'0')}.${ms.toString().padStart(3,'0')}`;
        }

        async function executeBuy(symbol, amount) {
            log('🔥 <b>FIRE! Duke blerë...</b>', 'success');
            playAlert(1000, 300);
            document.getElementById('countdown').textContent = 'FIRE!';
            
            const startTime = Date.now();
            
            try {
                let result;
                if (currentExchange === 'bitget') {
                    result = await buyBitget(symbol, amount);
                } else {
                    result = await buyMexc(symbol, amount);
                }
                
                const elapsed = Date.now() - startTime;
                
                if (result.success) {
                    log(`✅ <b>BLERJE në ${elapsed}ms!</b> @ ${result.price}`, 'success');
                    
                    currentPosition = {
                        symbol: symbol,
                        entryPrice: result.price,
                        currentPrice: result.price,
                        originalSize: result.size,
                        remainingSize: result.size,
                        exchange: currentExchange,
                        startTime: Date.now()
                    };
                    
                    document.getElementById('positionCard').classList.remove('hidden');
                    document.getElementById('posSymbol').textContent = symbol;
                    document.getElementById('posExchange').textContent = currentExchange.toUpperCase();
                    document.getElementById('posEntry').textContent = result.price;
                    document.getElementById('posSize').textContent = result.size.toFixed(4);
                    document.getElementById('statusBadge').className = 'status active';
                    document.getElementById('statusBadge').textContent = '● Monitoring';
                    
                    sendTelegram(`✅ <b>BLERJE E SUKSESSHME (${currentExchange.toUpperCase()})</b>\nCoin: <code>${symbol}</code>\nPrice: ${result.price}\nTime: ${elapsed}ms`);
                    
                    const checkInt = parseInt(document.getElementById('checkInterval').value);
                    positionMonitor = setInterval(() => monitorPosition(), checkInt);
                    
                } else if (result.skipped) {
                    log(`⏭️ SKIP: ${result.error}`, 'warning');
                    disarm();
                } else {
                    throw new Error(result.error);
                }
                
            } catch (e) {
                log(`❌ <b>GABIM:</b> ${e.message}`, 'error');
                sendTelegram(`❌ <b>FAILED</b>\n${symbol}: ${e.message}`);
                disarm();
            }
        }

        async function monitorPosition() {
            if (!currentPosition) return;
            
            const { symbol, entryPrice, remainingSize, exchange } = currentPosition;
            
            let currentPrice;
            if (exchange === 'bitget') {
                currentPrice = await getBitgetPrice(symbol);
            } else {
                currentPrice = await getMexcPrice(symbol);
            }
            
            if (!currentPrice) return;
            
            currentPosition.currentPrice = currentPrice;
            const pnl = ((currentPrice - entryPrice) / entryPrice) * 100;
            
            document.getElementById('posCurrent').textContent = currentPrice.toFixed(8);
            const pnlEl = document.getElementById('posPnl');
            pnlEl.textContent = `${pnl >= 0 ? '+' : ''}${pnl.toFixed(2)}%`;
            pnlEl.className = pnl >= 0 ? 'profit-positive' : 'profit-negative';
            
            const tp1 = parseFloat(document.getElementById('tp1').value);
            const tp2 = parseFloat(document.getElementById('tp2').value);
            const sl = parseFloat(document.getElementById('sl').value);
            
            if (pnl <= sl) {
                await executeSell(symbol, remainingSize, 'STOP LOSS', pnl);
                return;
            }
            
            if (pnl >= tp1 && !currentPosition.tp1Done) {
                const sellSize = currentPosition.originalSize * 0.5;
                await executeSell(symbol, sellSize, 'TP1', pnl);
                currentPosition.tp1Done = true;
                currentPosition.remainingSize -= sellSize;
                return;
            }
            
            if (pnl >= tp2 && currentPosition.tp1Done && !currentPosition.tp2Done) {
                await executeSell(symbol, currentPosition.remainingSize, 'TP2', pnl);
                currentPosition.tp2Done = true;
                currentPosition.remainingSize = 0;
                
                setTimeout(() => {
                    log(`🏁 <b>Position complete!</b>`, 'success');
                    sendTelegram(`🏁 <b>POSITION COMPLETE</b>\n${symbol}\nP&L: +${pnl.toFixed(2)}%`);
                    disarm();
                }, 2000);
            }
        }

        async function executeSell(symbol, size, reason, pnl) {
            playAlert(1200, 400);
            log(`💸 <b>SELLING:</b> ${reason}`, 'warning');
            
            try {
                let result;
                if (currentPosition.exchange === 'bitget') {
                    result = await sellBitget(symbol, size);
                    if (result.code === '00000') {
                        log(`✅ <b>SOLD:</b> ${size.toFixed(4)}`, 'success');
                        sendTelegram(`💰 <b>SELL (${reason})</b>\n${symbol}\nP&L: ${pnl.toFixed(2)}%`);
                    }
                } else {
                    result = await sellMexc(symbol, size);
                    if (result.orderId) {
                        log(`✅ <b>SOLD:</b> ${size.toFixed(4)}`, 'success');
                        sendTelegram(`💰 <b>SELL (${reason})</b>\n${symbol}\nP&L: ${pnl.toFixed(2)}%`);
                    }
                }
            } catch (e) {
                log(`❌ Sell failed: ${e.message}`, 'error');
            }
        }

        function disarm() {
            armed = false;
            clearInterval(countdownInterval);
            clearInterval(positionMonitor);
            currentPosition = null;
            
            document.getElementById('btnArm').classList.remove('hidden');
            document.getElementById('btnDisarm').classList.add('hidden');
            document.getElementById('countdown').classList.add('hidden');
            document.getElementById('positionCard').classList.add('hidden');
            document.getElementById('statusBadge').className = 'status inactive';
            document.getElementById('statusBadge').textContent = '● Ndalur';
            
            log('⏹️ <b>Sniper u çarmatos</b>', 'info');
        }

        // Save/Load
        document.addEventListener('change', () => {
            const config = {
                bitgetKey: document.getElementById('bitgetKey').value,
                mexcKey: document.getElementById('mexcKey').value,
                symbol: document.getElementById('symbol').value,
                amount: document.getElementById('amount').value,
                listTime: document.getElementById('listTime').value,
                maxPrice: document.getElementById('maxPrice').value,
                tp1: document.getElementById('tp1').value,
                tp2: document.getElementById('tp2').value,
                sl: document.getElementById('sl').value
            };
            localStorage.setItem('sniperConfig', JSON.stringify(config));
        });

        window.onload = () => {
            const saved = localStorage.getItem('sniperConfig');
            if (saved) {
                const c = JSON.parse(saved);
                if (c.bitgetKey) document.getElementById('bitgetKey').value = c.bitgetKey;
                if (c.mexcKey) document.getElementById('mexcKey').value = c.mexcKey;
                if (c.symbol) document.getElementById('symbol').value = c.symbol;
                if (c.amount) document.getElementById('amount').value = c.amount;
                if (c.listTime) document.getElementById('listTime').value = c.listTime;
                if (c.maxPrice) document.getElementById('maxPrice').value = c.maxPrice;
                if (c.tp1) document.getElementById('tp1').value = c.tp1;
                if (c.tp2) document.getElementById('tp2').value = c.tp2;
                if (c.sl) document.getElementById('sl').value = c.sl;
            }
            log('🤖 Sniper Pro (CORS Fixed) u ngarkua', 'info');
        };
    </script>
</body>
</html>
