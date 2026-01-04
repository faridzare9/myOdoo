Odoo server
--------------------------------------

axiom@Axiom:~$ ls
  Desktop    Downloads  odoo-dev  Public  Templates       Videos
  Documents  Music      Pictures  snap    venv-odoo-18.0  wkhtmltox_0.12.6.1-3.jammy_amd64.deb
axiom@Axiom:~$ cd odoo-dev
axiom@Axiom:~/odoo-dev$ cd odoo
axiom@Axiom:~/odoo-dev/odoo$ ls
  addons           COPYRIGHT  doc      MANIFEST.in  odoo-bin   requirements.txt  setup      setup.py
  CONTRIBUTING.md  debian     LICENSE  odoo         README.md  SECURITY.md       setup.cfg
axiom@Axiom:~/odoo-dev/odoo$

python3 odoo-bin -d 'databasename' -i base --addons-path=addons --db-filter=odoo-test
