import telebot
token = 'ваш token api'
bot = telebot.TeleBot(token)
@bot.message_handler(commands=['start'])
def start_message(message):
bot.send_message(message.chat.id, 'Привет!')
bot.polling()
