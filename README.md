# tressdos

## FEATURES
- Auto checkin
- Auto Ping
- Multi-threaded, multi-account

## Installation

1. Clone this repository

```bash
git clone https://github.com/0xDee-Coder/tressdoss.git
cd tressdoss
```
- set the ref_code in the .env file
```bash
nano .env
```
2. Install dependencies
```bash
npm install
```
3. Fill Data and Proxy (Optional)

```bash
nano proxy.txt
```
5. stores account information in the format: `email|password`
```bash
nano data.txt
```
5. Run Bot
```bash
node main
```
-----------------------------------------------------------------

6. If you're logging in with a third-party service (e.g., Google), you’ll need to manually retrieve the token (valid for 2 months):

6-1. Method 1: Open the website 
- → press F12 (Inspect) 
- → go to the Application tab 
- → then LocalStorage → find accessToken

6-2. Method 2: Open the website 
- → press F12 
- → go to the Console tab 
- → paste and run the following code:
(If pasting is not allowed, type allow pasting manually first, then paste again)
```
try {
  const token = localStorage.getItem('accessToken');
  console.log(token); 
} catch (error) {
  console.error(error);
}
```
- After retrieving the token, save it into the file tokens.txt.
```bash
nano tokens.txt
```

- Run the command node setup to set up the token.
```bash
node setup
```
- run node main.
```bash
node main
```


## Contributing

Feel free to fork this repository and submit pull requests for any improvements.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Disclaimer

This bot is for educational purposes only. Use it at your own risk. The developer is not responsible for any account-related issues or potential losses.
