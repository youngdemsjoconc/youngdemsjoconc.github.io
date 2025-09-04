import React, { useMemo, useState } from "react";

// --- YDJC Onboarding Web App (single-file React component) ---
// How to use:
// 1) Replace the placeholder links (JOIN_FORM_URL, DONATE_URL, EVENTS_CAL_URL) with real links.
//    - JOIN_FORM_URL: a Google Form, Airtable form, or EveryAction/NGP form.
//    - DONATE_URL: your ActBlue / Donorbox / contribution link.
//    - EVENTS_CAL_URL: a public Google Calendar (embed) or MobilizeAmerica feed.
// 2) Deploy this as a static app on Vercel/Netlify/GitHub Pages.
// 3) Print the QR from the “Share” menu and put it on flyers, tables, and name badges.

export default function YDJCApp() {
  // === CONFIG: update these three URLs ===
  const JOIN_FORM_URL = "https://www.mobilize.us/ncdems/event/610672/"; // TODO: replace with your live form
  const DONATE_URL = "https://secure.actblue.com/donate/youngdemsjoco"; // TODO: replace with ActBlue or similar
  const EVENTS_CAL_URL = "https://calendar.google.com/calendar/embed?src=N2MyYzc0YTE5ZTFkNjA1MjM2YjMwY2NhYzMyNWExMDVlYjJlOTIzYTMyNDkxNWM3MDMyZDJlZTAyMzM3MzU0NkBncm91cC5jYWxlbmRhci5nb29nbGUuY29t&ctz=America%2FNew_York"; // TODO: replace with public Google Calendar embed URL

  // Optional: fallback events list if you don't have a calendar yet
  const seedEvents = [
    {
      title: "Monthly Meeting",
      date: "Thu, Oct 10, 7–8:30 PM",
      where: "Clayton Community Center",
      url: "#",
    },
    {
      title: "Canvass Launch",
      date: "Sat, Oct 19, 10 AM",
      where: "Smithfield HQ",
      url: "#",
    },
    {
      title: "Phones & Pizza",
      date: "Wed, Oct 23, 6–8 PM",
      where: "Zoom (RSVP)",
      url: "#",
    },
  ];

  const [showQR, setShowQR] = useState(false);
  const [tab, setTab] = useState("home");

  // Build a QR that points to this app's public URL; replace with your deployed URL once live
  const appUrl = typeof window !== "undefined" ? window.location.href : "https://ydjc.example.org";
  const qrSrc = useMemo(() => {
    const encoded = encodeURIComponent(appUrl);
    // Using a public QR service; you can swap for any preferred generator
    return `https://api.qrserver.com/v1/create-qr-code/?size=512x512&data=${encoded}`;
  }, [appUrl]);

  const NavButton = ({ id, label, icon }) => (
    <button
      onClick={() => setTab(id)}
      className={`px-4 py-2 rounded-xl text-sm md:text-base transition hover:shadow ${
        tab === id ? "bg-slate-900 text-white" : "bg-white text-slate-900 border"
      }`}
    >
      <span className="inline-flex items-center gap-2">
        <span aria-hidden>{icon}</span>
        {label}
      </span>
    </button>
  );

  const Card = ({ children }) => (
    <div className="bg-white rounded-2xl shadow p-5 md:p-6 border">
      {children}
    </div>
  );

  return (
    <div className="min-h-screen bg-slate-50 text-slate-900">
      {/* Header */}
      <header className="sticky top-0 z-10 backdrop-blur bg-white/80 border-b">
        <div className="max-w-5xl mx-auto px-4 py-3 flex items-center justify-between gap-4">
          <div className="flex items-center gap-3">
            <div className="w-10 h-10 rounded-xl bg-slate-900 text-white grid place-items-center font-bold">Y</div>
            <div>
              <h1 className="text-lg md:text-xl font-semibold">Young Democrats of Johnston County</h1>
              <p className="text-xs md:text-sm text-slate-600">Connect • Volunteer • Vote</p>
            </div>
          </div>

          <div className="flex items-center gap-2">
            <button
              onClick={() => setShowQR(true)}
              className="hidden sm:inline-flex items-center gap-2 px-4 py-2 rounded-xl border bg-white hover:shadow"
            >
              <span aria-hidden>📱</span> Share / QR
            </button>
            <a
              href={DONATE_URL}
              target="_blank"
              rel="noreferrer"
              className="inline-flex items-center gap-2 px-4 py-2 rounded-xl bg-emerald-600 text-white hover:shadow"
            >
              <span aria-hidden>💚</span> Donate
            </a>
          </div>
        </div>
      </header>

      {/* Nav */}
      <nav className="max-w-5xl mx-auto px-4 mt-5">
        <div className="flex flex-wrap gap-2">
          <NavButton id="home" label="Home" icon="🏠" />
          <NavButton id="join" label="Join" icon="📝" />
          <NavButton id="events" label="Events" icon="📅" />
          <NavButton id="donate" label="Donate" icon="💳" />
          <NavButton id="about" label="About" icon="ℹ️" />
        </div>
      </nav>

      {/* Main */}
      <main className="max-w-5xl mx-auto px-4 py-6 grid gap-6">
        {tab === "home" && (
          <div className="grid md:grid-cols-3 gap-6">
            <Card>
              <h2 className="text-lg font-semibold">New here?</h2>
              <p className="text-sm text-slate-600 mt-1">Become a member in under two minutes.</p>
              <a
                href={JOIN_FORM_URL}
                target="_blank"
                rel="noreferrer"
                className="mt-4 inline-flex items-center gap-2 px-4 py-2 rounded-xl bg-slate-900 text-white hover:shadow"
              >
                Join now →
              </a>
            </Card>

            <Card>
              <h2 className="text-lg font-semibold">Support the work</h2>
              <p className="text-sm text-slate-600 mt-1">Chip in to help register voters & train organizers.</p>
              <a
                href={DONATE_URL}
                target="_blank"
                rel="noreferrer"
                className="mt-4 inline-flex items-center gap-2 px-4 py-2 rounded-xl bg-emerald-600 text-white hover:shadow"
              >
                Donate →
              </a>
            </Card>

            <Card>
              <h2 className="text-lg font-semibold">Upcoming events</h2>
              <ul className="mt-3 space-y-2">
                {seedEvents.map((e, i) => (
                  <li key={i} className="text-sm">
                    <div className="font-medium">{e.title}</div>
                    <div className="text-slate-600">{e.date} • {e.where}</div>
                  </li>
                ))}
              </ul>
              <button
                onClick={() => setTab("events")}
                className="mt-4 inline-flex items-center gap-2 px-4 py-2 rounded-xl border bg-white hover:shadow"
              >
                See all events →
              </button>
            </Card>
          </div>
        )}

        {tab === "join" && (
          <Card>
            <h2 className="text-xl font-semibold">Join YDJC</h2>
            <p className="text-sm text-slate-600 mt-1">
              Tap the button below to open our membership form. After you submit, you’ll get a confirmation
              email with next steps and ways to plug in.
            </p>
            <a
              href={JOIN_FORM_URL}
              target="_blank"
              rel="noreferrer"
              className="mt-4 inline-flex items-center gap-2 px-4 py-2 rounded-xl bg-slate-900 text-white hover:shadow"
            >
              Open membership form →
            </a>
            <div className="mt-6 text-xs text-slate-500">
              Admin tip: Use a Google Form/Airtable form with fields for name, email, phone, zip, interests, volunteer availability.
            </div>
          </Card>
        )}

        {tab === "events" && (
          <div className="grid lg:grid-cols-2 gap-6">
            <Card>
              <h2 className="text-xl font-semibold">Events Calendar</h2>
              <p className="text-sm text-slate-600 mt-1">If you see a blank area, make sure your Google Calendar embed URL is public.</p>
              <div className="mt-4 aspect-video w-full overflow-hidden rounded-xl border bg-white">
                <iframe
                  title="Events"
                  src={EVENTS_CAL_URL}
                  className="w-full h-full"
                />
              </div>
            </Card>
            <Card>
              <h2 className="text-xl font-semibold">Quick RSVP Links</h2>
              <ul className="mt-2 list-disc list-inside text-sm space-y-1">
                {seedEvents.map((e, i) => (
                  <li key={i}>
                    <a href={e.url} className="underline decoration-slate-400 hover:decoration-slate-900">
                      {e.title}
                    </a>
                    <span className="text-slate-600"> — {e.date} • {e.where}</span>
                  </li>
                ))}
              </ul>
            </Card>
          </div>
        )}

        {tab === "donate" && (
          <Card>
            <h2 className="text-xl font-semibold">Donate</h2>
            <p className="text-sm text-slate-600 mt-1">Every dollar helps us organize and elect Democrats locally.</p>
            <a
              href={DONATE_URL}
              target="_blank"
              rel="noreferrer"
              className="mt-4 inline-flex items-center gap-2 px-4 py-2 rounded-xl bg-emerald-600 text-white hover:shadow"
            >
              Give now →
            </a>
            <div className="mt-6 text-xs text-slate-500">
              Admin tip: Use ActBlue or Donorbox, and enable Apple/Google Pay for 1-tap giving.
            </div>
          </Card>
        )}

        {tab === "about" && (
          <Card>
            <h2 className="text-xl font-semibold">About YDJC</h2>
            <p className="text-sm text-slate-600 mt-1">
              We’re young people building power in Johnston County through voter registration, leadership
              development, and community service.
            </p>
            <div className="mt-4 grid sm:grid-cols-2 gap-4 text-sm">
              <div className="p-4 rounded-xl bg-slate-100">
                <div className="font-medium">Contact</div>
                <div className="text-slate-700">Email: info@ydjohnston.org</div>
                <div className="text-slate-700">Instagram: @ydjohnston</div>
              </div>
              <div className="p-4 rounded-xl bg-slate-100">
                <div className="font-medium">Meetings</div>
                <div className="text-slate-700">2nd Thursdays, 7 PM</div>
                <div className="text-slate-700">Clayton Community Center</div>
              </div>
            </div>
          </Card>
        )}
      </main>

      {/* Footer */}
      <footer className="border-t">
        <div className="max-w-5xl mx-auto px-4 py-6 text-xs text-slate-500 flex flex-wrap items-center justify-between gap-2">
          <div>Paid for by Young Democrats of Johnston County</div>
          <div className="flex items-center gap-2">
            <button
              onClick={() => setShowQR(true)}
              className="inline-flex items-center gap-2 px-3 py-1.5 rounded-lg border bg-white hover:shadow"
            >
              <span aria-hidden>🔗</span> Share this app
            </button>
            <button
              onClick={() => {
                if (navigator.share) {
                  navigator.share({ title: "YDJC Onboarding", url: appUrl });
                } else {
                  navigator.clipboard.writeText(appUrl);
                  alert("Link copied to clipboard!");
                }
              }}
              className="inline-flex items-center gap-2 px-3 py-1.5 rounded-lg border bg-white hover:shadow"
            >
              Copy link
            </button>
          </div>
        </div>
      </footer>

      {/* QR Modal */}
      {showQR && (
        <div className="fixed inset-0 bg-black/50 grid place-items-center p-4" onClick={() => setShowQR(false)}>
          <div className="bg-white rounded-2xl shadow-xl max-w-md w-full p-6 relative" onClick={(e) => e.stopPropagation()}>
            <button
              onClick={() => setShowQR(false)}
              className="absolute right-3 top-3 w-8 h-8 rounded-full border grid place-items-center"
              aria-label="Close"
            >
              ✕
            </button>
            <h3 className="text-lg font-semibold">Scan to open</h3>
            <p className="text-sm text-slate-600">Point your camera at the QR to open this app.</p>
            <img src={qrSrc} alt="QR code" className="mt-4 w-full rounded-xl border" />
            <div className="mt-4 text-xs text-slate-500">Tip: Tap-and-hold to save the QR to your Photos, then drop it into flyers or slides.</div>
          </div>
        </div>
      )}
    </div>
  );
}
