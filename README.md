<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Bonrod Supplies — Clothing • Laptops & Accessories • Stationery</title>
  <meta name="description" content="Bonrod Supplies — quality clothing, laptops & accessories, and stationery. One-page shop with add-to-cart functionality." />

  <!-- Tailwind CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    // Tailwind custom color
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            gold: {
              DEFAULT: '#c49b31',
              50: '#fbf6e9',
              100: '#f8f0d6',
              200: '#eedfa6',
              300: '#e6cf7a',
              400: '#d9b94d',
              500: '#c49b31',
              600: '#a87720',
              700: '#865b18',
              800: '#614011',
              900: '#3b2a0b'
            }
          }
        }
      }
    }
  </script>

  <style>
    /* small niceties */
    .product-img { height: 180px; object-fit: cover; }
  </style>
</head>
<body class="bg-gray-50 text-gray-800">

  <!-- Header / Nav -->
  <header class="bg-white shadow-sm sticky top-0 z-40">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-20">
        <div class="flex items-center gap-4">
          <div class="rounded-md bg-gold p-3 text-white font-bold">BR</div>
          <div>
            <a href="#home" class="text-xl font-semibold">Bonrod Supplies</a>
            <div class="text-sm text-gray-500">Clothing • Laptops & Accessories • Stationery</div>
          </div>
        </div>
        <nav class="hidden md:flex items-center gap-6 text-gray-700">
          <a href="#categories" class="hover:text-gold">Categories</a>
          <a href="#featured" class="hover:text-gold">Featured</a>
          <a href="#contact" class="hover:text-gold">Contact</a>
          <button id="cartBtn" class="flex items-center gap-2 bg-gold text-white px-4 py-2 rounded-md">
            Cart (<span id="cartCount">0</span>)
          </button>
        </nav>

        <!-- mobile menu button -->
        <div class="md:hidden">
          <button id="mobileMenuBtn" class="p-2 rounded-md border">
            ☰
          </button>
        </div>
      </div>
    </div>
  </header>

  <!-- Mobile nav -->
  <div id="mobileMenu" class="md:hidden bg-white shadow-sm hidden">
    <div class="px-4 py-3 flex flex-col gap-2">
      <a href="#categories" class="py-2">Categories</a>
      <a href="#featured" class="py-2">Featured</a>
      <a href="#contact" class="py-2">Contact</a>
      <button id="cartBtnMobile" class="py-2 bg-gold text-white rounded-md">Cart (<span id="cartCountMobile">0</span>)</button>
    </div>
  </div>

  <!-- Hero Banner -->
  <section id="home" class="relative overflow-hidden">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8 items-center py-16">
        <div>
          <h1 class="text-4xl sm:text-5xl font-extrabold">Bonrod Supplies</h1>
          <p class="mt-4 text-lg text-gray-700">Quality clothing, reliable laptops & accessories, and stationery to keep your life and business running smoothly. Fast delivery • Warranty on electronics • Bulk discounts available.</p>

          <div class="mt-6 flex gap-3">
            <a href="#featured" class="bg-gold text-white px-5 py-3 rounded-md font-medium">Shop Featured</a>
            <a href="#contact" class="border border-gold text-gold px-5 py-3 rounded-md font-medium">Contact Us</a>
          </div>
        </div>

        <div class="rounded-lg overflow-hidden shadow-lg">
          <img src="https://images.unsplash.com/photo-1545239351-1141bd82e8a6?q=80&w=1200&auto=format&fit=crop&ixlib=rb-4.0.3&s=ea1e6b3f0f0872c9e0f3e8b3f7f1e6b4" alt="store banner" class="w-full h-72 object-cover">
        </div>
      </div>
    </div>
  </section>

  <!-- Categories -->
  <section id="categories" class="py-12">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-2xl font-semibold mb-6">Categories</h2>
      <div class="grid grid-cols-1 sm:grid-cols-3 gap-6">
        <article class="bg-white rounded-lg shadow p-6 text-center">
          <img src="https://images.unsplash.com/photo-1520975910089-8a0c6b4b0b02?q=80&w=800&auto=format&fit=crop&ixlib=rb-4.0.3&s=7cf8c4b40dfb0d6e9abf6a7f1c5b2a2b" alt="clothing" class="h-40 mx-auto object-cover rounded-md mb-4">
          <h3 class="font-semibold">Clothing</h3>
          <p class="text-sm text-gray-600 mt-2">Casual wear, work uniforms, and seasonal collections.</p>
          <a href="#featured" class="mt-4 inline-block text-gold">View clothing</a>
        </article>

        <article class="bg-white rounded-lg shadow p-6 text-center">
          <img src="https://images.unsplash.com/photo-1517336714731-489689fd1ca8?q=80&w=800&auto=format&fit=crop&ixlib=rb-4.0.3&s=9c8f1b2b8d3b9c2a3b9f6d6b0f2a1b2c" alt="laptops" class="h-40 mx-auto object-cover rounded-md mb-4">
          <h3 class="font-semibold">Laptops & Accessories</h3>
          <p class="text-sm text-gray-600 mt-2">Laptops from trusted brands and useful accessories.</p>
          <a href="#featured" class="mt-4 inline-block text-gold">View electronics</a>
        </article>

        <article class="bg-white rounded-lg shadow p-6 text-center">
          <img src="https://images.unsplash.com/photo-1528747045269-390fe33c19d9?q=80&w=800&auto=format&fit=crop&ixlib=rb-4.0.3&s=8f3f4b7b7dbeae2b6c3c1a3b2a4d7c8e" alt="stationery" class="h-40 mx-auto object-cover rounded-md mb-4">
          <h3 class="font-semibold">Stationery</h3>
          <p class="text-sm text-gray-600 mt-2">Notebooks, pens, planners and office essentials.</p>
          <a href="#featured" class="mt-4 inline-block text-gold">View stationery</a>
        </article>
      </div>
    </div>
  </section>

  <!-- Featured products / shop -->
  <section id="featured" class="py-12 bg-gray-100">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between mb-6">
        <h2 class="text-2xl font-semibold">Featured Products</h2>
        <div class="text-sm text-gray-600">Free delivery on orders over KES 10,000</div>
      </div>

      <div id="productsGrid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
        <!-- products are injected by JS -->
      </div>
    </div>
  </section>

  <!-- Cart modal -->
  <div id="cartModal" class="fixed inset-0 bg-black/40 hidden items-center justify-center z-50">
    <div class="bg-white rounded-lg w-full max-w-2xl p-6">
      <div class="flex justify-between items-center mb-4">
        <h3 class="text-lg font-semibold">Your Cart</h3>
        <button id="closeCart" class="text-gray-500">✕</button>
      </div>
      <div id="cartItems" class="space-y-4 max-h-64 overflow-auto">
        <!-- cart items here -->
      </div>

      <div class="mt-4 flex items-center justify-between">
        <div class="font-semibold">Total: <span id="cartTotal">KES 0</span></div>
        <div class="flex gap-3">
          <button id="clearCart" class="px-4 py-2 border rounded-md">Clear</button>
          <button id="checkoutBtn" class="px-4 py-2 bg-gold text-white rounded-md">Checkout</button>
        </div>
      </div>

      <div id="checkoutArea" class="mt-6 hidden">
        <h4 class="font-semibold mb-2">Checkout</h4>
        <form id="checkoutForm" class="grid grid-cols-1 gap-3">
          <input required name="name" placeholder="Full name" class="border p-2 rounded-md" />
          <input required name="email" type="email" placeholder="Email" class="border p-2 rounded-md" />
          <input required name="phone" placeholder="Phone" class="border p-2 rounded-md" />
          <textarea name="address" placeholder="Delivery address" class="border p-2 rounded-md"></textarea>
          <div class="flex gap-2">
            <button type="submit" class="px-4 py-2 bg-gold text-white rounded-md">Place order</button>
            <button type="button" id="cancelCheckout" class="px-4 py-2 border rounded-md">Cancel</button>
          </div>
        </form>
        <p class="text-sm text-gray-500 mt-3">This demo does not process payments. You will receive a simulated confirmation.</p>
      </div>
    </div>
  </div>

  <!-- Contact -->
  <section id="contact" class="py-12">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8 items-start">
        <div>
          <h2 class="text-2xl font-semibold">Contact Bonrod Supplies</h2>
          <p class="mt-2 text-gray-600">Have a question, want bulk pricing, or need support with an order? Use the form — we'll respond within one business day.</p>

          <ul class="mt-6 space-y-3 text-gray-700">
            <li><strong>Phone:</strong> +254 700 000 000</li>
            <li><strong>Email:</strong> info@bonrodsupplies.example</li>
            <li><strong>Location:</strong> Nairobi, Kenya</li>
          </ul>

          <div class="mt-6">
            <h4 class="font-semibold">Store hours</h4>
            <p class="text-sm text-gray-600">Mon–Fri 9:00–18:00 • Sat 9:00–14:00 • Sun closed</p>
          </div>
        </div>

        <div class="bg-white p-6 rounded-lg shadow">
          <form id="contactForm" class="grid gap-3">
            <input required name="name" placeholder="Your name" class="border p-2 rounded-md" />
            <input required name="email" type="email" placeholder="Your email" class="border p-2 rounded-md" />
            <textarea required name="message" placeholder="Message" class="border p-2 rounded-md"></textarea>
            <button type="submit" class="mt-2 bg-gold text-white px-4 py-2 rounded-md">Send message</button>
          </form>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-white border-t">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 py-6 text-sm text-gray-600 flex flex-col sm:flex-row justify-between">
      <div>© <span id="year"></span> Bonrod Supplies — All rights reserved.</div>
      <div class="mt-3 sm:mt-0">Built with care • Local pickup & delivery available</div>
    </div>
  </footer>


  <!-- Scripts: simple product + cart logic -->
  <script>
    document.getElementById('year').textContent = new Date().getFullYear();

    const products = [
      // Clothing
      { id: 'c1', title: 'Classic Polo Shirt', category: 'Clothing', price: 1500, img: 'https://images.unsplash.com/photo-1520975910089-8a0c6b4b0b02?q=80&w=800&auto=format&fit=crop&ixlib=rb-4.0.3&s=7cf8c4b40dfb0d6e9abf6a7f1c5b2a2b' },
      { id: 'c2', title: 'Work Jacket', category: 'Clothing', price: 3200, img: 'https://images.unsplash.com/photo-1543785734-4b1b8f3f0d8b?q=80&w=800&auto=format&fit=crop&ixlib=rb-4.0.3&s=2a3b4c5d6e7f8a9b' },

      // Laptops & Accessories
      { id: 'l1', title: '14" Ultrabook Pro', category: 'Laptops', price: 72000, img: 'https://images.unsplash.com/photo-1517336714731-489689fd1ca8?q=80&w=800&auto=format&fit=crop&ixlib=rb-4.0.3&s=9c8f1b2b8d3b9c2a3b9f6d6b0f2a1b2c' },
      { id: 'a1', title: 'Wireless Mouse', category: 'Accessories', price: 2200, img: 'https://images.unsplash.com/photo-1587825140708-6b8b9b3b6d1f?q=80&w=800&auto=format&fit=crop&ixlib=rb-4.0.3&s=a1b2c3d4e5f6a7b8' },

      // Stationery
      { id: 's1', title: 'A5 Notebook (set of 3)', category: 'Stationery', price: 900, img: 'https://images.unsplash.com/photo-1528747045269-390fe33c19d9?q=80&w=800&auto=format&fit=crop&ixlib=rb-4.0.3&s=8f3f4b7b7dbeae2b6c3c1a3b2a4d7c8e' },
      { id: 's2', title: 'Executive Pen', category: 'Stationery', price: 450, img: 'https://images.unsplash.com/photo-1515879218367-8466d910aaa4?q=80&w=800&auto=format&fit=crop&ixlib=rb-4.0.3&s=b3c4d5e6f7a8b9c0' }
    ];

    // Render products
    const productsGrid = document.getElementById('productsGrid');
    products.forEach(p => {
      const div = document.createElement('div');
      div.className = 'bg-white rounded-lg shadow p-4 flex flex-col';
      div.innerHTML = `
        <img src="${p.img}" alt="${p.title}" class="product-img rounded-md mb-4 w-full">
        <h3 class="font-semibold">${p.title}</h3>
        <div class="text-sm text-gray-500">${p.category}</div>
        <div class="mt-3 flex items-center justify-between">
          <div class="font-semibold">KES ${p.price.toLocaleString()}</div>
          <button data-id="${p.id}" class="addBtn px-3 py-1 bg-gold text-white rounded-md">Add</button>
        </div>
      `;
      productsGrid.appendChild(div);
    });

    // Cart logic
    let cart = JSON.parse(localStorage.getItem('bonrod_cart') || '[]');

    function saveCart() { localStorage.setItem('bonrod_cart', JSON.stringify(cart)); updateCartUI(); }
    function updateCartUI() {
      const count = cart.reduce((s,i)=>s+i.qty,0);
      document.getElementById('cartCount').textContent = count;
      document.getElementById('cartCountMobile').textContent = count;
    }

    function addToCart(id) {
      const prod = products.find(p=>p.id===id);
      if(!prod) return;
      const existing = cart.find(i=>i.id===id);
      if(existing) existing.qty++;
      else cart.push({ id: prod.id, title: prod.title, price: prod.price, qty: 1 });
      saveCart();
    }

    document.addEventListener('click', (e)=>{
      if(e.target.matches('.addBtn')){
        const id = e.target.dataset.id; addToCart(id);
        e.target.textContent = 'Added ✓';
        setTimeout(()=> e.target.textContent = 'Add', 1200);
      }
    });

    // cart modal
    const cartModal = document.getElementById('cartModal');
    const cartItemsEl = document.getElementById('cartItems');
    const cartTotalEl = document.getElementById('cartTotal');

    function renderCart() {
      cartItemsEl.innerHTML = '';
      if(cart.length===0){ cartItemsEl.innerHTML = '<div class="text-gray-600">Your cart is empty.</div>'; cartTotalEl.textContent = 'KES 0'; return; }
      let total = 0;
      cart.forEach(item=>{
        total += item.price * item.qty;
        const row = document.createElement('div');
        row.className = 'flex items-center justify-between';
        row.innerHTML = `
          <div>
            <div class="font-medium">${item.title}</div>
            <div class="text-sm text-gray-500">KES ${item.price.toLocaleString()} × ${item.qty}</div>
          </div>
          <div class="flex items-center gap-2">
            <button class="px-2 py-1 border rounded decBtn" data-id="${item.id}">-</button>
            <button class="px-2 py-1 border rounded incBtn" data-id="${item.id}">+</button>
            <button class="px-2 py-1 text-sm text-red-600 delBtn" data-id="${item.id}">Remove</button>
          </div>
        `;
        cartItemsEl.appendChild(row);
      });
      cartTotalEl.textContent = 'KES ' + total.toLocaleString();
    }

    document.getElementById('cartBtn').addEventListener('click', ()=>{ renderCart(); cartModal.classList.remove('hidden'); cartModal.classList.add('flex'); });
    document.getElementById('cartBtnMobile').addEventListener('click', ()=>{ renderCart(); cartModal.classList.remove('hidden'); cartModal.classList.add('flex'); });
    document.getElementById('closeCart').addEventListener('click', ()=>{ cartModal.classList.add('hidden'); cartModal.classList.remove('flex'); document.getElementById('checkoutArea').classList.add('hidden'); });

    document.getElementById('clearCart').addEventListener('click', ()=>{ cart = []; saveCart(); renderCart(); });

    cartItemsEl.addEventListener('click', (e)=>{
      const id = e.target.dataset.id;
      if(e.target.matches('.incBtn')){ const it = cart.find(i=>i.id===id); if(it) it.qty++; saveCart(); renderCart(); }
      if(e.target.matches('.decBtn')){ const it = cart.find(i=>i.id===id); if(it){ it.qty--; if(it.qty<=0) cart = cart.filter(x=>x.id!==id); saveCart(); renderCart(); }}
      if(e.target.matches('.delBtn')){ cart = cart.filter(x=>x.id!==id); saveCart(); renderCart(); }
    });

    document.getElementById('checkoutBtn').addEventListener('click', ()=>{ document.getElementById('checkoutArea').classList.remove('hidden'); });
    document.getElementById('cancelCheckout').addEventListener('click', ()=>{ document.getElementById('checkoutArea').classList.add('hidden'); });

    document.getElementById('checkoutForm').addEventListener('submit', (e)=>{
      e.preventDefault();
      const data = new FormData(e.target);
      // simulate order
      const name = data.get('name');
      alert('Thank you, ' + name + '! Your order has been placed (simulation). We will contact you by email.');
      cart = [];
      saveCart(); renderCart(); document.getElementById('checkoutArea').classList.add('hidden'); cartModal.classList.add('hidden'); cartModal.classList.remove('flex');
    });

    // Contact form (demo)
    document.getElementById('contactForm').addEventListener('submit', (e)=>{
      e.preventDefault();
      const fm = new FormData(e.target);
      alert('Thanks, ' + fm.get('name') + '. Your message has been received (demo).');
      e.target.reset();
    });

    // Mobile menu toggle
    document.getElementById('mobileMenuBtn').addEventListener('click', ()=>{
      const m = document.getElementById('mobileMenu'); m.classList.toggle('hidden');
    });

    // initialize UI
    updateCartUI();
  </script>
</body>
</html>
