# Installation

Pour installer ce paquet, non propagé vers `pip`, il faut : 

```
python -m venv <NOM_ENVIRONNEMENT_VIRTUEL>
source <NOM_ENVIRONNEMENT_VIRTUEL>/bin/activate
pip install certstream

cd /tmp
git clone https://github.com/yapoc/websocket-client.git
cd websocket-client
python setup.py build
python setup.py install

cd /tmp
git clone https://github.com/yapoc/certstream-python.git
cd certstream-python
python setup.py build
python setup.py install
```

# Utilisation & exemples

En plus de toutes les informations que vous pourrez trouver sur la [documentation originale du projet](https://github.com/CaliDog/certstream-python), vous pouvez maintenant utiliser ce paquet derrière un proxy nécessitant une authentification :  

```
(NOM_ENVIRONNEMENT_VIRTUEL) certstream --proxy-host <HÔTE_PROXY> --proxy-port <PORT_PROXY> --proxy-auth "<LOGIN_PROXY>:<MOT_DE_PASSE_PROXY>"
```
