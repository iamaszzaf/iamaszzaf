```csharp

using System;
using System.Collections.Generic;

namespace PortfolioData
{
    public static class Data
    {
        public static Portfolio Portfolio = new Portfolio
        {
            Name = "Łukasz Majka",
            Description = "👋 Cześć! Jestem Łukasz – programista, który łączy wygląd i technologię w nowoczesnych aplikacjach.",
            Location = "Szczecin, Poland",
            Website = "https://aszzaf.pl",
            GitHub = "https://github.com/iamaszzaf",
            LinkedIn = "https://linkedin.com/in/majkalukasz07",
            Stack = new Stack
            {
                Frontend = new List<string> { "TypeScript", "React.js", "Next.js", "Tailwind CSS" },
                Backend = new List<string> { "Node.js", "NestJS", "Laravel" },
                Database = new List<string> { "PostgreSQL", "MySQL", "Prisma" },
                DevOps = new List<string> { "Docker", "Git", "CI/CD (GitHub Actions / GitLab CI)" },
                Testing = new List<string> { "Playwright", "Cypress" },
                Other = new List<string> { "GraphQL" }
            },
            Experience = new List<Experience>
            {
                new Experience { Position = "Magazynier", Company = "PDC Logistics", StartDate = "11/2024", EndDate = null },
                new Experience { Position = "Stażysta ds. logistyki", Company = "Grupa Muszkieterów", StartDate = "09/2023", EndDate = "08/2024" }
            },
            Certifications = new List<Certification>
            {
                new Certification { Name = "AI-102: Azure AI Engineer Associate", Issuer = "Microsoft", ValidFrom = "07/2025", ValidTo = "07/2026" },
                new Certification { Name = "AZ-900: Azure Fundamentals", Issuer = "Microsoft", ValidFrom = "01/2025", ValidTo = null }
            },
            Projects = new List<Project>
            {
                new Project { Name = "Zeptra", Description = "Zaawansowany system zarządzania magazynem, automatyzujący i optymalizujący kluczowe procesy magazynowe." },
                new Project { Name = "CzyPunktualnie?", Description = "Innowacyjna platforma do śledzenia komunikacji miejskiej w czasie rzeczywistym i poprawy punktualności." }
            }
        };
    }

    public class Portfolio
    {
        public string Name { get; set; }
        public string Description { get; set; }  // opis po imieniu z emoji
        public string Location { get; set; }
        public string Website { get; set; }
        public string GitHub { get; set; }
        public string LinkedIn { get; set; }
        public Stack Stack { get; set; }
        public List<Experience> Experience { get; set; }
        public List<Certification> Certifications { get; set; }
        public List<Project> Projects { get; set; }
    }

    public class Stack
    {
        public List<string> Frontend { get; set; }
        public List<string> Backend { get; set; }
        public List<string> Database { get; set; }
        public List<string> DevOps { get; set; }
        public List<string> Testing { get; set; }
        public List<string> Other { get; set; }
    }

    public class Experience
    {
        public string Position { get; set; }
        public string Company { get; set; }
        public string StartDate { get; set; }
        public string EndDate { get; set; }
    }

    public class Certification
    {
        public string Name { get; set; }
        public string Issuer { get; set; }
        public string ValidFrom { get; set; }
        public string ValidTo { get; set; }
    }

    public class Project
    {
        public string Name { get; set; }
        public string Description { get; set; }
    }
}
