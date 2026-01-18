# Create Your First Mobile App (Expo Router)

## Objective

The objective of this task is to create and run a first mobile application using the Expo Router template. This task focuses on scaffolding a React Native project, modifying the home screen, running the app on a physical device, and understanding the project reset process.

---

## Project Setup Steps

### Step 1: Navigate to Project Directory

I navigated to the parent project directory using the terminal:

```bash
cd prodev-mobile-setup
```

Then moved into the working directory:

```bash
cd prodev-mobile-app-0x00
```

---

### Step 2: Initialize Expo Project

I initialized a new Expo project using the latest Expo Router template:

```bash
npx create-expo-app@latest .
```

This command scaffolded a new React Native project with Expo Router and created the default project structure.

---

### Step 3: Modify the Home Screen

I opened the following file:

```text
app/(tabs)/index.tsx
```

I changed the default text:

```tsx
Welcome!
```

To:

```tsx
First App Created
```

This confirmed my ability to locate and modify files within the Expo Router structure.

---

### Step 4: Run and Test the Application

I started the Expo development server using:

```bash
npx expo start
```

* On Android, I scanned the QR code using the Expo Go app.
* On iOS, the QR code can be scanned using the Camera app.

The application ran successfully on a physical device, displaying the updated home screen text.

---

## Resetting the Project

### Reset Command

I ran the reset command:

```bash
npm run reset-project
```

During the reset process, I was prompted with the option to move existing files instead of deleting them.

I selected **Yes (Y)**, which moved the existing project files into an `app-example` directory.

---

### Observations from reset-project

* The existing application files were preserved inside the `app-example` folder.
* A fresh Expo Router project structure was recreated.
* The `app-example` directory now contains:

  * `app-example/app/(tabs)/index.tsx`
  * `app-example/constants/Colors.tsx`

This process helps retain reference files while resetting the project for a clean development state.

### Reset Project Observations (Windows)

During the reset process, the script attempted to move existing files into an `app-example` directory. However, a Windows permission (EPERM) error occurred while renaming the `app` folder.

This is a known Windows filesystem behavior when files are in use or restricted. The intended result of the reset process was still achieved by manually moving the project files into the `app-example` directory.

The reset process is therefore considered successful.


---

## Conclusion

I successfully scaffolded my first mobile application using Expo Router, modified the home screen, ran the app on a physical device using Expo Go, and reset the project while preserving the original template files for reference.
