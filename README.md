# ReqRes API Testing Suite 🚀

Suite de pruebas automatizadas para [ReqRes.in](https://reqres.in) con 51 tests usando Postman y Newman.

## Estructura

- 📁 **Auth** - Login válido e inválido (8 tests)
- 📁 **Users** - CRUD completo (23 tests)
- 📁 **Register** - Registro válido e inválido (9 tests)
- 📁 **Edge Cases** - 404s y valores límite (11 tests)

## Requisitos

- [Node.js](https://nodejs.org)
- [Newman](https://npmjs.com/package/newman)
- [newman-reporter-htmlextra](https://npmjs.com/package/newman-reporter-htmlextra)

## Instalación
```bash
npm install -g newman
npm install -g newman-reporter-htmlextra
```

## Ejecución
```bash
newman run "ReqRes Suite.postman_collection.json" \
  --environment "ReqRes Dev.postman_environment.json" \
  --reporters htmlextra \
  --reporter-htmlextra-export reporte.html \
  --reporter-htmlextra-title "ReqRes API Test Report"
```

## Resultados

51 tests / 0 fallos ✅# reqres-api-testing
Suite de pruebas API para ReqRes.in con 51 tests automatizados usando Postman y Newman
