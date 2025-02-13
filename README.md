<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Jualan Abaya</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Jualan Abaya Turki</h1>
        <div class="cart">
            <button onclick="toggleCart()">Keranjang (0)</button>
        </div>
    </header>
    <main>
        <div class="products">
            < !-- Produk Abaya 1 -->
            <div class="product" data-id="1">
                <img src="https://via.placeholder.com/200?text=Abaya+Maroon" alt="Abaya Maroon">
                <h2>Abaya Turki Maroon</h2>
                <p>Abaya Turki dengan desain elegan dan bahan berkualitas.</p>
                <div class="options">
                    <label for="size-maroon">Ukuran:</label>
                    <select id="size-maroon" data-product="1" onchange="updatePriceAndStock(1)">
                        <option value="S">S - Rp105.000</option>
                        <option value="M">M - Rp115.000</option>
                        <option value="L">L - Rp130.000</option>
                        <option value="XL">XL - Rp140.000</option>
                    </select>
                    <p id="stock-maroon">Stok: 5</p>
                    <button class="add-to-cart" onclick="addToCart(1)">Tambah ke Keranjang</button>
                </div>
            </div>
            < !-- Produk Abaya 2 -->
            <div class="product" data-id="2">
                <img src="https://via.placeholder.com/200?text=Abaya+Hitam" alt="Abaya Hitam">
                <h2>Abaya Turki Hitam</h2>
                <p>Abaya Turki dengan desain elegan dan bahan berkualitas.</p>
                <div class="options">
                    <label for="size-black">Ukuran:</label>
                    <select id="size-black" data-product="2" onchange="updatePriceAndStock(2)">
                        <option value="S">S - Rp105.000</option>
                        <option value="M">M - Rp115.000</option>
                        <option value="L">L - Rp130.000</option>
                        <option value="XL">XL - Rp140.000</option>
                    </select>
                    <p id="stock-black">Stok: 5</p>
                    <button class="add-to-cart" onclick="addToCart(2)">Tambah ke Keranjang</button>
                </div>
            </div>
            < !-- Produk Abaya 3 -->
            <div class="product" data-id="3">
                <img src="https://via.placeholder.com/200?text=Abaya+Army" alt="Abaya Army">
                <h2>Abaya Turki Army</h2>
                <p>Abaya Turki dengan desain elegan dan bahan berkualitas.</p>
                <div class="options">
                    <label for="size-army">Ukuran:</label>
                    <select id="size-army" data-product="3" onchange="updatePriceAndStock(3)">
                        <option value="S">S - Rp105.000</option>
                        <option value="M">M - Rp115.000</option>
                        <option value="L">L - Rp130.000</option>
                        <option value="XL">XL - Rp140.000</option>
                    </select>
                    <p id="stock-army">Stok: 5</p>
                    <button class="add-to-cart" onclick="addToCart(3)">Tambah ke Keranjang</button>
                </div>
            </div>
            < !-- Produk Abaya 4 -->
            <div class="product" data-id="4">
                <img src="https://via.placeholder.com/200?text=Abaya+Mocca" alt="Abaya Mocca">
                <h2>Abaya Turki Mocca</h2>
                <p>Abaya Turki dengan desain elegan dan bahan berkualitas.</p>
                <div class="options">
                    <label for="size-mocca">Ukuran:</label>
                    <select id="size-mocca" data-product="4" onchange="updatePriceAndStock(4)">
                        <option value="S">S - Rp105.000</option>
                        <option value="M">M - Rp115.000</option>
                        <option value="L">L - Rp130.000</option>
                        <option value="XL">XL - Rp140.000</option>
                    </select>
                    <p id="stock-mocca">Stok: 5</p>
                    <button class="add-to-cart" onclick="addToCart(4)">Tambah ke Keranjang</button>
                </div>
            </div>
            < !-- Produk Abaya 5 -->
            <div class="product" data-id="5">
                <img src="https://via.placeholder.com/200?text=Abaya+Putih" alt="Abaya Putih">
                <h2>Abaya Turki Putih</h2>
                <p>Abaya Turki dengan desain elegan dan bahan berkualitas.</p>
                <div class="options">
                    <label for="size-white">Ukuran:</label>
                    <select id="size-white" data-product="5" onchange="updatePriceAndStock(5)">
                        <option value="S">S - Rp105.000</option>
                        <option value="M">M - Rp115.000</option>
                        <option value="L">L - Rp130.000</option>
                        <option value="XL">XL - Rp140.000</option>
                    </select>
                    <p id="stock-white">Stok: 5</p>
                    <button class="add-to-cart" onclick="addToCart(5)">Tambah ke Keranjang</button>
                </div>
            </div>
        </div>
    </main>
    <div id="cart-modal" class="cart-modal">
        <div class="cart-modal-content">
            <h2>Keranjang Belanja</h2>
            <ul id="cart-items"></ul>
            <p>Total: <span id="total-price">Rp0</span></p>
            <button onclick="checkout()">Proses Pembayaran</button>
            <button onclick="closeCart()">Tutup</button>
        </div>
    </div>
    <script src="script.js"></script>
</body>
</html>
