1. Download Termux app
  
2. In Termux run:
```
apt update && apt upgrade && pkg update && pkg upgrade
```
```
pkg install nodejs
```
```
mkdir nextjs-project && cd nextjs-project && npx create-next-app@latest
```
3. Download Acode app
4. Select ```NEXTJS-PROJECT``` file from Termux
4. Open ```package.json```
5. delete line 6 and paste:

```
"dev": "NEXT_NO_TURBO=1 next dev",
```
7. Go back to termux and run:

```
npm run dev
```
8. Open any browser and type:
```localhost:3000```
