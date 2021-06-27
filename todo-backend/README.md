# Todo App - backend

## Comparison between Google Cloud SQ and PostgreSQL

This is a short comparison between DBaaS like Google Cloud SQL versus "Do if
Yourself" solution like PostgreSQL using persistent volume.

Considering the amount of required work and cost to initialize the systems, they
are in the same level. PostgreSQL and other DIY database solutions running on
Kubernetes using persistent volumes can be easily launched using kubectl and a
small config file. Google Cloud SQL can be set up in minutes: standard
connection drivers and built-in migrational tools allow you to create and
connect to your first database in just a few minutes. Also the cost of
initialization for both strategies is virtually zero.

The bigger differences comes with the maintanibility. When using DIY database
solution, all maintain work has to be done by company itself, including database
upgrades, migrations, backups, scaling, etc. which in general requires quite a
lot of expertise to make things right.

For personal hobby projects, maintaining own database might be an interesting
experiment, but when dealing with real data, the use of DBaaS is better solution
as long as the running costs are not too high compared to the DYI solution. And
that mainly depends on the amount of data.
