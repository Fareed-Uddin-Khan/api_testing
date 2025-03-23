# 🧪 Postman API Test Automation Badge – Assignment Walkthrough

This repository contains my complete solution for the **Postman API Test Automation badge** challenge.  
It includes all 5 assignments, Postman test scripts, and a working GitHub Actions setup.

---

## 🏁 Badge Earned: [API Test Automation by Postman](https://badgr.com/public/assertions/k9-vD6LQRA2cQ_wVes2Wcg)

---

## 📁 Repo Structure

```
api_testing/
├── assignment_5.postman_collection.json     # Postman collection with all tests
└── .github/
    └── workflows/
        └── postman.yml                      # GitHub Actions workflow to run collection
```

---

## ✅ Steps I Followed to Earn the Badge

### 📝 Assignment 1–4 (Inside Postman)
- Wrote tests using `pm.test()` and `pm.expect()` to:
  - Check status codes
  - Parse response JSON
  - Validate response properties
  - Extract variables and reuse them
  - Write JSON schema tests with required fields + no extra props

---

### ⚙️ Assignment 5: GitHub Automation

1. **Created a public GitHub repo** (`api_testing`)
2. **Exported my Postman collection** as v2.1 format
3. **Added a GitHub Actions workflow** at `.github/workflows/postman.yml`
4. **Used the Postman CLI**, not Newman, to run the collection:
   ```yaml
   postman login --with-api-key "$POSTMAN_API_KEY"
   postman collection run "assignment_5.postman_collection.json"
   ```
5. **Created a GitHub secret**:
   - Go to `Settings > Secrets > Actions`
   - Name: `POSTMAN_API_KEY`
   - Value: (from Postman account > API keys)
6. **Updated the Postman variable** `githubProjectUrl` with my GitHub repo URL
7. **Committed everything** and ran the workflow

---

## 🌐 Key Links

- 🔗 [Badge on Badgr](https://badgr.com/public/assertions/k9-vD6LQRA2cQ_wVes2Wcg)
- 📘 [Postman Academy](https://academy.postman.com/)
- 📚 [Postman CLI Docs](https://learning.postman.com/docs/postman-cli/postman-cli-overview/)
- 🛠 [GitHub Actions Docs](https://docs.github.com/en/actions)

---

## 🙋‍♂️ Need Help?

If you're trying to earn the badge too and got stuck:
- Fork this repo
- Update your own workspace and GitHub Actions
- Open an issue or ping me on LinkedIn!

I’m happy to help others on the same learning journey.

---

## 🧠 Final Thoughts

This challenge gave me real-world exposure to:
- Writing dynamic API tests in Postman
- Using Postman CLI in CI/CD
- Structuring automated test pipelines
- Debugging API requests + workflows

Thanks to the Postman team for making this badge challenging, hands-on, and rewarding! 🧡

---

Made with 💻 by [Fareed-Uddin-Khan](https://github.com/Fareed-Uddin-Khan)
```

---

Let me know when you paste this in your repo — or if you want help customizing it further (e.g., screenshots or badges)!
