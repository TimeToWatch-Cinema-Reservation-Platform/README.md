# Front-End and Back-End Project Management Guide

This guide provides step-by-step instructions for creating and managing Front-End and Back-End projects, as well as tips for synchronizing the two.

## Front-End Project with Vite for Working with React

1. **Create a New Front-End Project with Vite**:
   
   ```bash
   npm create @vitejs/app timetowatch-front --template react
   ```

2. **Navigate to the Front-End Project Directory**:

   ```bash
   cd timetowatch-front
   ```

## Back-End Project with NestJS

1. **Create a New Back-End Project with NestJS**:

   ```bash
   npx @nestjs/cli new timetowatch-back
   ```

2. **Navigate to the Back-End Project Directory**:

   ```bash
   cd timetowatch-back
   ```

## Initialize a Git Repository

1. **Initialize a New Git Repository**:

   ```bash
   git init
   ```

## Add a Remote Repository

1. **Add a "front" Remote Repository for the Front-End Project**:

   ```bash
   git remote add front <link_to_your_front-end_repository>
   ```

2. **Add a "back" Remote Repository for the Back-End Project**:

   ```bash
   git remote add back <link_to_your_back-end_repository>
   ```

## Make Changes and Send Them

1. **Make Local Changes**: Make changes in your files.

2. **Add and Commit the Changes**:

   ```bash
   git add .
   git commit -m "Commit description"
   ```

3. **Send the Changes to the Remote Repository**:

   ```bash
   git push front main
   git push back main
   ```

## Synchronize Front-End and Back-End Projects

1. **To Update the Front-End with the Latest Changes from the Back-End**:

   ```bash
   cd path_to_your_front-end_project
   git remote add back <link_to_your_back-end_repository>
   git pull back main
   ```

2. **To Update the Back-End with the Latest Changes from the Front-End**:

   ```bash
   cd path_to_your_back-end_project
   git remote add front <link_to_your_front-end_repository>
   git pull front main
   ```
