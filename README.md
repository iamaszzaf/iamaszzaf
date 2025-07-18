```js

const portfolioData = {
  name: "Łukasz Majka",
  location: "Szczecin, Poland",
  website: "https://aszzaf.pl",
  github: "https://github.com/iamaszzaf",
  linkedin: "https://linkedin.com/in/majkalukasz07",
  stack: {
    frontend: ["TypeScript", "React.js", "Next.js", "Tailwind CSS"],
    backend: ["Node.js", "NestJS", "Laravel"],
    database: ["PostgreSQL", "MySQL", "Prisma"],
    devops: ["Docker", "Git", "CI/CD (GitHub Actions / GitLab CI)"],
    testing: ["Playwright", "Cypress"],
    other: ["GraphQL"],
  },
  experience: [
    { position: "Magazynier", company: "PDC Logistics", start: "11/2024", end: null },
    { position: "Stażysta ds. logistyki", company: "Grupa Muszkieterów", start: "09/2023", end: "08/2024" },
  ],
  certifications: [
    { name: "AI-102: Azure AI Engineer Associate", issuer: "Microsoft", validFrom: "07/2025", validTo: "07/2026" },
    { name: "AZ-900: Azure Fundamentals", issuer: "Microsoft", validFrom: "01/2025", validTo: null },
  ],
  projects: [
    {
      name: "Zeptra",
      description:
        "Zaawansowany system zarządzania magazynem, automatyzujący i optymalizujący kluczowe procesy magazynowe.",
    },
    {
      name: "CzyPunktualnie?",
      description:
        "Innowacyjna platforma do śledzenia komunikacji miejskiej w czasie rzeczywistym i poprawy punktualności.",
    },
  ],
};

export default portfolioData;

