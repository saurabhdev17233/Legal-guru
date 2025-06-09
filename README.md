# Legal-guru

python manage.py runserver
Watching for file changes with StatReloader
Exception in thread django-main-thread:
Traceback (most recent call last):
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\threading.py", line 1041, in _bootstrap_inner
    self.run()
    ~~~~~~~~^^
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\threading.py", line 992, in run
    self._target(*self._args, **self._kwargs)
    ~~~~~~~~~~~~^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\site-packages\django\utils\autoreload.py", line 64, in wrapper
    fn(*args, **kwargs)
    ~~^^^^^^^^^^^^^^^^^
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\site-packages\django\core\management\commands\runserver.py", line 124, in inner_run
    autoreload.raise_last_exception()
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^^
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\site-packages\django\utils\autoreload.py", line 86, in raise_last_exception
    raise _exception[1]
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\site-packages\django\core\management\__init__.py", line 394, in execute
    autoreload.check_errors(django.setup)()
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^^
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\site-packages\django\utils\autoreload.py", line 64, in wrapper
    fn(*args, **kwargs)
    ~~^^^^^^^^^^^^^^^^^
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\site-packages\django\__init__.py", line 24, in setup
    apps.populate(settings.INSTALLED_APPS)
    ~~~~~~~~~~~~~^^^^^^^^^^^^^^^^^^^^^^^^^
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\site-packages\django\apps\registry.py", line 124, in populate
    app_config.ready()
    ~~~~~~~~~~~~~~~~^^
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\site-packages\django\contrib\admin\apps.py", line 27, in ready
    self.module.autodiscover()
    ~~~~~~~~~~~~~~~~~~~~~~~~^^
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\site-packages\django\contrib\admin\__init__.py", line 52, in autodiscover
    autodiscover_modules("admin", register_to=site)
    ~~~~~~~~~~~~~~~~~~~~^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\site-packages\django\utils\module_loading.py", line 58, in autodiscover_modules
    import_module("%s.%s" % (app_config.name, module_to_search))
    ~~~~~~~~~~~~~^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\importlib\__init__.py", line 88, in import_module
    return _bootstrap._gcd_import(name[level:], package, level)
           ~~~~~~~~~~~~~~~~~~~~~~^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "<frozen importlib._bootstrap>", line 1387, in _gcd_import
  File "<frozen importlib._bootstrap>", line 1360, in _find_and_load
  File "<frozen importlib._bootstrap>", line 1331, in _find_and_load_unlocked
  File "<frozen importlib._bootstrap>", line 935, in _load_unlocked
  File "<frozen importlib._bootstrap_external>", line 1026, in exec_module
  File "<frozen importlib._bootstrap>", line 488, in _call_with_frames_removed
  File "C:\Users\saura\Documents\TRAINING WORK\task\bike_rental\bikerent\rental\admin.py", line 13, in <module>
    @admin.register(Booking)
     ~~~~~~~~~~~~~~^^^^^^^^^
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\site-packages\django\contrib\admin\decorators.py", line 107, in _model_admin_wrapper
    admin_site.register(models, admin_class=admin_class)
    ~~~~~~~~~~~~~~~~~~~^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "C:\Users\saura\AppData\Local\Programs\Python\Python313\Lib\site-packages\django\contrib\admin\sites.py", line 130, in register
    raise AlreadyRegistered(msg)
django.contrib.admin.exceptions.AlreadyRegistered: The model Booking is already registered in app 'rental'.
