# ratnakalashjewellers
jewellery website
npx create-next-app@latest rana-kalash
cd rana-kalash
npm install axios

"use client";
import Link from "next/link";

export default function Home() {
  return (
    <main className="min-h-screen bg-black text-white">

      {/* Navbar */}
      <header className="flex justify-between items-center px-8 py-6 border-b border-gray-800">
        <h1 className="text-2xl font-serif text-yellow-500">
          Rana Kalash
        </h1>

        <nav className="space-x-6 text-sm">
          <Link href="/shop">Shop</Link>
          <Link href="/cart">Cart</Link>
        </nav>
      </header>

      {/* Hero */}
      <section className="flex flex-col items-center justify-center text-center h-[80vh] px-6">
        <h2 className="text-5xl font-serif mb-6 text-yellow-500">
          Bridal & Fashion Jewellery
        </h2>
        <p className="text-gray-300 max-w-xl">
          Elevate every occasion with handcrafted luxury pieces.
        </p>

        <Link href="/shop">
          <button className="mt-8 bg-yellow-500 text-black px-8 py-3 font-semibold hover:scale-105 transition">
            Explore Collection
          </button>
        </Link>
      </section>

    </main>
  );
}
