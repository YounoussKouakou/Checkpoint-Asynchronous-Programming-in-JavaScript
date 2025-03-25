# Async/Await - Point de Contrôle

Ce projet vise à démontrer l'utilisation de `async/await` en JavaScript à travers plusieurs tâches liées à la gestion des appels asynchrones, de la gestion des erreurs, de l'enchaînement des fonctions et de l'attente de requêtes simultanées et parallèles.

## Objectif

Dans ce point de contrôle, vous apprendrez et appliquerez les concepts suivants :
- Itérer avec `async/await`
- Attendre un appel API
- Gérer les erreurs avec `async/await`
- Enchaîner des fonctions asynchrones avec `async/await`
- Attendre des requêtes simultanées avec `Promise.all()`
- Attendre des appels parallèles avec `Promise.all()`

## Tâches

### Tâche 01 : Itérer avec `Async/Await`

Créer une fonction asynchrone `iterateWithAsyncAwait` qui prend un tableau de valeurs et enregistre chaque valeur avec un délai de 1 seconde entre les enregistrements.

```javascript
async function iterateWithAsyncAwait(values) {
    for (const value of values) {
        await new Promise(resolve => setTimeout(resolve, 1000));  // Délai de 1 seconde
        console.log(value);  // Enregistre la valeur
    }
}
