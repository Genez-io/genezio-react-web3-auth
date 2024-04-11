# Genezio Web3 Wallet Authentication Example

This repository demonstrates the integration of Genezio, a framework for building serverless applications, with Web3 wallet authentication to secure access to your application's functionalities.

# Run

1. Install genezio.

```
npm install genezio -g
```

2. Deploy the project. If you are not logged in, you will be redirected to login or register with a genezio account.

```
genezio deploy
```

3. Go to your project on the genezio dashboard and active the Authentication for your project from the "Authentication" section. 
4. Activate the Web 3 Auth provider and after that copy the `Token` and `Region` values. Paste them in `client/src/App.tsx`:

```typescript
// Add your own values here
AuthService.getInstance().setTokenAndRegion("<token>", "<region>");
```

4. Deploy again the client

```
genezio deploy --frontend
```
