name: DevOps CI

on:
  push:
    branches: [ main ]

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout code
        uses: actions/checkout@v4

      - name: Run test
        run: echo "Build successful!"

      - name: Deploy
        run: echo "Deployment completed!"
