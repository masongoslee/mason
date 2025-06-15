# mason
CS photography website 
// File: pages/index.js (Home Page)
import Link from 'next/link';

export default function Home() {
  return (
    <main className="min-h-screen bg-gray-100 text-center p-8">
      <h1 className="text-4xl font-bold mb-6">CS Photography</h1>
      <p className="mb-6">Capturing Cars, Wildlife, and Events</p>
      <nav className="space-x-4">
        <Link href="/portfolio">Portfolio</Link>
        <Link href="/pricing">Pricing</Link>
        <Link href="/about">About</Link>
        <Link href="/contact">Contact</Link>
        <Link href="/admin">Login</Link>
      </nav>
    </main>
  );
}

// File: pages/portfolio.js
export default function Portfolio() {
  return (
    <main className="p-8">
      <h2 className="text-2xl font-bold mb-4">Portfolio</h2>
      <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4">
        <div className="border p-4">Cars</div>
        <div className="border p-4">Wildlife</div>
        <div className="border p-4">Events</div>
      </div>
    </main>
  );
}

// File: pages/pricing.js
export default function Pricing() {
  return (
    <main className="p-8">
      <h2 className="text-2xl font-bold mb-4">Prices and Packages</h2>
      <img src="/images/packages.jpg" alt="Packages" className="mx-auto mb-8" />
      <img src="/images/prints.jpg" alt="Prints" className="mx-auto" />
    </main>
  );
}

// File: pages/about.js
export default function About() {
  return (
    <main className="p-8">
      <h2 className="text-2xl font-bold mb-4">About CS Photography</h2>
      <p>I’m a passionate photographer capturing moments through cars, wildlife, and live events. Let’s create something beautiful together.</p>
    </main>
  );
}

// File: pages/contact.js
export default function Contact() {
  return (
    <main className="p-8">
      <h2 className="text-2xl font-bold mb-4">Contact</h2>
      <form className="flex flex-col space-y-4 max-w-md mx-auto">
        <input type="text" placeholder="Name" className="border p-2" />
        <input type="email" placeholder="Email" className="border p-2" />
        <textarea placeholder="Message" className="border p-2"></textarea>
        <button type="submit" className="bg-black text-white p-2">Send</button>
      </form>
    </main>
  );
}

// File: pages/admin.js (Login page)
export default function AdminLogin() {
  return (
    <main className="p-8">
      <h2 className="text-2xl font-bold mb-4">Admin Login</h2>
      <form className="flex flex-col space-y-4 max-w-sm mx-auto">
        <input type="email" placeholder="Email" className="border p-2" />
        <input type="password" placeholder="Password" className="border p-2" />
        <button type="submit" className="bg-blue-600 text-white p-2">Login</button>
      </form>
    </main>
  );
}
