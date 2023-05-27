# IMAGINE APPS - PRUEBA TÉCNICA

## Requerimiento 1: Utilizar una fuente de datos pública y gratuita
La fuente de datos seleccionada para este proyecto es la API REST relacionada al COVID-19. La API proporciona información sobre los casos de COVID-19 en diferentes países. La URL de la API es: [https://disease.sh/v3/covid-19/countries](https://disease.sh/v3/covid-19/countries).

## Requerimiento 2: Diseñar y crear un informe de Power BI
El informe de Power BI fue creado utilizando Power BI Desktop. El informe contiene diferentes visualizaciones y dispone de tres páginas para un mejor analisis de la información (Resumen, Casos, Pruebas)
El informe es interactivo, por lo que permite a los usuarios filtrar y seleccionar segmentos de datos, como continente, países específicos o rangos en los valores de casos o pruebas.

**Nota:** Se emplea un cuenta organizacional con licencia de prueba, sin embargo, lo recomdable sería disponer de una licencia completa.

## Requerimiento 3: Publicar el informe en Power BI Service y configurar Power BI Embedded
El informe fue publicado en Power BI Service para facilitar su acceso y compartirlo con otros usuarios. Se configuraron los permisos de acceso adecuados para el informe y se realizo la respectiva públicación para su posterior integración con la aplicación de Angular

## Requerimiento 4: Crear una aplicación Angular básica
Se utilizó la CLI de Angular para crear una aplicación Angular básica. Se ejecutó el siguiente comando:
```
ng new imagineapps-powerbi
```
Esto generó la estructura inicial del proyecto de la aplicación Angular e inicializo el repositorio.

## Requerimiento 5: Implementar Power BI Embedded en la aplicación Angular
Se procede con la generación de las credenciales y la url, para posteriormente realizar la respectiva incrustación del reporte en la aplicación Angular.

## Requerimiento 6: Documentación de configuración y despliegue
Teniendo en cuenta que las necesidades de la aplicación no demandan recursos considerables en cuanto hardware e infraestructura, se procede a desplegar la aplicación mediante **GitHub Pages** para lo cual, se procede a crear una nueva rama, con el siguiente comando

```
git checkout -b gh-pages
```
Se procede a eliminar realizar el build de la aplicación
```
npm run deploy
```
Posteriormente, se extre eliminan todos los archivos de esta rama, exceptuando los generados en el build. `/dist`

Se procede a actualizar el repositorio remoto y GitHub Actions realiza el despliegue.

La aplicación se encuentra disponible en [https://zbrayantg.github.io/imagineapps-powerbi/](https://zbrayantg.github.io/imagineapps-powerbi/)
