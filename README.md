# Book Search App

Proyecto de aprendizaje: desarrollo seguro con IA.

## Descripcion

API REST con Express.js que permite buscar libros por titulo. Endpoint: `GET /books/:title` que busca coincidencias parciales en una base de datos mock.

## Instalacion

```bash
npm install
```

## Uso

```bash
npm start
# Servidor en http://localhost:3000
```

Ejemplo de peticion:
```
GET http://localhost:3000/books/quijote
```

Respuesta:
```json
{
  "success": true,
  "data": [
    {
      "id": 1,
      "title": "Don Quijote de la Mancha",
      "author": "Miguel de Cervantes",
      "year": 1605,
      "genre": "Novela"
    }
  ],
  "error": null
}
```

## Tests

```bash
npm test
```

## Como se uso la IA

- Handler generado por Claude
- Cada linea fue revisada manualmente
- Tests expandidos con edge cases (null, vacio, case-insensitive, multiples resultados)

Ver `RULES.md` para la politica completa.
