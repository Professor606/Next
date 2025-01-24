1. Download termux app
2. apt update && apt upgrade && pkg update && pkg upgrade
3. pkg install nodejs
4. mkdir nextjs-project && cd nextjs-project && npx create-next-app@latest
5. Download Acode app
6. select NEXTJS-PROJECT file from termux
7. Open package.json
8. In line 6: "dev": "NEXT_NO_TURBO=1 next dev",
9. Go back to termux and run: npm run dev
10. Open any browser and type: localhost:3000
