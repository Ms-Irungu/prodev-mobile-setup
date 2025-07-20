# Welcome to your Expo app 👋

This is an [Expo](https://expo.dev) project created with [`create-expo-app`](https://www.npmjs.com/package/create-expo-app).

## Get started

1. Install dependencies

   ```bash
   npm install
   ```

2. Start the app

   ```bash
   npx expo start
   ```

In the output, you'll find options to open the app in a

- [development build](https://docs.expo.dev/develop/development-builds/introduction/)
- [Android emulator](https://docs.expo.dev/workflow/android-studio-emulator/)
- [iOS simulator](https://docs.expo.dev/workflow/ios-simulator/)
- [Expo Go](https://expo.dev/go), a limited sandbox for trying out app development with Expo

You can start developing by editing the files inside the **app** directory. This project uses [file-based routing](https://docs.expo.dev/router/introduction).

## Get a fresh project

When you're ready, run:

```bash
npm run reset-project
```

This command will move the starter code to the **app-example** directory and create a blank **app** directory where you can start developing.

### Troubleshooting `npm run reset-project`

If you encounter a permission error like this when running `npm run reset-project`:

```bash
❌ Error during script execution: EPERM: operation not permitted, rename 'app' -> 'app-example\app'
```

**Cause:** This error occurs when the Expo development server is still running and has file locks on the `app` directory, preventing Windows from moving/renaming it.

**Solution:**

1. **Stop the Expo development server** by pressing `Ctrl+C` in any terminal where you ran `npx expo start`
2. **Close Expo Go app** if it's still connected to your development server
3. **Wait a few seconds** for all file locks to be released
4. **Re-run the command**: `npm run reset-project`

**Alternative Solution (if the above doesn't work):**

- Kill any remaining Node.js processes: `taskkill /F /IM node.exe`
- Then run `npm run reset-project` again

> **💡 Tip:** Always stop your development server before running project reset or file manipulation commands to avoid permission conflicts.

## Learn more

To learn more about developing your project with Expo, look at the following resources:

- [Expo documentation](https://docs.expo.dev/): Learn fundamentals, or go into advanced topics with our [guides](https://docs.expo.dev/guides).
- [Learn Expo tutorial](https://docs.expo.dev/tutorial/introduction/): Follow a step-by-step tutorial where you'll create a project that runs on Android, iOS, and the web.

## Join the community

Join our community of developers creating universal apps.

- [Expo on GitHub](https://github.com/expo/expo): View our open source platform and contribute.
- [Discord community](https://chat.expo.dev): Chat with Expo users and ask questions.
