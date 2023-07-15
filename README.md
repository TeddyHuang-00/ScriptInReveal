1. Init project

   ```sh
   pnpm create vuepress-theme-hope ScriptInReveal
   ```

2. Update dependencies

   ```sh
   pnpm docs:update-package
   ```

3. Insert html code block in [slides](./src/slides.md)

   ````md
   <!-- .slide: data-transition="slide" -->

   ## HTML 代码

   ```html
   <script>
     alert("Hello World!");
   </script>
   ```
   ````

   And this will lead to an unexpected termination of the slides at the `</script>` tag. Check through `pnpm docs:dev`

4. (For comparison) Insert the same code block as above in [intro](./src/intro.md), and it works fine.
