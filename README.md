# The steps to connect to GitHub using SSH

## 1. Generate an SSH key

First, you need to generate an SSH key. Open your terminal or command prompt and execute the following command:

```terminal
ssh-keygen -t ed25519 -C "your_email@example.com"
```

Note: If you already have an SSH key, you can skip this step.

## 2. Copy the public key to the clipboard

Copy the public key to your clipboard by executing the following command:

- Linux/macOS:

```terminal
cat ~/.ssh/id_ed25519.pub | pbcopy
```

- Windows (Git Bash):

```terminal
cat ~/.ssh/id_ed25519.pub | clip
```

## 3. Add the public key to GitHub

Access your GitHub account settings and add the SSH key.

- Log in to GitHub, click on your avatar in the top right corner, and select "Settings."
- From the left menu, select "SSH and GPG keys."
- Click the "New SSH key" button.
- Enter a descriptive title and paste the public key from your clipboard into the key field, then click "Add SSH key."

## 4. Test the SSH connection

Run the following command to test if the SSH connection to GitHub is working correctly:

```terminal
ssh -T git@github.com
```

On the first connection, you will be asked whether to accept the GitHub host key. Type "yes" and press Enter.

If the connection is successful, you should see a message like this:

```terminal
Hi username! You've successfully authenticated, but GitHub does not provide shell access.
```

Now you can securely connect to GitHub using SSH when cloning, pushing, and pulling repositories.
# github_flow
# github_flow
