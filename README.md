# Tempel.BOI

Catatan re-deployment http://tempel.blankonlinux.or.id

---------------------------------------------------------------------

## Dependensi:
* Python 2.6.6
* Django 1.2.5
* SQLite3

---------------------------------------------------------------------

## Instalasi

Jalankan perintah:

```sh
$ cd $HOME
$ git clone https://github.com/yyuu/pyenv.git ~/.pyenv
$ echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bash_profile
$ echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bash_profile
$ echo 'eval "$(pyenv init -)"' >> ~/.bash_profile
```

Reload shell, lalu jalankan perintah instalasi Python 2.6.6.

```sh
$ pyenv install 2.6.6
```

Pasang virtualenv melalui pip dan buat lingkungan virtual lalu aktifkan.

```sh
$ pip install virtualenv
$ virtualenv venv01
$ source venv01/bin/activate
```

Pasang django.

```sh
$ pip install django==1.2.5
```

Unduh revisi terakhir dari dev.blankonlinux.or.id atau repo github ini.

```sh
$ bzr branch http://dev.blankonlinux.or.id/browser/infrastruktur/tempel
```

Coba jalankan.

```sh
$ cd tempel
$ python manage.py runserver
```

---------------------------------------------------------------------

## Catatan

Sampai saat ini masih terdapat beberapa masalah yang harus ditelusuri.
