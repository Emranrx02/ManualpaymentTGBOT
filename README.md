🚀 Telegram Payment Bot with Crypto Payment Gateway (NOWPayments)
This project is a fully functional Telegram Payment Bot that allows users to make cryptocurrency payments and gain access to a VIP group upon successful payment. It is built using Python, Flask, and the python-telegram-bot library, with integration to the NOWPayments crypto gateway.

📌 Features
✅ Supports payments using multiple cryptocurrencies via NOWPayments.

✅ Secure and automated payment confirmation using a webhook.

✅ Manual admin approval option for payments (admin can manually approve).

✅ Auto-access to a VIP Telegram group after payment confirmation.

✅ Customizable error messages for better user experience.

✅ Detailed logging of each payment attempt.

🚀 Demo

🚀 How It Works
Users start the bot using /start and see payment options.

They can choose a payment method (TRX, BNB, ETH).

After payment, they use the command /getaccess <order_id> to access the group.

If the payment is confirmed, they are given a link to join the VIP group.

Admins can manually confirm payments if needed.

🚀 Setup Instructions
Prerequisites
Python 3.8 or above.

Replit or any other cloud hosting platform (Heroku, DigitalOcean, etc.).

A NOWPayments account with an API Key.

A Telegram Bot Token (create via @BotFather).

Installation
Clone the Repository:

bash
Copy
Edit
git clone https://github.com/your-username/telegram-payment-bot.git
cd telegram-payment-bot
Install Required Packages:

bash
Copy
Edit
pip install -r requirements.txt
Set Up Environment Variables:
Create a .env file with the following keys:

bash
Copy
Edit
BOT_TOKEN=YOUR_TELEGRAM_BOT_TOKEN
NOWPAY_API=YOUR_NOWPAYMENTS_API_KEY
GROUP_LINK=YOUR_VIP_GROUP_LINK
REPL_OWNER=YOUR_REPL_OWNER_USERNAME
REPL_SLUG=YOUR_REPL_SLUG_NAME
Run the Bot:

bash
Copy
Edit
python main.py
🚀 Webhook Configuration (NOWPayments)
Go to your NOWPayments dashboard.

Set the IPN/Webhook URL to:

arduino
Copy
Edit
https://your-repl-slug.your-repl-username.repl.co/payment-webhook
Make sure the webhook is enabled.

🚀 Usage
Users type /start to see payment options.

They choose a crypto to pay.

After paying, they use /getaccess <order_id>.

If the payment is confirmed, they are given the VIP group link.

🚀 Admin Commands
/approve <order_id> - Manually approve a payment if needed.

/getaccess <order_id> - Check payment status and give access.

🚀 Screenshots
User Flow

Payment Confirmation

🚀 Contributing
Feel free to fork this project, make changes, and submit a pull request.

🚀 License
This project is licensed under the MIT License.

🚀 Support
If you have any questions or need help, feel free to contact me via https://t.me/emranrx
