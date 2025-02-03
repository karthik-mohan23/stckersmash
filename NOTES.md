Start the app

```bash
 npx expo start
```

Expo Router basics

- app directory: A special directory containing only routes and their layouts. Any files added to this directory become a screen inside our native app and a page on the web.
- Root layout: The app/\_layout.tsx file. It defines shared UI elements such as headers and tab bars so they are consistent between different routes.
- File name conventions: Index file names, such as index.tsx, match their parent directory and do not add a path segment. For example, the index.tsx file in the app directory matches / route.

## Navigation

## stack navigation

What is a Stack?

A stack navigator is the foundation for navigating between different screens in an app. On Android, a stacked route animates on top of the current screen. On iOS, a stacked route animates from the right. Expo Router provides a Stack component to create a navigation stack to add new routes.

bottom tab bar

not-found route

Expo Router uses a special +not-found.tsx file to handle this case.

(tabs) subdirectory
This special directory is used to group routes together and display them in a bottom tab bar.
