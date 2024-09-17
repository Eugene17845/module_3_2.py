def send_email(message,recipient,sender = "university.help@gmail.com"):
    print(send_email)


message = str(input('Введите текст:', ))
recipient = str(input('Ведите почту получателя:', ))
sender = str(input('Ведите почту отправителя:', ))
if recipient == sender:
    print('Нельзя отправить письмо самому себе!')
elif sender == 'university.help@gmail.com':
    print('Письмо успешно отправлено с адреса', sender, 'на адрес', recipient, '.')
elif ("@" and (".com" or ".ru" or ".net")) not in recipient and ("@" and (".com" or ".ru" or ".net")) not in sender:
    print('Невозможно отправить письмо с адреса', sender, 'на адрес', recipient, '.')
else:
    print('НЕСТАНДАРТНЫЙ ОТПРАВИТЕЛЬ! Письмо отправлено с адреса', sender, 'на адрес', recipient, '.')
