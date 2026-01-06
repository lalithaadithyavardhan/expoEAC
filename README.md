# expo-cli


🔹 Step 1: Install EAS CLI (one time)

Open Terminal / Command Prompt in your project folder and run:

npm install -g eas-cli


Check installation:

eas --version

🔹 Step 2: Login to Expo
expo login


(Login with the same account you used earlier)

🔹 Step 3: Configure EAS (one time per project)

Inside your project directory:

eas build:configure


✔ This creates eas.json
✔ Choose Android when asked
✔ Select APK (not AAB)

🔹 Step 4: Build the APK

Now run:

eas build -p android --profile preview


What happens:

Expo uploads your latest updated code

Builds APK in the cloud

Takes 5–10 minutes



🔹 Step 5: Download the APK

After build finishes:

Terminal shows a download link

OR go to 👉 https://expo.dev/accounts
 → Projects → Builds

📥 Download the .apk file
📲 Install it on your phone

🎉 DONE!

Your new updated APK is ready.





🔁 EVERY TIME YOU CHANGE CODE

You only need one command again:

eas build -p android --profile preview


No QR, no reinstalling Expo Go.
