# merge-requirements

simple lib for organize two requirements.txt in a unique requirements.txt file

### Example:

```script
pip install merge-requirements

cat requirements_edgcore.txt
gunicorn==0.12.2
python-memcached==1.47
# Projeto publicacao
dashboard==1.3.3
## Globocore e suas dependências ##
globocore==4.11.1
alf==0.4.2

cat requirements_especiais.txt
globocore==4.16.13
Django==1.4.13
IPTCInfo==1.9.5-6
alf==0.4
argparse==1.2.1
gunicorn==0.12.1
html5lib==0.95
#httplib2==0.7.2

merge_requirements requirements_edgcore.txt requirements_especiais.txt
create new file ./requirements-merged.txt

cat requirements-merged.txt
dashboard==1.3.3
Django==1.4.13
gunicorn==0.12.2
argparse==1.2.1
globocore==4.16.13
html5lib==0.95
alf==0.4.2
python-memcached==1.47
IPTCInfo==1.9.5-6

```
