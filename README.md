- 👋 Hi, I’m @RizalKurniawan538
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
RizalKurniawan538/RizalKurniawan538 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
// Octokit.js
// https://github.com/octokit/core.js#readme
const octokit = new Octokit({
  auth: 'YOUR-TOKEN'
})

await octokit.request('GET /repos/{owner}/{repo}/dependency-graph/compare/{basehead}', {
  owner: 'OWNER',
  repo: 'REPO',
  basehead: 'BASEHEAD',
  headers: {
    'X-GitHub-Api-Version': '2022-11-28'
  }
})
