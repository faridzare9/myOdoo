To create a backup (assuming that the PostgreSQL server is running locally), use the following command:
$ pg_dump -Fc -f dbname.dump dbname
$ tar cjf dbname.tgz dbname.dump ~/.local/share/Odoo/filestore/dbname
--------------------------------------------------------------------------------------------------------------
To restore the backup, run the following command:
$ tar xf dbname.tgz
$ pg_restore -C -d dbname dbname.dump
