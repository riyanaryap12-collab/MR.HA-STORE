import React from "react";

// Single-file React component (Tailwind CSS required in the host project) // Usage: import CatalogWebsite from './CatalogWebsite.jsx' and render <CatalogWebsite />

export default function CatalogWebsite() { const waNumber = "6285695895096"; // international format (no +) const waLink = https://wa.me/${waNumber}?text=${encodeURIComponent( 'Halo%20MR.HA%20STORE%20-%20Saya%20mau%20pesan%20Jokian%20Arena%20Breakout%20.%20Bisa%20bantu%3F' )};

return ( <div className="min-h-screen bg-gradient-to-b from-gray-900 to-gray-800 text-white font-sans"> <header className="max-w-5xl mx-auto p-6 flex items-center justify-between"> <div className="flex items-center gap-4"> <div className="w-16 h-16 bg-gradient-to-br from-indigo-500 to-pink-500 rounded-2xl flex items-center justify-center shadow-2xl"> <svg xmlns="http://www.w3.org/2000/svg" className="w-10 h-10" viewBox="0 0 24 24" fill="none" stroke="white" strokeWidth="1.5"> <path d="M3 3h18v18H3z" strokeLinecap="round" strokeLinejoin="round" /> </svg> </div> <div> <h1 className="text-2xl font-extrabold">MR.HA STORE</h1> <p className="text-sm text-gray-300">Jokian Arena Breakout — Top-up cepat & terpercaya</p> </div> </div> <a href={waLink} target="_blank" rel="noreferrer" className="inline-flex items-center gap-2 bg-green-500 hover:bg-green-600 text-gray-900 rounded-md px-4 py-2 font-semibold shadow"> <svg xmlns="http://www.w3.org/2000/svg" className="w-5 h-5" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2"> <path d="M21 2L11 13" strokeLinecap="round" strokeLinejoin="round" /> <path d="M21 2l-7 19-4-9-9-4 19-6z" strokeLinecap="round" strokeLinejoin="round" /> </svg> Order via WhatsApp </a> </header>

<main className="max-w-5xl mx-auto p-6 grid grid-cols-1 lg:grid-cols-3 gap-8">
    {/* Left: Hero + Benefits */}
    <section className="lg:col-span-2 bg-gradient-to-br from-gray-800/60 to-gray-700/40 rounded-2xl p-6 shadow-xl">
      <div className="flex flex-col lg:flex-row gap-6">
        <div className="flex-1">
          <h2 className="text-3xl font-bold">Catalog & Website — Jokian Arena Breakout</h2>
          <p className="mt-3 text-gray-300">Cepat, aman, dan harga bersaing. Pilih paket Koen atau Velue — kami siap proses instan. Tersedia juga bundling & promo khusus untuk pembelian banyak.</p>

          <ul className="mt-5 grid grid-cols-1 sm:grid-cols-2 gap-3">
            <li className="bg-gray-900/40 p-3 rounded-lg">⚡ Proses instan</li>
            <li className="bg-gray-900/40 p-3 rounded-lg">🔒 Aman & Terpercaya</li>
            <li className="bg-gray-900/40 p-3 rounded-lg">🎮 Support 24/7</li>
            <li className="bg-gray-900/40 p-3 rounded-lg">📱 Order via WhatsApp</li>
          </ul>

          <div className="mt-6 flex gap-3">
            <a href={waLink} target="_blank" rel="noreferrer" className="px-5 py-3 bg-indigo-600 rounded-lg font-semibold shadow hover:bg-indigo-700">Pesan Sekarang</a>
            <button onClick={() => window.print()} className="px-4 py-3 border border-gray-700 rounded-lg text-gray-200">Cetak Katalog</button>
          </div>
        </div>

        <div className="w-full lg:w-80 bg-gradient-to-br from-indigo-600/10 to-pink-600/8 rounded-2xl p-4 flex flex-col gap-4">
          <h3 className="text-xl font-bold">Highlight Promo</h3>
          <div className="p-3 bg-gray-900/30 rounded-lg">
            <h4 className="font-semibold">🔥 Paket Hemat</h4>
            <p className="text-sm text-gray-300">2M Koen + 1M Velue — Rp120.000 (hemat Rp15.000)</p>
          </div>

          <div className="p-3 bg-gray-900/30 rounded-lg">
            <h4 className="font-semibold">💎 Paket Sultan</h4>
            <p className="text-sm text-gray-300">5M Koen + 5M Velue — Rp360.000 (hemat Rp15.000)</p>
          </div>

          <div className="p-3 bg-gray-900/30 rounded-lg">
            <h4 className="font-semibold">⚡ Promo Spesial</h4>
            <p className="text-sm text-gray-300">Beli 10M Koen + Gratis 1M Velue</p>
          </div>

          <div className="p-3 bg-gray-900/30 rounded-lg">
            <h4 className="font-semibold">🎉 Bonus Member</h4>
            <p className="text-sm text-gray-300">Transaksi 3x, dapat potongan Rp20.000 di order berikutnya</p>
          </div>
        </div>
      </div>

      {/* Price table */}
      <div className="mt-8 bg-gray-900/20 p-4 rounded-xl">
        <h3 className="text-2xl font-bold mb-4">Price List</h3>
        <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
          <div className="p-4 bg-gradient-to-br from-indigo-700/40 to-indigo-600/20 rounded-lg">
            <h4 className="text-xl font-semibold">Koen</h4>
            <ul className="mt-3 text-gray-200 leading-relaxed">
              <li>1M = Rp45.000</li>
              <li>2M = Rp90.000</li>
              <li>5M = Rp225.000</li>
              <li>10M = Rp450.000</li>
            </ul>
          </div>

          <div className="p-4 bg-gradient-to-br from-pink-700/30 to-pink-600/15 rounded-lg">
            <h4 className="text-xl font-semibold">Velue</h4>
            <ul className="mt-3 text-gray-200 leading-relaxed">
              <li>1M = Rp30.000</li>
              <li>2M = Rp60.000</li>
              <li>5M = Rp150.000</li>
              <li>10M = Rp300.000</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    {/* Right column: Contact + Order form (simulated) */}
    <aside className="bg-gray-900/30 rounded-2xl p-6 shadow-xl">
      <h3 className="text-xl font-bold mb-3">Order Cepat</h3>

      <div className="mb-4">
        <label className="block text-sm text-gray-300">Nama</label>
        <input className="mt-1 w-full rounded-md bg-gray-800/50 p-2 outline-none" placeholder="Nama Anda" />
      </div>

      <div className="mb-4">
        <label className="block text-sm text-gray-300">Paket yang diinginkan</label>
        <select className="mt-1 w-full rounded-md bg-gray-800/50 p-2">
          <option>1M Koen (Rp45.000)</option>
          <option>1M Velue (Rp30.000)</option>
          <option>2M Koen + 1M Velue (Paket Hemat)</option>
          <option>5M Koen + 5M Velue (Paket Sultan)</option>
        </select>
      </div>

      <div className="mb-4">
        <label className="block text-sm text-gray-300">WhatsApp / No. HP</label>
        <input className="mt-1 w-full rounded-md bg-gray-800/50 p-2" placeholder="08xx..." />
      </div>

      <a href={waLink} target="_blank" rel="noreferrer" className="block text-center mt-4 px-4 py-3 bg-green-500 rounded-lg font-semibold text-gray-900">Kirim Pesan ke WhatsApp</a>

      <div className="mt-6 text-sm text-gray-300">
        <p>Untuk pesanan otomatis dan konfirmasi cepat, klik tombol WhatsApp. Nomor penjual: <strong>0856-9589-5096</strong>.</p>
      </div>
    </aside>
  </main>

  <footer className="max-w-5xl mx-auto p-6 text-center text-gray-400">© {new Date().getFullYear()} MR.HA STORE — Semua harga dapat berubah tanpa pemberitahuan. Hubungi via WA untuk ketersediaan & konfirmasi.</footer>
</div>

); }

