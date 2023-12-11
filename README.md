First Steps¶

[Source Premiers pas avec FastAPI](https://fastapi.tiangolo.com/tutorial/first-steps/)


The simplest FastAPI file could look like this:

Bien sûr, voici le texte reformaté en Markdown pour un fichier README, parfait pour présenter votre projet FastAPI sur GitHub ou d'autres plateformes supportant Markdown :

```markdown
# Premiers Pas avec FastAPI

## Création d'un Fichier Simple

Le fichier FastAPI le plus simple pourrait ressembler à ceci :

```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
async def root():
    return {"message": "Hello World"}
```

Copiez cela dans un fichier nommé `main.py`.

## Exécution du Serveur en Direct

Exécutez le serveur en direct avec la commande suivante :

```bash
uvicorn main:app --reload
```

Vous devriez voir des informations de démarrage dans la console, semblables à :

```
INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
INFO:     Started reloader process [28720]
INFO:     Started server process [28722]
INFO:     Waiting for application startup.
INFO:     Application startup complete.
```

## À Noter

La commande `uvicorn main:app` fait référence à :

- `main` : le fichier `main.py` (le "module" Python).
- `app` : l'objet créé dans `main.py` avec la ligne `app = FastAPI()`.
- `--reload` : fait redémarrer le serveur après des modifications de code. À utiliser uniquement pour le développement.

Dans la sortie, il y a une ligne indiquant l'URL où votre application est servie localement :

```
INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
```

## Vérification

Ouvrez votre navigateur à l'adresse http://127.0.0.1:8000.

Vous verrez la réponse JSON comme suit :

```json
{"message": "Hello World"}
```

## Documentation API Interactive

Rendez-vous maintenant à l'adresse http://127.0.0.1:8000/docs.

Vous verrez la documentation API interactive automatique (fournie par Swagger UI) :

![Swagger UI](https://fastapi.tiangolo.com/img/index/index-01-swagger-ui-simple.png)
```

Ce formatage en Markdown permet de structurer clairement le contenu pour une meilleure lisibilité. Vous pouvez le copier directement dans votre fichier README.md. N'oubliez pas de remplacer `lien_vers_image_swagger_ui` par le lien approprié de l'image Swagger UI si vous souhaitez inclure une capture d'écran dans votre documentation.
