# 3D-
 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
index e12f6cfdff2eca7d0a715487f755cb8bf7f0ddae..ecc065e59427133daf4c35c29d8a4912e15dfa86 100644
--- a/README.md
+++ b/README.md
@@ -47,25 +47,40 @@ In this exercise, you will:
 
 2. In the new tab, most of the prompts will automatically fill in for you.
    - For owner, choose your personal account or an organization to host the repository.
    - We recommend creating a public repository, as private repositories will [use Actions minutes](https://docs.github.chttps://github.com/Greg-Coraino/skills-introduction-to-github/billing/managing-billing-for-github-actions/about-billing-for-github-actions).
    - Scroll down and click the **Create repository** button at the bottom of the form.
 
 3. After your new repository is created, wait about 20 seconds for the exercise to be prepared and buttons updated. You will continue working from your copy of the exercise.
    - The **Copy Exercise** button will deactivate, changing to gray.
    - The **Start Exercise** button will activate, changing to green.
    - You will likely need to refresh the page.
 
 4. Click **Start Exercise**. Follow the step-by-step instructions and feedback will be provided as you progress.
 
    <a id="start-exercise" href="https://github.com/Greg-Coraino/skills-introduction-to-github/issues/1">
       <img src="https://img.shields.io/badge/🚀_Start_Exercise-008000" height="25pt"/>
    </a>
 
 > [!IMPORTANT]
 > The **Start Exercise** button will activate after copying the repository. You will probably need to refresh the page.
 
 ---
 
 Get help: [Post in our discussion board](https://github.com/orgs/skills/discussions/categories/introduction-to-github) &bull; [Review the GitHub status page](https://www.githubstatus.com/)
 
 &copy; 2024 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)
+
+## 手势驱动的 Three.js 粒子演示
+
+在浏览器中打开 `index.html` 即可体验：
+
+- 允许摄像头权限，双手张开/合拢可控制粒子群收缩与扩散。
+- 单手做 1/2/3 手势，粒子会分别排布成 **Hello**、**CSC**、**666**。
+
+### 如何本地运行
+
+1. 在项目根目录启动本地静态服务器（保持 `localhost` 作用域以便使用摄像头）。例如：
+   - 使用 Python 3：`python3 -m http.server 8080`
+   - 或使用 Node：先 `npm i -g http-server`，再运行 `http-server -p 8080`
+2. 打开浏览器访问 <http://localhost:8080>（或终端提示的端口），页面会加载 `index.html`。
+3. 允许浏览器的摄像头权限，然后在摄像头前做双手张合与 1/2/3 手势，即可触发粒子收缩/扩散与文字切换。
 
EOF
)
