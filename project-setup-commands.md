# Project Setup Commands for NextJS
## If you are tired of repeating the process of folder or file creation manually in NextJS, you can use these commands in your terminal to auto-generate them easily.
(Note: this is written for a generic project structure, change the commands as per your needs)


```
npx create-next-app@latest <project-name> --typescript --eslint --tailwind --app --import-alias "@/*" && cd <project-name>

mkdir -p app/{api/{auth,folder1, folder2,..},home,user/\[id\]} components lib
mkdir -p app/\(auth\)/{login,signup}

touch app/page.tsx \
      app/layout.tsx \
      app/\(auth\)/login/page.tsx \
      app/\(auth\)/signup/page.tsx \
      app/api/auth/\[...nextauth\].ts \
      app/api/folder1/route.ts \
      app/api/folder2/route.ts \
      app/home/page.tsx \
      app/user/\[id\]/page.tsx \
      components/{LoginForm,SignupForm,UserProfile}.tsx \
      lib/{db,auth}.ts
```
