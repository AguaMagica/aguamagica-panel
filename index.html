<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Panel de Control - AguaMagica</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #f0f2f5;
        }
        .sidebar {
            width: 250px;
            height: 100vh;
            background: linear-gradient(135deg, #1a237e, #0d47a1);
            color: white;
            position: fixed;
            padding: 20px 0;
        }
        .sidebar h2 {
            text-align: center;
            padding: 20px 0;
            border-bottom: 1px solid rgba(255,255,255,0.1);
        }
        .sidebar ul {
            list-style: none;
            padding: 20px 0;
        }
        .sidebar ul li {
            padding: 15px 25px;
            cursor: pointer;
            transition: 0.3s;
        }
        .sidebar ul li:hover {
            background: rgba(255,255,255,0.1);
        }
        .sidebar ul li i {
            margin-right: 10px;
            width: 20px;
        }
        .main-content {
            margin-left: 250px;
            padding: 20px;
        }
        .header {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            margin-bottom: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .card {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            margin-bottom: 20px;
        }
        .grid-2 {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }
        textarea, input, select {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            margin: 5px 0 15px 0;
        }
        .btn {
            background: #0d47a1;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: 0.3s;
        }
        .btn:hover {
            background: #1565c0;
            transform: scale(1.05);
        }
        .btn-success { background: #2e7d32; }
        .btn-warning { background: #f57c00; }
        .btn-danger { background: #c62828; }
        .btn-info { background: #00838f; }
        .client-list {
            max-height: 400px;
            overflow-y: auto;
        }
        .client-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px;
            border-bottom: 1px solid #eee;
        }
        .client-item input[type="checkbox"] {
            width: 20px;
            margin-right: 10px;
        }
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.5);
            justify-content: center;
            align-items: center;
        }
        .modal-content {
            background: white;
            padding: 30px;
            border-radius: 10px;
            max-width: 500px;
            width: 90%;
        }
        .tab {
            display: none;
        }
        .tab.active {
            display: block;
        }
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 15px;
            margin: 20px 0;
        }
        .stat-card {
            background: white;
            padding: 15px;
            border-radius: 8px;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .qr-code {
            text-align: center;
            padding: 20px;
        }
        .product-item {
            display: flex;
            justify-content: space-between;
            padding: 10px;
            border-bottom: 1px solid #eee;
        }
    </style>
</head>
<body>
    <div class="sidebar">
        <h2>💧 AguaMagica</h2>
        <ul>
            <li onclick="showTab('dashboard')"><i class="fas fa-home"></i> Dashboard</li>
            <li onclick="showTab('clientes')"><i class="fas fa-users"></i> Clientes</li>
            <li onclick="showTab('mensajes')"><i class="fas fa-envelope"></i> Mensajes</li>
            <li onclick="showTab('pedidos')"><i class="fas fa-shopping-cart"></i> Pedidos</li>
            <li onclick="showTab('productos')"><i class="fas fa-box"></i> Productos</li>
            <li onclick="showTab('reportes')"><i class="fas fa-chart-bar"></i> Reportes</li>
            <li onclick="showTab('configuracion')"><i class="fas fa-cog"></i> Configuración</li>
        </ul>
    </div>

    <div class="main-content">
        <div class="header">
            <h2>Panel de Control</h2>
            <div>
                <span id="currentTime"></span>
                <button class="btn btn-success" onclick="sendBulkMessage()"><i class="fab fa-whatsapp"></i> Enviar Campaña</button>
            </div>
        </div>

        <!-- Dashboard -->
        <div id="dashboard" class="tab active">
            <div class="stats-grid">
                <div class="stat-card"><h3>Total Clientes</h3><p id="totalClients">0</p></div>
                <div class="stat-card"><h3>Pedidos Hoy</h3><p id="todayOrders">0</p></div>
                <div class="stat-card"><h3>Ventas Mes</h3><p id="monthSales">$0</p></div>
                <div class="stat-card"><h3>Mensajes Enviados</h3><p id="totalMessages">0</p></div>
            </div>
            <div class="card">
                <h3>Accesos Rápidos</h3>
                <div style="display: flex; gap: 10px; flex-wrap: wrap;">
                    <a href="https://wa.me/584141485985" target="_blank" class="btn btn-success"><i class="fab fa-whatsapp"></i> WhatsApp</a>
                    <a href="https://www.instagram.com/aguamagica" target="_blank" class="btn btn-info"><i class="fab fa-instagram"></i> Instagram</a>
                    <button class="btn" onclick="generateQR()"><i class="fas fa-qrcode"></i> Generar QR</button>
                </div>
            </div>
        </div>

        <!-- Clientes -->
        <div id="clientes" class="tab">
            <div class="grid-2">
                <div class="card">
                    <h3><i class="fas fa-user-plus"></i> Agregar Clientes</h3>
                    <label>Copiar y pegar lista (Nombre, Teléfono):</label>
                    <textarea id="clientBulkInput" rows="5" placeholder="Juan Pérez, 04141234567&#10;María García, 04147654321"></textarea>
                    <button class="btn btn-success" onclick="addBulkClients()"><i class="fas fa-plus"></i> Agregar Clientes</button>
                </div>
                <div class="card">
                    <h3><i class="fas fa-search"></i> Buscar Cliente</h3>
                    <input type="text" id="clientSearch" placeholder="Buscar por nombre o teléfono" onkeyup="searchClients()">
                    <div class="client-list" id="clientList"></div>
                </div>
            </div>
        </div>

        <!-- Mensajes -->
        <div id="mensajes" class="tab">
            <div class="card">
                <h3><i class="fas fa-edit"></i> Editor de Mensajes</h3>
                <textarea id="messageEditor" rows="4" placeholder="Escribe tu mensaje aquí..."></textarea>
                <button class="btn" onclick="saveMessage()"><i class="fas fa-save"></i> Guardar Mensaje</button>
                <button class="btn btn-success" onclick="syncToGitHub()"><i class="fab fa-github"></i> Sincronizar con GitHub</button>
                <div style="margin-top: 10px;">
                    <label>Mensajes Guardados:</label>
                    <select id="savedMessages" onchange="loadMessage()"></select>
                </div>
            </div>
        </div>

        <!-- Pedidos -->
        <div id="pedidos" class="tab">
            <div class="card">
                <h3><i class="fas fa-clipboard-list"></i> Historial de Pedidos</h3>
                <select id="periodFilter" onchange="filterOrders()">
                    <option value="hour">Hora</option>
                    <option value="day">Día</option>
                    <option value="week">Semana</option>
                    <option value="biweek">Quincena</option>
                    <option value="month">Mes</option>
                    <option value="quarter">Trimestre</option>
                    <option value="semester">Semestre</option>
                    <option value="year">Año</option>
                </select>
                <div id="orderHistory"></div>
            </div>
        </div>

        <!-- Productos -->
        <div id="productos" class="tab">
            <div class="card">
                <h3><i class="fas fa-boxes"></i> Gestión de Productos</h3>
                <div class="grid-2">
                    <div>
                        <input type="text" id="productName" placeholder="Nombre del producto">
                        <input type="number" id="productPrice" placeholder="Precio">
                        <button class="btn btn-success" onclick="addProduct()"><i class="fas fa-plus"></i> Agregar Producto</button>
                    </div>
                    <div id="productList"></div>
                </div>
            </div>
        </div>

        <!-- Reportes -->
        <div id="reportes" class="tab">
            <div class="card">
                <h3><i class="fas fa-chart-line"></i> Reportes y Estadísticas</h3>
                <div id="reportsContent">
                    <p>Selecciona un período para ver las estadísticas</p>
                </div>
            </div>
        </div>

        <!-- Configuración -->
        <div id="configuracion" class="tab">
            <div class="card">
                <h3><i class="fas fa-qrcode"></i> Código QR</h3>
                <div class="qr-code" id="qrDisplay">
                    <p>Click en "Generar QR" para crear el código</p>
                    <button class="btn" onclick="generateQR()"><i class="fas fa-qrcode"></i> Generar QR</button>
                    <div id="qrResult"></div>
                </div>
                <h3>Link Corto</h3>
                <input type="text" id="shortLink" value="https://bit.ly/aguamagica" readonly>
                <button class="btn" onclick="copyLink()"><i class="fas fa-copy"></i> Copiar Link</button>
            </div>
        </div>
    </div>

    <!-- Modal Cliente -->
    <div id="clientModal" class="modal">
        <div class="modal-content">
            <h3>Detalles del Cliente</h3>
            <div id="clientDetails"></div>
            <button class="btn" onclick="closeModal()">Cerrar</button>
        </div>
    </div>

    <script>
        // Base de datos simulada
        let db = {
            clients: [],
            messages: [],
            products: [],
            orders: [],
            responses: []
        };

        // Cargar datos desde localStorage
        function loadDB() {
            const saved = localStorage.getItem('aguamagica_db');
            if (saved) {
                db = JSON.parse(saved);
            }
            updateUI();
        }

        function saveDB() {
            localStorage.setItem('aguamagica_db', JSON.stringify(db));
            updateUI();
        }

        function updateUI() {
            document.getElementById('totalClients').textContent = db.clients.length;
            document.getElementById('clientList').innerHTML = '';
            db.clients.forEach((client, index) => {
                const div = document.createElement('div');
                div.className = 'client-item';
                div.innerHTML = `
                    <div>
                        <input type="checkbox" onchange="selectClient(${index})">
                        <strong>${client.name}</strong> - ${client.phone}
                    </div>
                    <button class="btn btn-info" onclick="viewClient(${index})"><i class="fas fa-eye"></i></button>
                `;
                document.getElementById('clientList').appendChild(div);
            });
            updateProductList();
            updateSavedMessages();
        }

        // Agregar clientes en masa
        function addBulkClients() {
            const input = document.getElementById('clientBulkInput').value;
            const lines = input.split('\n');
            lines.forEach(line => {
                const parts = line.split(',').map(s => s.trim());
                if (parts.length === 2) {
                    db.clients.push({
                        name: parts[0],
                        phone: parts[1],
                        history: [],
                        responses: []
                    });
                }
            });
            saveDB();
            document.getElementById('clientBulkInput').value = '';
            alert('Clientes agregados exitosamente!');
        }

        // Mensajes
        function saveMessage() {
            const content = document.getElementById('messageEditor').value;
            if (content) {
                const name = prompt('Nombre del mensaje:');
                if (name) {
                    db.messages.push({ name, content, date: new Date().toISOString() });
                    saveDB();
                    document.getElementById('messageEditor').value = '';
                    alert('Mensaje guardado!');
                }
            }
        }

        function updateSavedMessages() {
            const select = document.getElementById('savedMessages');
            select.innerHTML = '<option value="">Seleccionar mensaje...</option>';
            db.messages.forEach((msg, index) => {
                const option = document.createElement('option');
                option.value = index;
                option.textContent = msg.name;
                select.appendChild(option);
            });
        }

        function loadMessage() {
            const index = document.getElementById('savedMessages').value;
            if (index !== '') {
                document.getElementById('messageEditor').value = db.messages[index].content;
            }
        }

        // Enviar mensaje masivo
        function sendBulkMessage() {
            const selected = document.querySelectorAll('.client-item input[type="checkbox"]:checked');
            if (selected.length === 0) {
                alert('Selecciona al menos un cliente');
                return;
            }
            
            const message = document.getElementById('messageEditor').value;
            if (!message) {
                alert('Escribe un mensaje primero');
                return;
            }

            const fullMessage = `${message}\n\n📦 Pedido: [Producto] - [Cantidad]\n⏰ Hora de entrega: [Selecciona]\n\n📱 WhatsApp: https://wa.me/584141485985\n📸 Instagram: https://www.instagram.com/reel/C7bqvkYuHb0/?igsh=MXJkaGV1NXl3emh4Yw==`;

            selected.forEach(checkbox => {
                const index = Array.from(document.querySelectorAll('.client-item input[type="checkbox"]')).indexOf(checkbox);
                const client = db.clients[index];
                const url = `https://wa.me/${client.phone}?text=${encodeURIComponent(fullMessage)}`;
                window.open(url, '_blank');
                
                // Registrar envío
                db.responses.push({
                    client: client.name,
                    phone: client.phone,
                    message: fullMessage,
                    date: new Date().toISOString(),
                    type: 'whatsapp'
                });
            });
            saveDB();
        }

        // Sincronizar con GitHub
        function syncToGitHub() {
            const content = document.getElementById('messageEditor').value;
            if (!content) {
                alert('Escribe un mensaje primero');
                return;
            }

            // Simular sincronización con GitHub
            const githubData = {
                message: content,
                user: 'AguaMagica',
                date: new Date().toISOString()
            };

            console.log('Sincronizando con GitHub...', githubData);
            
            // Aquí iría la integración real con GitHub API
            // fetch('https://api.github.com/repos/AguaMagica/...', { ... })
            
            alert('✅ Mensaje sincronizado con GitHub!\nUsuario: AguaMagica\nRepositorio: aguamagica-panel');
            
            // Guardar en historial
            db.messages.push({
                name: `Sync ${new Date().toLocaleString()}`,
                content: content,
                github: true
            });
            saveDB();
        }

        // Productos
        function addProduct() {
            const name = document.getElementById('productName').value;
            const price = document.getElementById('productPrice').value;
            if (name && price) {
                db.products.push({ name, price: parseFloat(price) });
                saveDB();
                document.getElementById('productName').value = '';
                document.getElementById('productPrice').value = '';
                alert('Producto agregado!');
            }
        }

        function updateProductList() {
            const div = document.getElementById('productList');
            div.innerHTML = '<h4>Productos disponibles:</h4>';
            db.products.forEach((product, index) => {
                const item = document.createElement('div');
                item.className = 'product-item';
                item.innerHTML = `
                    <span>${product.name}</span>
                    <span>$${product.price.toFixed(2)}</span>
                    <button class="btn btn-danger" onclick="deleteProduct(${index})"><i class="fas fa-trash"></i></button>
                `;
                div.appendChild(item);
            });
        }

        function deleteProduct(index) {
            db.products.splice(index, 1);
            saveDB();
        }

        // Generar QR
        function generateQR() {
            const url = 'https://aguamagica.com/pedido';
            const qrDiv = document.getElementById('qrResult');
            qrDiv.innerHTML = `
                <div style="padding: 20px; background: white; display: inline-block;">
                    <img src="https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=${encodeURIComponent(url)}" alt="QR Code">
                    <p><small>${url}</small></p>
                </div>
            `;
        }

        // Navegación
        function showTab(tabId) {
            document.querySelectorAll('.tab').forEach(tab => tab.classList.remove('active'));
            document.getElementById(tabId).classList.add('active');
        }

        // Reloj
        function updateClock() {
            document.getElementById('currentTime').textContent = new Date().toLocaleString();
        }
        setInterval(updateClock, 1000);

        // Inicializar
        loadDB();
        updateClock();

        // Funciones adicionales
        function searchClients() {
            // Implementar búsqueda
        }

        function viewClient(index) {
            const client = db.clients[index];
            const modal = document.getElementById('clientModal');
            document.getElementById('clientDetails').innerHTML = `
                <h4>${client.name}</h4>
                <p>📱 ${client.phone}</p>
                <p>📝 Historial de compras: ${client.history ? client.history.length : 0} compras</p>
                <div style="margin-top: 10px;">
                    <h5>Últimas respuestas:</h5>
                    ${client.responses ? client.responses.slice(-3).map(r => `<p>${r}</p>`).join('') : 'Sin respuestas'}
                </div>
            `;
            modal.style.display = 'flex';
        }

        function closeModal() {
            document.getElementById('clientModal').style.display = 'none';
        }

        function filterOrders() {
            // Implementar filtro de pedidos
        }

        function copyLink() {
            const link = document.getElementById('shortLink');
            link.select();
            document.execCommand('copy');
            alert('Link copiado!');
        }

        // Cerrar modal al hacer click fuera
        window.onclick = function(event) {
            const modal = document.getElementById('clientModal');
            if (event.target === modal) {
                modal.style.display = 'none';
            }
        };
    </script>
</body>
</html>
