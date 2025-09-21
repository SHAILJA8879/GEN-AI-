# GEN-AI-

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>AI Marketplace Assistant</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    /* Apply gradient backgrounds to all sections */
section {
  padding-top: 60px;
  padding-bottom: 60px;
  border-radius: 12px;
  margin-bottom: 40px;
  color: #1f2937; /* dark text for readability */
  animation: gradientBG 10s ease infinite;
  background: linear-gradient(270deg, #fde68a, #fca5a5, #a5f3fc, #d8b4fe);
  background-size: 800% 800%;
  transition: all 0.5s ease;
}

/* Different vibe for cards inside */
.card {
  background: rgba(255, 255, 255, 0.85);
  border-radius: 12px;
  padding: 15px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  transition: transform 0.4s ease, box-shadow 0.4s ease;
}
.card:hover {
  transform: translateY(-6px) scale(1.03);
  box-shadow: 0 8px 18px rgba(0,0,0,0.2);
}

/* Gradient Animation */
@keyframes gradientBG {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

  </style>
</head>
<body>
  <header>
    <div class="container" style="display:flex; align-items:center; justify-content:space-between;">
      <h1>🛍️ Artisan AI</h1>
      <nav>
        <a href="#home">Home</a>
        <a href="#features">Features</a>
        <a href="#marketplace">Marketplace</a>
        <a href="#upload">For Artisans</a>
        <a href="#chat">Chat</a>
      </nav>
    </div>
  </header>

  <!-- Home -->
  <section id="home" class="container">
    <div class="card">
      <h2>Turn Handmade into Headlines</h2>
      <p>Upload a photo and let AI generate title, price, and marketing copy — making it easy for artisans to reach buyers worldwide.</p>
      <button onclick="location.href='#features'">Get Started</button>
    </div>
  </section>

  <!-- Features -->
  <section id="features" class="container">
    <h2>Features</h2>
    <div class="grid grid-2 features">
      <div class="card">
        <h3>🤖 Auto Listing</h3>
        <p>AI generates title, tags, and price from product images.</p>
      </div>
      <div class="card">
        <h3>🌐 Multilingual</h3>
        <p>Supports regional languages and voice input.</p>
      </div>
      <div class="card">
        <h3>📦 Inventory Alerts</h3>
        <p>Low-stock warnings & festival demand predictions.</p>
      </div>
      <div class="card">
        <h3>📢 Marketing</h3>
        <p>AI-crafted social media posts to boost sales.</p>
      </div>
    </div>
  </section>

  <!-- Marketplace -->
  <section id="marketplace" class="container">
    <h2>Buyer Marketplace</h2>
    <div class="grid grid-2">
      <div class="card">
        <img src="https://images.unsplash.com/photo-1524758631624-e2822e304c36?auto=format&fit=crop&w=800&q=60" alt="Bowl">
        <h3>Handmade Terracotta Bowl</h3>
        <p>₹499</p>
        <button>Buy Now</button>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1540574163026-643ea20ade25?auto=format&fit=crop&w=800&q=60" alt="Scarf">
        <h3>Block-printed Scarf</h3>
        <p>₹699</p>
        <button>Buy Now</button>
      </div>
    </div>
    <section id="marketplace" class="container">
  <h2>Buyer Marketplace</h2>
  <div class="grid grid-2">
    <div class="card">
      <img src="https://images.unsplash.com/photo-1524758631624-e2822e304c36?auto=format&fit=crop&w=800&q=60" alt="Bowl">
      <h3>Handmade Terracotta Bowl</h3>
      <p>₹499</p>
      <button>Buy Now</button>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1540574163026-643ea20ade25?auto=format&fit=crop&w=800&q=60" alt="Scarf">
      <h3>Block-printed Scarf</h3>
      <p>₹699</p>
      <button>Buy Now</button>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1606813903063-5d3fb1c5f5f7?auto=format&fit=crop&w=800&q=60" alt="Lamp">
      <h3>Bamboo Table Lamp</h3>
      <p>₹1,299</p>
      <button>Buy Now</button>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1526045612212-70caf35c14df?auto=format&fit=crop&w=800&q=60" alt="Pottery">
      <h3>Hand-painted Pottery Mug</h3>
      <p>₹349</p>
      <button>Buy Now</button>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1600185365483-26d6c2e6b9db?auto=format&fit=crop&w=800&q=60" alt="Jewelry">
      <h3>Tribal Silver Earrings</h3>
      <p>₹899</p>
      <button>Buy Now</button>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1596461404969-9ae70f2830c1?auto=format&fit=crop&w=800&q=60" alt="Bag">
      <h3>Handwoven Jute Bag</h3>
      <p>₹1,099</p>
      <button>Buy Now</button>
    </div>
  </div>
</section>

 

  <!-- For Artisans -->
  <section id="upload" class="container">
    <h2>For Artisans – Upload Product</h2>
    <div class="card">
      <form id="uploadForm">
        <label>Upload Product Image:</label>
        <input type="file" accept="image/*">
        
        <label>Product Name:</label>
        <input type="text" placeholder="Enter product name">

        <label>Description:</label>
        <textarea rows="3" placeholder="Enter short description"></textarea>

        <label>Price (₹):</label>
        <input type="number" placeholder="Enter price">

        <button type="button" onclick="generateSuggestions()">Generate AI Suggestions</button>
      </form>

      <div id="suggestions" class="suggestion-box">
        <h4>AI Suggestions:</h4>
        <p id="title"></p>
        <p id="price"></p>
        <p id="marketing"></p>
      </div>
    </div>
  </section>

  <!-- Chatbot -->
  <section id="chat" class="container">
    <h2>AI Chatbot</h2>
    <div class="card">
      <div class="chatbox" id="chatbox">
        <div class="chat-msg bot">Hello! Ask me about any product or shipping.</div>
      </div>
      <div style="display: flex; margin-top: 10px; gap: 10px;">
        <input type="text" id="message" placeholder="Type a message..." style="flex: 1;">
        <button onclick="sendMessage()">Send</button>
      </div>
    </div>
  </section>

    
  <!-- Tribal Heritage -->
<section id="tribal" class="container">
  <h2 style="text-align:center; font-size:28px; background: linear-gradient(90deg, #f59e0b, #d97706); 
             -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
    🌿 Tribal Heritage of India
  </h2>
  <p style="text-align:center; margin-bottom:30px; font-size:16px; color:#555;">
    A tribute to the rich culture and traditions of India’s tribal communities.
  </p>
  <div class="grid grid-2">
    <div class="card tribal-card">
      <h3>Gond Tribe</h3>
      <p>Largest tribal group in central India, known for Gond art and folklore.</p>
    </div>
    <div class="card tribal-card">
      <h3>Santhal Tribe</h3>
      <p>Eastern India’s major tribe, rich in music, dance, and festivals.</p>
    </div>
    <div class="card tribal-card">
      <h3>Bhils</h3>
      <p>One of the oldest tribes of western India, renowned for archery skills.</p>
    </div>
    <div class="card tribal-card">
      <h3>Khasi Tribe</h3>
      <p>From Meghalaya, famous for matrilineal society and vibrant traditions.</p>
    </div>
    <div class="card tribal-card">
      <h3>Toda Tribe</h3>
      <p>Nilgiri Hills community, known for pastoral lifestyle and embroidery.</p>
    </div>
    <div class="card tribal-card">
      <h3>Warli Tribe</h3>
      <p>Maharashtra’s tribe, celebrated for Warli paintings and eco-living.</p>
    </div>
  </div>
</section>

<style>
/* Tribal section special styles */
.tribal-card {
  background: linear-gradient(135deg, #fff7ed, #ffedd5); /* soft warm gradient */
  color: #333;
  border-left: 6px solid #f59e0b;
  transform: translateY(20px);
  opacity: 0;
  animation: fadeInUp 1s ease forwards;
}
.tribal-card h3 {
  color: #d97706;
}
.tribal-card:hover {
  transform: translateY(-5px) scale(1.02);
  transition: all 0.4s ease;
  box-shadow: 0 6px 15px rgba(0,0,0,0.15);
  background: linear-gradient(135deg, #fff, #fde68a);
}

/* Animation for fade-in effect */
@keyframes fadeInUp {
  0% { opacity: 0; transform: translateY(20px); }
  100% { opacity: 1; transform: translateY(0); }
}
</style>

  </section>


  <footer>
    <p>© 2025 Artisan AI Marketplace — Prototype for Hackathon</p>
  </footer>

  <script>
    function sendMessage() {
      const input = document.getElementById("message");
      const chatbox = document.getElementById("chatbox");
      if (!input.value) return;

      let userMsg = document.createElement("div");
      userMsg.className = "chat-msg user";
      userMsg.innerText = input.value;
      chatbox.appendChild(userMsg);

      setTimeout(() => {
        let botMsg = document.createElement("div");
        botMsg.className = "chat-msg bot";
        botMsg.innerText = "Thanks for asking! Products usually ship within 3-5 days.";
        chatbox.appendChild(botMsg);
        chatbox.scrollTop = chatbox.scrollHeight;
      }, 800);

      input.value = "";
      chatbox.scrollTop = chatbox.scrollHeight;
    }

    function generateSuggestions() {
      const titles = [
        "Authentic Handwoven Scarf",
        "Eco-friendly Bamboo Basket",
        "Hand-painted Terracotta Vase",
        "Traditional Block Print Shawl",
        "Rustic Clay Tea Set"
      ];

      const marketingLines = [
        "Wrap yourself in tradition – crafted with love by artisans.",
        "Sustainably made, perfect for eco-conscious living.",
        "Add a touch of heritage to your home décor.",
        "Unique, handmade, and one-of-a-kind.",
        "Celebrate culture with every purchase."
      ];

      const prices = [499, 599, 749, 899, 999];

      // Pick random suggestions
      const title = titles[Math.floor(Math.random() * titles.length)];
      const marketing = marketingLines[Math.floor(Math.random() * marketingLines.length)];
      const price = "₹" + prices[Math.floor(Math.random() * prices.length)];

      // Show results
      document.getElementById("suggestions").style.display = "block";
      document.getElementById("title").innerHTML = "<b>Title:</b> " + title;
      document.getElementById("price").innerHTML = "<b>Suggested Price:</b> " + price;
      document.getElementById("marketing").innerHTML = "<b>Marketing Copy:</b> " + marketing;
    }
  </script>
</body>
</html>
