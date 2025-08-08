# jamalawar.com
portfolio website
export default function Website() {
  const projects = [
    {
      title: "Waiting for Gouraud (feature mockumentary)",
      role: "Writer • Director • Producer",
      year: "2025–26",
      tags: ["Satire", "Mockumentary", "Lebanon", "Funding/Industry Critique"],
      blurb:
        "Feature-length satirical mockumentary probing funding politics and postcolonial narratives in Lebanese cinema. Teaser filming August 2025; principal photography planned for 2026.",
      link: "#",
    },
    {
      title: "Music Videos (select)",
      role: "Director • Editor • Colorist",
      year: "2018–2025",
      tags: ["Narrative", "Performance", "VFX-light"],
      blurb:
        "Concept-led videos balancing visual storytelling with strong performance direction and clean, client-friendly delivery pipelines (Premiere/Resolve).",
      link: "#",
    },
    {
      title: "Waiting for Gouraud — Teaser",
      role: "Director • Editor",
      year: "2025",
      tags: ["Proof of Concept", "Satire", "Hybrid"],
      blurb:
        "10-minute proof filmed at the Piccadilly Theatre (Hamra, Beirut). Ensemble chaos, meta-fiction, and dry humor with documentary texture.",
      link: "#",
    },
    {
      title: "Commissioned Work (ITV / The FA / Google Pixel)",
      role: "Camera • Editor",
      year: "2025",
      tags: ["Sports", "Broadcast", "Branded"],
      blurb:
        "Pre- and post‑match analysis coverage for England Women vs Belgium (April 2025). Fast-turnaround capture and delivery to broadcast specs.",
      link: "#",
    },
  ];

  const clients = [
    "ITV",
    "The FA (England Football Association)",
    "Google Pixel",
    "Solo Films",
    "University for the Creative Arts (UCA)",
    "Independent artists, charities & cultural orgs",
  ];

  const services = [
    {
      title: "Directing & Creative Development",
      desc: "Narrative shorts, features, and music videos with satirical edge and strong performance direction.",
    },
    {
      title: "Editing & Post",
      desc: "Premiere Pro and DaVinci Resolve (conform, grade, broadcast delivery). Efficient, reliable pipelines.",
    },
    {
      title: "Research & Academic Partnerships",
      desc: "Practice-based film research, postcolonial theory, Lebanese cinema; talks, essays, and consults.",
    },
    {
      title: "Production Services",
      desc: "Teaser/proof-of-concept builds, festival deliverables, press kits, and pitch materials.",
    },
  ];

  const publications = [
    {
      outlet: "PhD (Film by Practice), UCA",
      item:
        "Research on Lebanese cinema’s funding structures and the civil war narrative; practice output: mockumentary feature *Waiting for Gouraud*.",
    },
    {
      outlet: "Talks & Panels",
      item:
        "Postcolonial cinema, co‑production treaties, and satire as critical practice (Lebanon/UK).",
    },
  ];

  return (
    <div className="min-h-screen bg-neutral-50 text-neutral-900">
      {/* Header / Nav */}
      <header className="sticky top-0 z-40 backdrop-blur supports-[backdrop-filter]:bg-white/60 bg-white/80 border-b border-neutral-200">
        <div className="max-w-6xl mx-auto px-4 py-4 flex items-center justify-between">
          <a href="#home" className="font-semibold tracking-tight flex items-center gap-3">
            <div className="w-8 h-8 rounded-2xl bg-neutral-900 text-white grid place-items-center text-sm">JA</div>
            <span>Jamal Awar <span className="text-neutral-400">/ جمال الأعور</span></span>
          </a>
          <nav className="hidden md:flex gap-6 text-sm">
            <a href="#work" className="hover:opacity-70">Work</a>
            <a href="#research" className="hover:opacity-70">Research</a>
            <a href="#services" className="hover:opacity-70">Services</a>
            <a href="#about" className="hover:opacity-70">About</a>
            <a href="#contact" className="hover:opacity-70">Contact</a>
          </nav>
          <a href="#contact" className="md:inline-flex hidden px-3 py-2 rounded-xl bg-neutral-900 text-white text-sm">Hire me</a>
        </div>
      </header>

      {/* Hero */}
      <section id="home" className="max-w-6xl mx-auto px-4 pt-16 pb-10">
        <div className="grid md:grid-cols-12 gap-8 items-center">
          <div className="md:col-span-7 space-y-6">
            <h1 className="text-4xl md:text-6xl font-semibold leading-tight">
              Lebanese filmmaker, editor, and researcher based in London.
            </h1>
            <p className="text-neutral-700 text-lg md:text-xl max-w-2xl">
              I make satirical, formally playful films and music videos—while building clear, dependable workflows for clients. Currently completing a PhD in Film by Practice at UCA, researching how funding shapes Lebanese cinema’s obsession with the civil war.
            </p>
            <div className="flex flex-wrap gap-3">
              <a href="#work" className="px-4 py-2 rounded-xl bg-neutral-900 text-white text-sm">See work</a>
              <a href="#research" className="px-4 py-2 rounded-xl border border-neutral-300 text-sm">Read research</a>
              <a href="#contact" className="px-4 py-2 rounded-xl border border-neutral-300 text-sm">Book a project</a>
            </div>
            <div className="flex gap-6 text-sm text-neutral-500 pt-2">
              <span>DaVinci Resolve • Premiere Pro • Color • Avid-familiar</span>
            </div>
          </div>
          <div className="md:col-span-5">
            <div className="aspect-[4/5] rounded-2xl bg-neutral-200 overflow-hidden"></div>
            <p className="text-xs text-neutral-500 mt-2">(Drop a portrait or showreel still here.)</p>
          </div>
        </div>
      </section>

      {/* Work */}
      <section id="work" className="max-w-6xl mx-auto px-4 py-12">
        <div className="flex items-end justify-between">
          <h2 className="text-2xl md:text-3xl font-semibold">Selected Work</h2>
          <a href="#contact" className="text-sm underline">Request full filmography</a>
        </div>
        <div className="grid md:grid-cols-2 gap-6 mt-8">
          {projects.map((p, idx) => (
            <article key={idx} className="rounded-2xl border border-neutral-200 overflow-hidden bg-white">
              <div className="aspect-video bg-neutral-200"></div>
              <div className="p-5 space-y-2">
                <div className="flex items-center justify-between">
                  <h3 className="font-medium text-lg">{p.title}</h3>
                  <span className="text-xs text-neutral-500">{p.year}</span>
                </div>
                <p className="text-sm text-neutral-600">{p.role}</p>
                <p className="text-sm text-neutral-700">{p.blurb}</p>
                <div className="flex flex-wrap gap-2 pt-2">
                  {p.tags.map((t, i) => (
                    <span key={i} className="text-xs px-2 py-1 rounded-full bg-neutral-100 border border-neutral-200">{t}</span>
                  ))}
                </div>
                <div className="pt-3">
                  <a href={p.link} className="text-sm underline">Watch / Learn more</a>
                </div>
              </div>
            </article>
          ))}
        </div>
      </section>

      {/* Research */}
      <section id="research" className="max-w-6xl mx-auto px-4 py-12">
        <h2 className="text-2xl md:text-3xl font-semibold">Research & Writing</h2>
        <p className="text-neutral-700 mt-4 max-w-3xl">
          Practice-based PhD (Film by Practice) at the University for the Creative Arts. My work interrogates how foreign co‑production, especially French public funds, shapes Lebanese film narratives around the civil war—often rewarding trauma aesthetics while narrowing what gets financed. *Waiting for Gouraud* is both a critique and a contribution: a film that participates in, and exposes, the system making it.
        </p>
        <div className="grid md:grid-cols-2 gap-6 mt-6">
          {publications.map((pub, i) => (
            <div key={i} className="rounded-2xl border border-neutral-200 bg-white p-5">
              <div className="text-sm text-neutral-500">{pub.outlet}</div>
              <div className="mt-1">{pub.item}</div>
            </div>
          ))}
        </div>
        <div className="mt-4">
          <a href="#contact" className="text-sm underline">Invite to speak • Request writing sample</a>
        </div>
      </section>

      {/* Services & Clients */}
      <section id="services" className="max-w-6xl mx-auto px-4 py-12">
        <div className="grid md:grid-cols-12 gap-8">
          <div className="md:col-span-7">
            <h2 className="text-2xl md:text-3xl font-semibold">Services</h2>
            <div className="grid sm:grid-cols-2 gap-4 mt-6">
              {services.map((s, i) => (
                <div key={i} className="rounded-2xl border border-neutral-200 bg-white p-5">
                  <div className="font-medium">{s.title}</div>
                  <p className="text-sm text-neutral-700 mt-1">{s.desc}</p>
                </div>
              ))}
            </div>
          </div>
          <div className="md:col-span-5">
            <h3 className="text-xl font-medium">Selected Clients</h3>
            <ul className="mt-4 space-y-2 text-sm text-neutral-700">
              {clients.map((c, i) => (
                <li key={i} className="flex items-center gap-2">
                  <span className="w-1.5 h-1.5 rounded-full bg-neutral-400 inline-block" />
                  {c}
                </li>
              ))}
            </ul>
            <div className="mt-4">
              <a href="#contact" className="text-sm underline">References available on request</a>
            </div>
          </div>
        </div>
      </section>

      {/* About */}
      <section id="about" className="max-w-6xl mx-auto px-4 py-12">
        <h2 className="text-2xl md:text-3xl font-semibold">About</h2>
        <div className="grid md:grid-cols-12 gap-8 mt-6">
          <div className="md:col-span-7 space-y-4">
            <p className="text-neutral-700">
              I’m a Lebanese filmmaker, video editor, and researcher based in London. I act, direct, write, and produce. From 2010–2017 I worked as an actor; since 2017 I’ve expanded into directing, writing, producing, and post. My practice focuses on satire, hybrid forms, and the politics of representation.
            </p>
            <p className="text-neutral-700">
              Current feature *Waiting for Gouraud* began in 2022 within my PhD and continues into production. Cast includes Saleh Bakri; producers include Abla Khoury, Reine Issa, and Samira Koujok. Soft equipment support secured via Solo Films. Shot language: Arabic (with some French/English).
            </p>
          </div>
          <div className="md:col-span-5">
            <div className="rounded-2xl border border-neutral-200 p-5 bg-white">
              <div className="font-medium">Quick Facts</div>
              <ul className="mt-3 space-y-2 text-sm text-neutral-700">
                <li>Base: London • Works in UK/Lebanon</li>
                <li>Editing & grade in DaVinci Resolve / Premiere Pro</li>
                <li>Languages: Arabic, English, French</li>
                <li>Academic focus: postcolonial theory, Third Cinema, co‑production treaties</li>
                <li>UCA PhD (Film by Practice)</li>
              </ul>
            </div>
          </div>
        </div>
      </section>

      {/* Contact */}
      <section id="contact" className="max-w-6xl mx-auto px-4 py-12">
        <div className="rounded-2xl border border-neutral-200 bg-white p-6">
          <h2 className="text-2xl md:text-3xl font-semibold">Work with me</h2>
          <p className="text-neutral-700 mt-2 max-w-3xl">
            For commissions, collaborations, or research requests, send a message with scope, timeline, and budget. I’m open to commercial, cultural, and academic work that values clarity and craft.
          </p>
          <div className="grid md:grid-cols-3 gap-4 mt-6 text-sm">
            <a href="mailto:hello@jamalawar.com" className="block p-4 rounded-xl border border-neutral-200 hover:bg-neutral-50">hello@jamalawar.com</a>
            <a href="https://vimeo.com/" target="_blank" className="block p-4 rounded-xl border border-neutral-200 hover:bg-neutral-50">Vimeo / Showreel</a>
            <a href="https://www.instagram.com/" target="_blank" className="block p-4 rounded-xl border border-neutral-200 hover:bg-neutral-50">Instagram</a>
          </div>
          <div className="mt-4 text-xs text-neutral-500">(Use your real email and links; these are placeholders.)</div>
        </div>
      </section>

      {/* Footer */}
      <footer className="max-w-6xl mx-auto px-4 pt-6 pb-20 text-sm text-neutral-500">
        <div className="flex flex-col md:flex-row items-center justify-between gap-2">
          <div>© {new Date().getFullYear()} Jamal Awar. All rights reserved.</div>
          <div className="flex gap-4">
            <a href="#" className="underline">Download CV (PDF)</a>
            <a href="#home" className="underline">Back to top</a>
          </div>
        </div>
      </footer>
    </div>
  );
}
