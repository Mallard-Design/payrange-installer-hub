<!-- The Giscus Board -->
<script src="https://giscus.app/client.js"
        data-repo="Mallard-Design/payrange-installer-hub"
        data-repo-id="R_kgDOTFfjZQ"
        data-category="Q&A"
        data-category-id="DIC_kwDOTFfjZc4DBr8Q"
        data-mapping="pathname"
        data-strict="0"
        data-reactions-enabled="1"
        data-emit-metadata="0"
        data-input-position="bottom"
        data-theme="light"
        data-lang="en"
        crossorigin="anonymous"
        async>
</script>

<!-- The Theme Sync Script -->
<script>
  var observer = new MutationObserver(function(mutations) {
    mutations.forEach(function(mutation) {
      if (mutation.attributeName === "data-md-color-scheme") {
        var isDark = document.body.getAttribute("data-md-color-scheme") === "slate";
        var theme = isDark ? "dark" : "light";
        var iframe = document.querySelector("iframe.giscus-frame");
        if (iframe) {
          iframe.contentWindow.postMessage({ giscus: { setConfig: { theme: theme } } }, "https://giscus.app");
        }
      }
    });
  });
  observer.observe(document.body, { attributes: true });
</script>