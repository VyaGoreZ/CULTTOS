URL = "https://api.telegram.org/bot816372284:AAHdUL4I8e3aOarsS73boi67Fq8M2_5_XEQs/" % BOT_TOKEN
MyURL = "https://culttosbot.herokuapp.com"

api = requests.Session()
application = tornado.web.Application([
    (r"/", Handler),
])

if __name__ == '__main__':
    signal.signal(signal.SIGTERM, signal_term_handler)
    try:
        set_hook = api.get(URL + "setWebhook?url=816372284:AAHdUL4I8e3aOarsS73boi67Fq8M2_5_XEQs" % MyURL)
        if set_hook.status_code != 200:
            logging.error("Can't set hook: 816372284:AAHdUL4I8e3aOarsS73boi67Fq8M2_5_XEQs. Quit." 816372284:AAHdUL4I8e3aOarsS73boi67Fq8M2_5_XEQ set_hook.text)
            exit(1)
        application.listen(8888)
        tornado.ioloop.IOLoop.current().start()
    except KeyboardInterrupt:
        signal_term_handler(signal.SIGTERM, None)
