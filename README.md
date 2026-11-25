# Бағлан Бекайдар — AI-маркетолог сайты

Рилс · Таргет · Запуск. Лендинг: кейстер, қызметтер, WhatsApp өтінім формасы.

## Жергілікті іске қосу

```bash
pip install -r requirements.txt
python flask_app.py
```
Содан кейін http://127.0.0.1:5000 ашыңыз.

## PythonAnywhere-ге орналастыру

1. **Consoles → Bash** ашып:
   ```bash
   git clone https://github.com/LagerREG11/baglan-site.git
   ```
2. **Web → Add a new web app → Next → Flask → Python 3.10** (кез келген соңғы нұсқа).
   Path сұрағанда: `/home/<USERNAME>/baglan-site/flask_app.py`
3. **Web** бетінде:
   - *Source code*: `/home/<USERNAME>/baglan-site`
   - *Static files*: URL `/static/` → Directory `/home/<USERNAME>/baglan-site/static/`
4. **WSGI configuration file** ішінде мына жолдар болуы керек:
   ```python
   import sys
   path = '/home/<USERNAME>/baglan-site'
   if path not in sys.path:
       sys.path.insert(0, path)
   from flask_app import app as application
   ```
5. Жасыл **Reload** батырмасын басыңыз → сайт `https://<USERNAME>.pythonanywhere.com` мекенжайында ашылады.

## Жаңарту
```bash
cd ~/baglan-site && git pull
```
Содан кейін Web бетінде **Reload**.

## WhatsApp нөмірі
`templates/index.html` соңындағы `var WA_NUMBER = "77474030693";`
