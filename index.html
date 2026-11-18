import React, { useEffect, useState } from 'react';
import {
  Award,
  Briefcase,
  Check,
  Code2,
  Copy,
  Download,
  FileText,
  GraduationCap,
  Layers,
  Mail,
  MapPin,
  PenTool,
  Phone,
  Share2,
  Smartphone,
  Sparkles,
  UserCheck,
} from 'lucide-react';
import { CvViewer } from './components/CvViewer';
import { Navbar } from './components/Navbar';
import { PdfCanvasViewer } from './components/PdfCanvasViewer';
import { AI_TOOLS, ADOBE_TOOLS, UI_TOOLS } from './components/ToolIcons';
import {
  CERTIFICATIONS,
  EDUCATION,
  EXPERIENCE,
  EXPERTISE,
  HERO_METRICS,
  PROCESS_STEPS,
  PROFILE,
} from './data/portfolioData';

const HERO_PORTRAIT_IMAGE = '/assets/aistudio/a_plz_adjest_the_posit_8b896b15.jpg';
const LAPTOP_WORK_IMAGE = '/assets/aistudio/a_laptop_screen_also_s_667b9aa6.jpg';

function isCvRouteActive(): boolean {
  if (typeof window === 'undefined') return false;
  const params = new URLSearchParams(window.location.search);
  return (
    params.get('view') === 'cv' ||
    window.location.pathname === '/cv' ||
    window.location.hash === '#/cv' ||
    window.location.hash === '#cv'
  );
}

function getShareableOrigin(): string {
  if (typeof window === 'undefined') return '';
  return window.location.origin.replace('https://ais-dev-', 'https://ais-pre-');
}

export default function App() {
  const [showCv, setShowCv] = useState<boolean>(() => isCvRouteActive());
  const [heroImgFailed, setHeroImgFailed] = useState(false);
  const [aboutLaptopFailed, setAboutLaptopFailed] = useState(false);
  const [toast, setToast] = useState<string | null>(null);
  const [copiedPdf, setCopiedPdf] = useState(false);

  const [formName, setFormName] = useState('');
  const [formEmail, setFormEmail] = useState('');
  const [formDetails, setFormDetails] = useState('');
  const [formNote, setFormNote] = useState('');

  const shareableOrigin = getShareableOrigin();
  const shareablePdfCvUrl = `${shareableOrigin}${PROFILE.cvPublicPath}`;

  useEffect(() => {
    const handleRouteChange = () => {
      setShowCv(isCvRouteActive());
    };
    window.addEventListener('popstate', handleRouteChange);
    window.addEventListener('hashchange', handleRouteChange);
    return () => {
      window.removeEventListener('popstate', handleRouteChange);
      window.removeEventListener('hashchange', handleRouteChange);
    };
  }, []);

  const notify = (message: string) => {
    setToast(message);
    window.setTimeout(() => {
      setToast((current) => (current === message ? null : current));
    }, 3000);
  };

  const openCvView = () => {
    setShowCv(true);
    const url = new URL(window.location.href);
    url.searchParams.set('view', 'cv');
    window.history.pushState(null, '', url.toString());
    window.scrollTo({ top: 0, behavior: 'smooth' });
  };

  const closeCvView = () => {
    setShowCv(false);
    const url = new URL(window.location.href);
    url.searchParams.delete('view');
    if (url.pathname === '/cv') url.pathname = '/';
    if (url.hash === '#cv' || url.hash === '#/cv') url.hash = '';
    window.history.pushState(null, '', url.toString());
    window.scrollTo({ top: 0, behavior: 'smooth' });
  };

  const handleCopyPdfLink = async () => {
    try {
      await navigator.clipboard.writeText(shareablePdfCvUrl);
      setCopiedPdf(true);
      notify('Direct CV PDF link copied to clipboard.');
      window.setTimeout(() => setCopiedPdf(false), 2400);
    } catch {
      notify('Unable to copy automatically — please select and copy the URL.');
    }
  };

  const handleContactSubmit = (e: React.FormEvent) => {
    e.preventDefault();
    const subject = encodeURIComponent(`Project enquiry from ${formName}`);
    const body = encodeURIComponent(
      `${formDetails}\n\nReply to: ${formEmail}`
    );
    window.location.href = `mailto:${PROFILE.email}?subject=${subject}&body=${body}`;
    setFormNote('Opening your email app with your message ready to send.');
  };

  const renderExpertiseIcon = (icon: (typeof EXPERTISE)[number]['icon']) => {
    switch (icon) {
      case 'brand':
        return <Layers className="h-5 w-5" aria-hidden="true" />;
      case 'art':
        return <PenTool className="h-5 w-5" aria-hidden="true" />;
      case 'social':
        return <Smartphone className="h-5 w-5" aria-hidden="true" />;
      case 'ai':
        return <Sparkles className="h-5 w-5" aria-hidden="true" />;
      case 'profile':
        return <UserCheck className="h-5 w-5" aria-hidden="true" />;
    }
  };

  if (showCv) {
    return (
      <>
        <CvViewer onBack={closeCvView} onNotify={notify} />
        {toast && (
          <div
            role="status"
            className="fixed bottom-6 left-1/2 z-50 -translate-x-1/2 rounded-xl border border-[#35C5E5] bg-[#073344] px-5 py-3 text-sm font-medium text-white shadow-xl"
          >
            {toast}
          </div>
        )}
      </>
    );
  }

  return (
    <div id="top" className="min-h-screen bg-[#031D2B] text-white">
      <Navbar onOpenCv={openCvView} />

      {/* Hero Section */}
      <header className="relative overflow-hidden py-16 md:py-24">
        <div
          className="pointer-events-none absolute -top-32 -right-24 h-96 w-96 rounded-full bg-[#35C5E5]/15 blur-[100px]"
          aria-hidden="true"
        />
        <div
          className="pointer-events-none absolute -bottom-24 -left-20 h-72 w-72 rounded-full bg-[#35C5E5]/10 blur-[90px]"
          aria-hidden="true"
        />

        <div className="relative mx-auto max-w-[1160px] px-6">
          <div className="grid items-stretch gap-12 lg:grid-cols-12">
            <div className="flex flex-col justify-center lg:col-span-7">
              <p className="mb-4 text-sm font-semibold tracking-wide text-[#54D8F0]">
                {PROFILE.title} · Lahore, Pakistan
              </p>
              <h1 className="text-4xl font-bold leading-[1.08] tracking-tight text-white sm:text-5xl lg:text-[3.25rem]">
                {PROFILE.headlineTop}
                <br />
                {PROFILE.headlineMid}{' '}
                <span className="text-[#35C5E5]">{PROFILE.headlineAccent}</span>
              </h1>
              <p className="mt-6 max-w-[58ch] text-base leading-relaxed text-[#A9BAC5] sm:text-lg">
                {PROFILE.subheadline}
              </p>

              <div className="mt-8 flex flex-wrap items-center gap-4">
                <button
                  type="button"
                  onClick={openCvView}
                  className="inline-flex items-center gap-2 rounded-full bg-[#35C5E5] px-7 py-3.5 text-sm font-semibold text-[#031D2B] whitespace-nowrap transition-all duration-200 hover:bg-[#54D8F0] hover:shadow-[0_0_28px_rgba(84,216,240,0.45)] cursor-pointer"
                >
                  <FileText className="h-4 w-4" aria-hidden="true" />
                  <span>See My CV</span>
                </button>
                <a
                  href="#contact"
                  className="inline-flex items-center gap-2 rounded-full border border-[#35C5E5] px-7 py-3.5 text-sm font-semibold text-[#35C5E5] whitespace-nowrap transition-all duration-200 hover:bg-[#35C5E5]/10 hover:text-[#54D8F0]"
                >
                  <span>Let’s Collaborate</span>
                </a>
              </div>
            </div>

            {/* Right Visual Container */}
            <div className="relative flex items-center justify-center lg:col-span-5">
              <div className="relative w-full max-w-[380px]">
                <div className="relative aspect-[1160/1664] w-full overflow-hidden rounded-3xl border border-[#23677C] bg-gradient-to-br from-[#073344] to-[#062B3A] shadow-[0_24px_60px_rgba(3,29,43,0.65)]">
                  {!heroImgFailed ? (
                    <img
                      src={HERO_PORTRAIT_IMAGE}
                      alt="Hafsa Khaliq, Senior Graphic and Brand Designer"
                      referrerPolicy="no-referrer"
                      onError={() => setHeroImgFailed(true)}
                      className="h-full w-full object-cover object-top"
                    />
                  ) : (
                    <div className="flex h-full w-full flex-col items-center justify-center p-8 text-center">
                      <PenTool className="h-12 w-12 text-[#35C5E5]" aria-hidden="true" />
                      <p className="mt-4 text-lg font-semibold text-white">
                        Brand Identity &amp; UI Systems
                      </p>
                      <p className="mt-1 text-sm text-[#A9BAC5]">{PROFILE.name}</p>
                    </div>
                  )}
                  <div
                    className="pointer-events-none absolute inset-0 bg-gradient-to-t from-[#031D2B]/40 via-transparent to-transparent"
                    aria-hidden="true"
                  />
                </div>

                {/* Signature Tool Chips: Figma, Adobe Photoshop, Claude AI */}
                <div
                  title="Figma"
                  className="animate-float-slow pointer-events-none absolute -top-3 -left-2 flex h-14 w-14 items-center justify-center rounded-2xl border border-[#35C5E5]/70 bg-[#073344]/95 shadow-[0_0_24px_rgba(53,197,229,0.28)] sm:-top-4 sm:-left-5"
                  aria-hidden="true"
                >
                  {UI_TOOLS[0].icon}
                </div>
                <div
                  title="Adobe Photoshop"
                  className="animate-float-slow pointer-events-none absolute top-1/2 -right-2 flex h-14 w-14 -translate-y-1/2 items-center justify-center rounded-2xl border border-[#35C5E5]/70 bg-[#073344]/95 shadow-[0_0_24px_rgba(53,197,229,0.28)] sm:-right-5"
                  style={{ animationDelay: '-2s' }}
                  aria-hidden="true"
                >
                  {ADOBE_TOOLS[0].icon}
                </div>
                <div
                  title="Claude AI"
                  className="animate-float-slow pointer-events-none absolute -bottom-3 left-5 flex h-14 w-14 items-center justify-center rounded-2xl border border-[#35C5E5]/70 bg-[#073344]/95 shadow-[0_0_24px_rgba(53,197,229,0.28)] sm:-bottom-4 sm:left-8"
                  style={{ animationDelay: '-4s' }}
                  aria-hidden="true"
                >
                  {AI_TOOLS[2].icon}
                </div>
              </div>
            </div>
          </div>

          {/* Full-width Metrics Strip below Hero Split */}
          <div className="mt-12 grid grid-cols-2 gap-6 border-t border-[#23677C]/60 pt-8 md:grid-cols-4">
            {HERO_METRICS.map((metric) => (
              <div key={metric.label}>
                <p className="text-3xl font-bold tracking-tight text-[#35C5E5] tabular-nums sm:text-4xl">
                  {metric.value}
                </p>
                <p className="mt-1 text-sm text-[#A9BAC5]">{metric.label}</p>
              </div>
            ))}
          </div>
        </div>
      </header>

      {/* About & Laptop Section */}
      <section id="about" className="bg-[#062B3A] py-20 md:py-24">
        <div className="mx-auto grid max-w-[1160px] items-center gap-12 px-6 lg:grid-cols-12">
          <div className="lg:col-span-6">
            <div className="aspect-[3/2] overflow-hidden rounded-3xl border border-[#23677C] bg-[#073344] shadow-[0_20px_50px_rgba(3,29,43,0.45)]">
              {!aboutLaptopFailed ? (
                <img
                  src={LAPTOP_WORK_IMAGE}
                  alt="Hafsa Khaliq working on brand colors and UI wireframes on her laptop"
                  referrerPolicy="no-referrer"
                  onError={() => setAboutLaptopFailed(true)}
                  className="h-full w-full object-cover object-center"
                />
              ) : (
                <div className="flex h-full w-full flex-col items-center justify-center p-8 text-center">
                  <Layers className="h-10 w-10 text-[#35C5E5]" aria-hidden="true" />
                  <p className="mt-3 text-base font-semibold text-white">
                    Brand &amp; UI Design Studio
                  </p>
                </div>
              )}
            </div>
          </div>

          <div className="flex flex-col justify-center lg:col-span-6">
            <h2 className="text-3xl font-bold tracking-tight text-white sm:text-4xl">
              More Than Design. It’s{' '}
              <span className="text-[#35C5E5]">Creative Thinking.</span>
            </h2>
            <p className="mt-6 max-w-[62ch] text-base leading-relaxed text-[#A9BAC5]">
              {PROFILE.aboutBio1}
            </p>
            <p className="mt-4 max-w-[62ch] text-base leading-relaxed text-[#A9BAC5]">
              {PROFILE.aboutBio2}
            </p>
            <div className="mt-8 flex flex-wrap items-center gap-x-6 gap-y-2 border-t border-[#23677C]/60 pt-6 text-sm text-[#A9BAC5]">
              <span>{PROFILE.location}</span>
              <span aria-hidden="true">·</span>
              <span>50+ Clients</span>
              <span aria-hidden="true">·</span>
              <span>150+ Projects Delivered</span>
            </div>
          </div>
        </div>
      </section>

      {/* Education & Qualifications */}
      <section id="education" className="py-20 md:py-24">
        <div className="mx-auto max-w-[1160px] px-6">
          <div className="mb-12">
            <h2 className="text-3xl font-bold tracking-tight text-white sm:text-4xl">
              Education &amp; <span className="text-[#35C5E5]">Qualifications.</span>
            </h2>
          </div>

          <div className="grid gap-6 md:grid-cols-2">
            {EDUCATION.map((edu, index) => (
              <div
                key={edu.degree}
                className="rounded-2xl border border-[#23677C] bg-[#073344] p-7 transition-colors duration-200 hover:border-[#35C5E5]"
              >
                <div className="mb-5 flex h-12 w-12 items-center justify-center rounded-xl border border-[#35C5E5] text-[#35C5E5]">
                  {index === 0 ? (
                    <Code2 className="h-5 w-5" aria-hidden="true" />
                  ) : (
                    <GraduationCap className="h-5 w-5" aria-hidden="true" />
                  )}
                </div>
                <h3 className="text-xl font-bold text-white">{edu.degree}</h3>
                <p className="mt-1 text-base font-medium text-[#A9BAC5]">
                  {edu.institution}
                </p>
                <p className="mt-4 text-sm text-[#A9BAC5] tabular-nums">
                  {edu.period}
                  {edu.status && (
                    <>
                      {' '}
                      <span aria-hidden="true">·</span>{' '}
                      <span className="font-medium text-[#54D8F0]">{edu.status}</span>
                    </>
                  )}
                </p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Work Experience */}
      <section id="experience" className="bg-[#062B3A] py-20 md:py-24">
        <div className="mx-auto max-w-[1160px] px-6">
          <div className="mb-12 flex flex-wrap items-end justify-between gap-6">
            <div>
              <h2 className="text-3xl font-bold tracking-tight text-white sm:text-4xl">
                Work <span className="text-[#35C5E5]">Experience.</span>
              </h2>
              <p className="mt-3 max-w-[56ch] text-base text-[#A9BAC5]">
                Hands-on brand identity, marketing design, and Figma UI/UX experience across agencies
                and product teams.
              </p>
            </div>
            <button
              type="button"
              onClick={openCvView}
              className="inline-flex items-center gap-2 rounded-full border border-[#35C5E5] px-5 py-2.5 text-sm font-semibold text-[#35C5E5] whitespace-nowrap transition-colors hover:bg-[#35C5E5]/10 hover:text-[#54D8F0] cursor-pointer"
            >
              <FileText className="h-4 w-4" aria-hidden="true" />
              <span>See Full CV</span>
            </button>
          </div>

          <div className="grid gap-6 lg:grid-cols-3">
            {EXPERIENCE.map((job) => (
              <div
                key={`${job.company}-${job.period}`}
                className="flex flex-col rounded-2xl border border-[#23677C] bg-[#073344] p-7 transition-colors duration-200 hover:border-[#35C5E5]"
              >
                <div className="mb-5 flex h-12 w-12 items-center justify-center rounded-xl border border-[#35C5E5] text-[#35C5E5]">
                  <Briefcase className="h-5 w-5" aria-hidden="true" />
                </div>
                <h3 className="text-xl font-bold text-white">{job.role}</h3>
                <p className="mt-1 text-base font-medium text-white/90">
                  {job.company} · {job.location}
                </p>
                <p className="mt-2 text-sm text-[#A9BAC5] tabular-nums">
                  {job.period}
                  {job.isCurrent && (
                    <>
                      {' '}
                      <span aria-hidden="true">·</span>{' '}
                      <span className="font-medium text-[#54D8F0]">Current role</span>
                    </>
                  )}
                </p>
                <p className="mt-4 text-sm leading-relaxed text-[#A9BAC5]">
                  {job.summary}
                </p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Expertise */}
      <section id="expertise" className="py-20 md:py-24">
        <div className="mx-auto max-w-[1160px] px-6">
          <div className="mb-12">
            <h2 className="text-3xl font-bold tracking-tight text-white sm:text-4xl">
              What I Bring to <span className="text-[#35C5E5]">Every Project.</span>
            </h2>
          </div>

          <div className="grid gap-5 md:grid-cols-2 lg:grid-cols-4">
            {EXPERTISE.map((item) => (
              <div
                key={item.title}
                className={`rounded-2xl border border-[#23677C] bg-[#073344] p-7 transition-colors duration-200 hover:border-[#35C5E5] ${
                  item.wide ? 'md:col-span-2 lg:col-span-4 flex flex-col sm:flex-row sm:items-center gap-6' : ''
                }`}
              >
                <div
                  className={`flex h-12 w-12 shrink-0 items-center justify-center rounded-xl border border-[#35C5E5] text-[#35C5E5] ${
                    item.wide ? '' : 'mb-5'
                  }`}
                >
                  {renderExpertiseIcon(item.icon)}
                </div>
                <div>
                  <h3 className="text-lg font-bold text-white">{item.title}</h3>
                  <p className="mt-2 max-w-[68ch] text-sm leading-relaxed text-[#A9BAC5]">
                    {item.description}
                  </p>
                </div>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Process */}
      <section id="process" className="bg-[#062B3A] py-20 md:py-24">
        <div className="mx-auto max-w-[1160px] px-6">
          <div className="mb-12">
            <h2 className="text-3xl font-bold tracking-tight text-white sm:text-4xl">
              From Concept <span className="text-[#35C5E5]">to Creation.</span>
            </h2>
          </div>

          <div className="grid gap-6 md:grid-cols-3">
            {PROCESS_STEPS.map((step) => (
              <div
                key={step.number}
                className="rounded-2xl border border-[#35C5E5]/70 bg-[#031D2B]/40 p-7"
              >
                <p className="text-4xl font-bold text-[#35C5E5] tabular-nums">
                  {step.number}
                </p>
                <h3 className="mt-3 text-xl font-bold text-white">{step.title}</h3>
                <p className="mt-2 text-sm leading-relaxed text-[#A9BAC5]">
                  {step.description}
                </p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Creative Arsenal / Tools */}
      <section id="tools" className="py-20 md:py-24">
        <div className="mx-auto max-w-[1160px] px-6">
          <div className="mb-12">
            <h2 className="text-3xl font-bold tracking-tight text-white sm:text-4xl">
              My Creative <span className="text-[#35C5E5]">Arsenal.</span>
            </h2>
          </div>

          <div className="space-y-8">
            <div>
              <h3 className="mb-4 text-sm font-semibold text-[#A9BAC5]">
                Adobe Creative Cloud
              </h3>
              <div className="flex flex-wrap gap-3">
                {ADOBE_TOOLS.map((tool) => (
                  <div
                    key={tool.id}
                    className="flex items-center gap-3 rounded-xl border border-[#23677C] bg-[#073344] py-2.5 pr-4 pl-2.5 text-sm font-medium text-white transition-colors hover:border-[#35C5E5]"
                  >
                    {tool.icon}
                    <span>{tool.name}</span>
                  </div>
                ))}
              </div>
            </div>

            <div>
              <h3 className="mb-4 text-sm font-semibold text-[#A9BAC5]">
                UI/UX &amp; Vector Design
              </h3>
              <div className="flex flex-wrap gap-3">
                {UI_TOOLS.map((tool) => (
                  <div
                    key={tool.id}
                    className="flex items-center gap-3 rounded-xl border border-[#23677C] bg-[#073344] py-2.5 pr-4 pl-2.5 text-sm font-medium text-white transition-colors hover:border-[#35C5E5]"
                  >
                    {tool.icon}
                    <span>{tool.name}</span>
                  </div>
                ))}
              </div>
            </div>

            <div>
              <h3 className="mb-4 text-sm font-semibold text-[#A9BAC5]">
                AI-Assisted Workflow Tools
              </h3>
              <div className="flex flex-wrap gap-3">
                {AI_TOOLS.map((tool) => (
                  <div
                    key={tool.id}
                    className="flex items-center gap-3 rounded-xl border border-[#23677C] bg-[#073344] py-2.5 pr-4 pl-2.5 text-sm font-medium text-white transition-colors hover:border-[#35C5E5]"
                  >
                    {tool.icon}
                    <span>{tool.name}</span>
                  </div>
                ))}
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Certifications & Recognition (Verified from CV) */}
      <section id="recognition" className="bg-[#062B3A] py-20 md:py-24">
        <div className="mx-auto max-w-[1160px] px-6">
          <div className="mb-12">
            <h2 className="text-3xl font-bold tracking-tight text-white sm:text-4xl">
              Certifications &amp; <span className="text-[#35C5E5]">Recognition.</span>
            </h2>
          </div>

          <div className="grid gap-5 md:grid-cols-2 lg:grid-cols-3">
            {CERTIFICATIONS.map((cert) => (
              <div
                key={cert.title}
                className="rounded-2xl border border-[#23677C] bg-[#073344] p-6 transition-colors duration-200 hover:border-[#35C5E5]"
              >
                <div className="mb-4 flex h-10 w-10 items-center justify-center rounded-xl border border-[#35C5E5]/70 text-[#35C5E5]">
                  <Award className="h-5 w-5" aria-hidden="true" />
                </div>
                <h3 className="text-base font-bold text-white">{cert.title}</h3>
                <p className="mt-1 text-xs font-medium text-[#54D8F0]">
                  {cert.issuer} · {cert.date}
                </p>
                <p className="mt-3 text-sm leading-relaxed text-[#A9BAC5]">
                  {cert.description}
                </p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Curriculum Vitae Live Preview Section */}
      <section id="cv-preview" className="py-20 md:py-24">
        <div className="mx-auto max-w-[1160px] px-6">
          <div className="mb-10 flex flex-wrap items-end justify-between gap-6">
            <div>
              <h2 className="text-3xl font-bold tracking-tight text-white sm:text-4xl">
                Curriculum <span className="text-[#35C5E5]">Vitae.</span>
              </h2>
              <p className="mt-3 max-w-[58ch] text-base text-[#A9BAC5]">
                Preview my complete CV directly below, open all 3 pages in full screen, or copy a
                shareable link for your profiles.
              </p>
            </div>
            <div className="flex flex-wrap items-center gap-3">
              <button
                type="button"
                onClick={openCvView}
                className="inline-flex items-center gap-2 rounded-full bg-[#35C5E5] px-6 py-3 text-sm font-semibold text-[#031D2B] whitespace-nowrap transition-colors hover:bg-[#54D8F0] cursor-pointer"
              >
                <FileText className="h-4 w-4" aria-hidden="true" />
                <span>Open Full CV (3 Pages)</span>
              </button>
              <a
                href={PROFILE.cvFilePath}
                download={PROFILE.cvDownloadName}
                className="inline-flex items-center gap-2 rounded-full border border-[#35C5E5] px-5 py-3 text-sm font-semibold text-[#35C5E5] whitespace-nowrap transition-colors hover:bg-[#35C5E5]/10 hover:text-[#54D8F0]"
              >
                <Download className="h-4 w-4" aria-hidden="true" />
                <span>Download PDF</span>
              </a>
            </div>
          </div>

          <div className="grid items-start gap-8 lg:grid-cols-12">
            <div className="lg:col-span-7">
              <PdfCanvasViewer
                fileUrl={PROFILE.cvFilePath}
                maxPages={1}
                compact
                onFallbackRequested={openCvView}
              />
            </div>

            <div className="space-y-5 rounded-2xl border border-[#23677C] bg-[#073344] p-7 lg:col-span-5">
              <h3 className="text-xl font-bold text-white">
                Complete 3-Page CV Ready to View &amp; Share
              </h3>
              <p className="text-sm leading-relaxed text-[#A9BAC5]">
                Includes my full work experience at PRG Pakistan, Ibuildsoft LLC, and Acme Filing
                Limited LLC, education, eco-friendly packaging project, certifications, and software
                skills.
              </p>

              <div className="space-y-3 border-t border-[#23677C]/60 pt-5">
                <button
                  type="button"
                  onClick={openCvView}
                  className="flex w-full items-center justify-center gap-2 rounded-full bg-[#35C5E5] px-5 py-3 text-sm font-semibold text-[#031D2B] transition-colors hover:bg-[#54D8F0] cursor-pointer"
                >
                  <FileText className="h-4 w-4" aria-hidden="true" />
                  <span>See My CV (All 3 Pages)</span>
                </button>
                <button
                  type="button"
                  onClick={handleCopyPdfLink}
                  className="flex w-full items-center justify-center gap-2 rounded-full border border-[#23677C] bg-[#031D2B]/70 px-5 py-3 text-sm font-medium text-white transition-colors hover:border-[#35C5E5] cursor-pointer"
                >
                  {copiedPdf ? (
                    <Check className="h-4 w-4 text-[#35C5E5]" aria-hidden="true" />
                  ) : (
                    <Share2 className="h-4 w-4 text-[#35C5E5]" aria-hidden="true" />
                  )}
                  <span>
                    {copiedPdf ? 'CV PDF Link Copied!' : 'Copy CV PDF Link'}
                  </span>
                </button>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Contact & Shareable CV Links Section */}
      <section id="contact" className="bg-[#062B3A] py-20 md:py-24">
        <div className="mx-auto grid max-w-[1160px] gap-12 px-6 lg:grid-cols-12">
          <div className="lg:col-span-6">
            <h2 className="text-3xl font-bold tracking-tight text-white sm:text-4xl">
              Have an Idea?{' '}
              <span className="text-[#35C5E5]">
                Let’s Create Something Extraordinary.
              </span>
            </h2>
            <p className="mt-5 max-w-[52ch] text-base leading-relaxed text-[#A9BAC5]">
              Looking for a creative partner to shape your brand identity, marketing visuals, or
              UI experience? Reach out directly or inspect my full CV below.
            </p>

            <div className="mt-7 space-y-3 text-sm text-[#A9BAC5]">
              <a
                href={`mailto:${PROFILE.email}`}
                className="flex items-center gap-3 text-[#54D8F0] hover:underline"
              >
                <Mail className="h-4 w-4 shrink-0" aria-hidden="true" />
                <span>{PROFILE.email}</span>
              </a>
              <a
                href={`tel:${PROFILE.phone.replace(/\s+/g, '')}`}
                className="flex items-center gap-3 tabular-nums hover:text-white"
              >
                <Phone className="h-4 w-4 shrink-0 text-[#35C5E5]" aria-hidden="true" />
                <span>{PROFILE.phone}</span>
              </a>
              <p className="flex items-center gap-3">
                <MapPin className="h-4 w-4 shrink-0 text-[#35C5E5]" aria-hidden="true" />
                <span>{PROFILE.location}</span>
              </p>
            </div>

            {/* Shareable CV Link Card for Professional Profiles */}
            <div className="mt-8 rounded-2xl border border-[#23677C] bg-[#073344] p-5">
              <div className="flex flex-wrap items-center justify-between gap-3">
                <div>
                  <h3 className="text-sm font-bold text-white">
                    Shareable CV Link
                  </h3>
                  <p className="mt-0.5 text-xs text-[#A9BAC5]">
                    Copy your direct CV PDF link for LinkedIn, Behance, or job applications.
                  </p>
                </div>
                <button
                  type="button"
                  onClick={openCvView}
                  className="inline-flex items-center gap-1.5 rounded-full bg-[#35C5E5] px-4 py-1.5 text-xs font-semibold text-[#031D2B] whitespace-nowrap hover:bg-[#54D8F0] cursor-pointer"
                >
                  <FileText className="h-3.5 w-3.5" aria-hidden="true" />
                  <span>See My CV</span>
                </button>
              </div>

              <div className="mt-4">
                <div className="flex items-center justify-between gap-2 rounded-xl border border-[#23677C]/80 bg-[#031D2B]/70 px-3.5 py-2">
                  <div className="min-w-0">
                    <p className="text-[11px] font-semibold text-[#54D8F0]">
                      Direct CV PDF Link
                    </p>
                    <p className="truncate text-xs text-[#A9BAC5]">
                      {shareablePdfCvUrl}
                    </p>
                  </div>
                  <div className="flex items-center gap-1.5 shrink-0">
                    <button
                      type="button"
                      onClick={handleCopyPdfLink}
                      className="inline-flex items-center gap-1.5 rounded-lg border border-[#23677C] bg-[#073344] px-3 py-1.5 text-xs font-medium text-white whitespace-nowrap hover:border-[#35C5E5] cursor-pointer"
                    >
                      {copiedPdf ? (
                        <Check className="h-3.5 w-3.5 text-[#35C5E5]" />
                      ) : (
                        <Copy className="h-3.5 w-3.5 text-[#35C5E5]" />
                      )}
                      <span>{copiedPdf ? 'Copied' : 'Copy'}</span>
                    </button>
                    <a
                      href={PROFILE.cvFilePath}
                      download={PROFILE.cvDownloadName}
                      title="Download CV PDF"
                      className="inline-flex items-center justify-center rounded-lg border border-[#23677C] bg-[#073344] p-1.5 text-[#A9BAC5] hover:border-[#35C5E5] hover:text-white"
                    >
                      <Download className="h-3.5 w-3.5" aria-hidden="true" />
                    </a>
                  </div>
                </div>
              </div>
            </div>

            <div className="mt-7 flex flex-wrap gap-3">
              {PROFILE.socials.map((soc) => (
                <a
                  key={soc.label}
                  href={soc.href}
                  target="_blank"
                  rel="noopener noreferrer"
                  className="rounded-full border border-[#23677C] px-4 py-2 text-xs font-medium text-[#A9BAC5] transition-colors hover:border-[#35C5E5] hover:text-[#54D8F0]"
                >
                  {soc.label}
                </a>
              ))}
            </div>
          </div>

          <form
            onSubmit={handleContactSubmit}
            className="flex flex-col gap-4 rounded-2xl border border-[#23677C] bg-[#062B3A] p-7 lg:col-span-6"
          >
            <label className="grid gap-2 text-sm text-[#A9BAC5]">
              <span>Name</span>
              <input
                type="text"
                required
                autoComplete="name"
                value={formName}
                onChange={(e) => setFormName(e.target.value)}
                placeholder="Your full name"
                className="rounded-xl border border-[#23677C] bg-[#073344] px-4 py-3 text-sm text-white placeholder:text-[#A9BAC5]/50 focus:border-[#35C5E5] focus:outline-none"
              />
            </label>
            <label className="grid gap-2 text-sm text-[#A9BAC5]">
              <span>Email</span>
              <input
                type="email"
                required
                autoComplete="email"
                value={formEmail}
                onChange={(e) => setFormEmail(e.target.value)}
                placeholder="you@example.com"
                className="rounded-xl border border-[#23677C] bg-[#073344] px-4 py-3 text-sm text-white placeholder:text-[#A9BAC5]/50 focus:border-[#35C5E5] focus:outline-none"
              />
            </label>
            <label className="grid gap-2 text-sm text-[#A9BAC5]">
              <span>Project details</span>
              <textarea
                rows={5}
                required
                value={formDetails}
                onChange={(e) => setFormDetails(e.target.value)}
                placeholder="Tell me about your brand, project timeline, and design goals..."
                className="rounded-xl border border-[#23677C] bg-[#073344] px-4 py-3 text-sm text-white placeholder:text-[#A9BAC5]/50 focus:border-[#35C5E5] focus:outline-none"
              />
            </label>
            <button
              type="submit"
              className="mt-2 inline-flex items-center justify-center rounded-full bg-[#35C5E5] px-7 py-3.5 text-sm font-semibold text-[#031D2B] transition-all duration-200 hover:bg-[#54D8F0] cursor-pointer"
            >
              Send Message
            </button>
            {formNote && (
              <p role="status" className="text-xs font-medium text-[#54D8F0]">
                {formNote}
              </p>
            )}
          </form>
        </div>
      </section>

      {/* Footer */}
      <footer className="border-t border-[#23677C]/70 bg-[#031D2B] py-12">
        <div className="mx-auto max-w-[1160px] px-6">
          <div className="flex flex-wrap items-start justify-between gap-8">
            <div>
              <p className="text-base font-bold text-white">{PROFILE.name}</p>
              <p className="mt-1 max-w-sm text-sm text-[#A9BAC5]">
                {PROFILE.title} creating meaningful visual identities and digital experiences.
              </p>
            </div>

            <div className="flex flex-wrap items-center gap-6 text-sm text-[#A9BAC5]">
              <a href="#about" className="hover:text-[#54D8F0]">
                About
              </a>
              <a href="#experience" className="hover:text-[#54D8F0]">
                Experience
              </a>
              <a href="#expertise" className="hover:text-[#54D8F0]">
                Expertise
              </a>
              <a href="#tools" className="hover:text-[#54D8F0]">
                Tools
              </a>
              <button
                type="button"
                onClick={openCvView}
                className="font-medium text-[#54D8F0] hover:underline cursor-pointer"
              >
                See My CV
              </button>
              <a href="#contact" className="hover:text-[#54D8F0]">
                Contact
              </a>
              {PROFILE.socials.map((soc) => (
                <a
                  key={soc.label}
                  href={soc.href}
                  target="_blank"
                  rel="noopener noreferrer"
                  className="hover:text-[#54D8F0]"
                >
                  {soc.label}
                </a>
              ))}
            </div>
          </div>

          <div className="mt-8 border-t border-[#23677C]/50 pt-6 text-xs text-[#A9BAC5]">
            © 2026 {PROFILE.name}. All rights reserved.
          </div>
        </div>
      </footer>

      {toast && (
        <div
          role="status"
          className="fixed bottom-6 left-1/2 z-50 -translate-x-1/2 rounded-xl border border-[#35C5E5] bg-[#073344] px-5 py-3 text-sm font-medium text-white shadow-xl"
        >
          {toast}
        </div>
      )}
    </div>
  );
}
