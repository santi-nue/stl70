# BlazorWASMwGithubPages
This is a template of a Blazor WebAssembly project with Github Actions to deploy the Blazor WASM site to Github Pages

You can access the page here: [https://reusabletemplates.github.io/BlazorWASMwGithubPages](https://santi-nue.github.io/stl70)

## Steps to reproduce

1. Create a repository
2. Create a `gh-pages` branch from master (or whatever you call it, I call it root)
3. Clone the repository and create your Blazor project
4. Add NuGet library `PublishSPAforGitHubPages.Build`
5. Add GitHub Action, you can take mine ;-) Remember to adjust these places for your project:
  - `run: dotnet publish {{relative path to your sln file}} -c:Release -o:publish -p:GHPages=true`

## Specific NuGet packages used
- [Publish SPA for GitHub Pages - MSBuild Task & Scripts (designed for Blazor WebAssembly)](https://www.nuget.org/packages/PublishSPAforGitHubPages.Build)

## References
- [How to deploy ASP.NET Blazor WebAssembly to GitHub Pages](https://dev.to/swimburger/how-to-deploy-asp-net-blazor-webassembly-to-github-pages-44o)
- [The easier way to publish your Blazor WebAssembly app for GitHub Pages](https://dev.to/j_sakamoto/the-easier-way-to-publish-your-blazor-webassembly-app-for-github-pages-319l)
