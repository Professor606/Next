# How to Set Up a Next.js Project on Termux  

## 1. Download and Install Termux  
First, download the **Termux** app from the Play Store or F-Droid.  

## 2. Update and Install Node.js  
Open Termux and run the following commands one by one:  
```sh
apt update && apt upgrade && pkg update && pkg upgrade
pkg install nodejs
```

## 3. Create a Next.js Project  
Run the following command to create a new Next.js project:  
```sh
mkdir nextjs-project && cd nextjs-project && npx create-next-app@latest
```

## 4. Download and Install Acode  
Download the **Acode** app from the Play Store to edit your Next.js files easily.  

## 5. Open Your Next.js Project in Acode  
In Acode, open your Next.js project folder (created in Termux).  

## 6. Modify `package.json`  
- Locate and open the `package.json` file.  
- On line 6, replace the `"dev"` script with the following:  
  ```json
  "dev": "NEXT_NO_TURBO=1 next dev",
  ```

## 7. Start the Development Server  
Go back to Termux and run:  
```sh
npm run dev
```

## 8. Access Your Site  
- Open any browser on your phone and enter:  
  ```
  localhost:3000
  ```
  
## 9. Access the Site from Another Device  
If you want to access your Next.js site from another device on the same network:  
- Find the local IP address of the device running the Next.js server (**Device A**).  
- On another device (**Device B**), open a browser and enter:  
  ```
  (Device A's local IP address):3000
  ```
  
Now, you can access your Next.js site from any device on the same network!
