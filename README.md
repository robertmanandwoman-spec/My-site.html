export default function IndustrialChemicalsWebsite() {
  const products = [
    {
      name: "Caustic Soda",
      description: "High-purity sodium hydroxide for industrial manufacturing and water treatment.",
      price: "$320 / Ton",
      image:
        "https://images.unsplash.com/photo-1581093458791-9f3c3900df4b?q=80&w=1200&auto=format&fit=crop",
    },
    {
      name: "Sulfuric Acid",
      description: "Industrial-grade sulfuric acid suitable for chemical processing applications.",
      price: "$450 / Ton",
      image:
        "https://images.unsplash.com/photo-1518770660439-4636190af475?q=80&w=1200&auto=format&fit=crop",
    },
    {
      name: "Methanol",
      description: "Premium methanol for energy, industrial, and laboratory applications.",
      price: "$520 / Ton",
      image:
        "https://images.unsplash.com/photo-1516321497487-e288fb19713f?q=80&w=1200&auto=format&fit=crop",
    },
  ];

  return (
    <div className="min-h-screen bg-slate-100 text-slate-800">
      {/* Header */}
      <header className="bg-slate-900 text-white sticky top-0 z-50 shadow-lg">
        <div className="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between">
          <div>
            <h1 className="text-2xl font-bold tracking-wide">ChemCore Industrial Supplies</h1>
            <p className="text-sm text-slate-300">Trusted Global Chemical Distributor</p>
          </div>

          <nav className="hidden md:flex gap-6 text-sm font-medium">
            <a href="#products" className="hover:text-cyan-400 transition">Products</a>
            <a href="#about" className="hover:text-cyan-400 transition">About</a>
            <a href="#contact" className="hover:text-cyan-400 transition">Contact</a>
          </nav>
        </div>
      </header>

      {/* Hero Section */}
      <section className="relative overflow-hidden bg-gradient-to-r from-slate-900 via-slate-800 to-slate-700 text-white">
        <div className="max-w-7xl mx-auto px-6 py-24 grid md:grid-cols-2 gap-12 items-center">
          <div>
            <h2 className="text-5xl font-extrabold leading-tight mb-6">
              Reliable Industrial Chemicals for Global Industries
            </h2>
            <p className="text-lg text-slate-300 mb-8">
              Supplying premium industrial chemicals for manufacturing, oil & gas,
              agriculture, water treatment, and construction industries.
            </p>

            <div className="flex gap-4 flex-wrap">
              <button className="bg-cyan-500 hover:bg-cyan-400 px-6 py-3 rounded-2xl font-semibold shadow-lg transition">
                Browse Products
              </button>

              <button className="border border-slate-400 hover:bg-white hover:text-slate-900 px-6 py-3 rounded-2xl font-semibold transition">
                Request Quotation
              </button>
            </div>
          </div>

          <div>
            <img
              src="https://images.unsplash.com/photo-1509395176047-4a66953fd231?q=80&w=1200&auto=format&fit=crop"
              alt="Industrial Chemicals"
              className="rounded-3xl shadow-2xl object-cover h-[420px] w-full"
            />
          </div>
        </div>
      </section>

      {/* Product Section */}
      <section id="products" className="max-w-7xl mx-auto px-6 py-20">
        <div className="text-center mb-14">
          <h3 className="text-4xl font-bold mb-4">Featured Products</h3>
          <p className="text-slate-600 max-w-2xl mx-auto">
            Explore our range of industrial-grade chemicals designed to meet international quality standards.
          </p>
        </div>

        <div className="grid md:grid-cols-3 gap-8">
          {products.map((product, index) => (
            <div
              key={index}
              className="bg-white rounded-3xl overflow-hidden shadow-md hover:shadow-2xl transition duration-300"
            >
              <img
                src={product.image}
                alt={product.name}
                className="h-60 w-full object-cover"
              />

              <div className="p-6">
                <h4 className="text-2xl font-bold mb-3">{product.name}</h4>
                <p className="text-slate-600 mb-4">{product.description}</p>

                <div className="flex items-center justify-between">
                  <span className="text-cyan-600 font-bold text-lg">{product.price}</span>
                  <button className="bg-slate-900 text-white px-4 py-2 rounded-xl hover:bg-slate-700 transition">
                    Order Now
                  </button>
                </div>
              </div>
            </div>
          ))}
        </div>
      </section>

      {/* About Section */}
      <section id="about" className="bg-white py-20">
        <div className="max-w-6xl mx-auto px-6 grid md:grid-cols-2 gap-12 items-center">
          <div>
            <img
              src="https://images.unsplash.com/photo-1565043666747-69f6646db940?q=80&w=1200&auto=format&fit=crop"
              alt="Chemical Storage"
              className="rounded-3xl shadow-xl"
            />
          </div>

          <div>
            <h3 className="text-4xl font-bold mb-6">About ChemCore</h3>
            <p className="text-slate-600 mb-4 leading-8">
              ChemCore Industrial Supplies is a trusted supplier of industrial chemicals serving clients worldwide.
              We prioritize safety, quality assurance, and timely delivery.
            </p>

            <p className="text-slate-600 mb-8 leading-8">
              Our logistics network ensures reliable shipping solutions for bulk and containerized chemical products.
            </p>

            <div className="grid grid-cols-2 gap-4">
              <div className="bg-slate-100 p-5 rounded-2xl">
                <h4 className="text-3xl font-bold">15+</h4>
                <p className="text-slate-600">Years Experience</p>
              </div>

              <div className="bg-slate-100 p-5 rounded-2xl">
                <h4 className="text-3xl font-bold">40+</h4>
                <p className="text-slate-600">Countries Served</p>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Contact Section */}
      <section id="contact" className="max-w-6xl mx-auto px-6 py-20">
        <div className="bg-slate-900 rounded-3xl p-10 text-white grid md:grid-cols-2 gap-10">
          <div>
            <h3 className="text-4xl font-bold mb-4">Contact Us</h3>
            <p className="text-slate-300 mb-8">
              Reach out to our sales and support team for quotations, partnerships, or product inquiries.
            </p>

            <div className="space-y-4 text-slate-300">
              <p>Email: sales@chemcore.com</p>
              <p>Phone: +60 12-345-6789</p>
              <p>Location: Kajang, Malaysia</p>
            </div>
          </div>

          <form className="space-y-4">
            <input
              type="text"
              placeholder="Your Name"
              className="w-full p-4 rounded-2xl bg-slate-800 border border-slate-700 outline-none"
            />

            <input
              type="email"
              placeholder="Your Email"
              className="w-full p-4 rounded-2xl bg-slate-800 border border-slate-700 outline-none"
            />

            <textarea
              rows="5"
              placeholder="Your Message"
              className="w-full p-4 rounded-2xl bg-slate-800 border border-slate-700 outline-none"
            ></textarea>

            <button className="bg-cyan-500 hover:bg-cyan-400 px-6 py-3 rounded-2xl font-semibold transition">
              Send Message
            </button>
          </form>
        </div>
      </section>

      {/* Customer Support Chat Box */}
      <div className="fixed bottom-6 right-6 w-80 bg-white rounded-3xl shadow-2xl overflow-hidden border border-slate-200">
        <div className="bg-cyan-600 text-white px-5 py-4 flex items-center justify-between">
          <div>
            <h4 className="font-bold">Live Support</h4>
            <p className="text-xs opacity-90">We usually reply instantly</p>
          </div>

          <div className="h-3 w-3 bg-green-400 rounded-full"></div>
        </div>

        <div className="p-4 h-64 overflow-y-auto bg-slate-50 space-y-3 text-sm">
          <div className="bg-slate-200 p-3 rounded-2xl w-fit max-w-[80%]">
            Hello 👋 Welcome to ChemCore support. How can we help you today?
          </div>

          <div className="bg-cyan-500 text-white p-3 rounded-2xl ml-auto w-fit max-w-[80%]">
            I want a quotation for bulk methanol supply.
          </div>

          <div className="bg-slate-200 p-3 rounded-2xl w-fit max-w-[80%]">
            Sure. Please provide the required quantity and destination port.
          </div>
        </div>

        <div className="p-3 border-t border-slate-200 flex gap-2">
          <input
            type="text"
            placeholder="Type a message..."
            className="flex-1 border border-slate-300 rounded-2xl px-4 py-2 outline-none"
          />

          <button className="bg-cyan-500 text-white px-4 rounded-2xl hover:bg-cyan-400 transition">
            Send
          </button>
        </div>
      </div>

      {/* Footer */}
      <footer className="bg-slate-950 text-slate-400 py-8 text-center text-sm mt-10">
        © 2026 ChemCore Industrial Supplies. All rights reserved.
      </footer>
    </div>
  );
}# My-site.html
