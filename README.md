# Roushan Kumar — ASP.NET Core MVC Portfolio

A professional portfolio built with ASP.NET Core MVC (.NET 8), plus a static `docs/` build for GitHub Pages.

## MVC project structure
- `Controllers/HomeController.cs` — prepares portfolio content
- `Models/PortfolioViewModel.cs` — strongly typed portfolio data
- `Views/Home/Index.cshtml` — main Razor view
- `Views/Shared/_Layout.cshtml` — layout/navigation/footer
- `wwwroot/css/site.css` — responsive styling
- `wwwroot/js/site.js` — navigation + reveal animation
- `wwwroot/images/profile-photo.jpeg` — profile image
- `wwwroot/files/Resume_RoushanKumar.docx` — downloadable resume

## Run locally
Install .NET 8 SDK, then run:

```bash
dotnet restore
dotnet run
```

Open the localhost URL printed in the terminal.

## Important: GitHub Pages and MVC
GitHub Pages can host only static files. It cannot execute ASP.NET Core/C# server-side MVC.

To keep the repository as a real MVC project **and** keep a live GitHub Pages portfolio, this project includes a static mirror in `/docs`.

### Publish the static mirror on GitHub Pages
1. Upload the full project to your GitHub repository.
2. Open `Settings` → `Pages`.
3. Under `Build and deployment`, choose `Deploy from a branch`.
4. Select branch `main` and folder `/docs`.
5. Save.

For repository `roushankumar3350/Roushan_Kumar_Portfolio`, the Pages URL remains:
`https://roushankumar3350.github.io/Roushan_Kumar_Portfolio/`

## Deploy the real MVC application
For the actual server-side MVC application, deploy the same GitHub repository to an ASP.NET Core host such as Azure App Service, a Windows/IIS server, or another .NET-compatible service.

## Notes
- The portfolio copy avoids artificial skill percentages and generic buzzwords.
- Project descriptions intentionally stay non-confidential and do not invent metrics.
- Update professional details in `Controllers/HomeController.cs` and contact details in `Models/PortfolioViewModel.cs`.

## Featured live project

Latest blockchain-based project: https://roushankumar3350-001-site1.ftempurl.com/
