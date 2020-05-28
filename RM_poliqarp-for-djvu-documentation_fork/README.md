Poliqarp for DjVu documentation sources.


Changes required for Django 1.7

W pliku /srv/poliqarp/django.wsgi trzeba ostatnie dwa wiersze zmienić na:
from django.core.wsgi import get_wsgi_application
application = get_wsgi_application()

W pliku marasca/settings/cykat.py trzeba było dodać wiersz
ALLOWED_HOSTS = ['korpusy.klf.uw.edu.pl', 'corpora.klf.uw.edu.pl', 'poliqarp.wbl.klf.uw.edu.pl’]
(Być może lepsze byłoby inne miejsce, tu w każdym razie działa).

