---
ms.author: yiwenwang
title: Чтобы отобразить макет отображения, используйте API поиска Майкрософт в Microsoft Graph
description: Используйте API поиска Майкрософт в Microsoft Graph для отображения результатов поиска по-разному.
author: yiwenwang
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: bc125fa05c6ba466c5430c07de822d0912f3cbad
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337133"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-manage-layout-templates-for-search-results-preview"></a>Используйте API поиска Майкрософт в Microsoft Graph для управления шаблонами макетов для результатов поиска (предварительный просмотр)

Макет отображения поиска или тип результатов — это правило, которое вызывает отображение различных видов результатов поиска на страницах результатов поиска по-разному. Оно состоит из следующих компонентов. 

- Одна или несколько характеристик или условий для сравнения каждого результата поиска, например источника или типа контента результата поиска.
- Шаблон отображения для результатов поиска, соответствующих условиям. Шаблон отображения определяет внешний вид и поведение результатов, соответствующих условиям. 

API поиска Microsoft Graph предоставляет рендеративный ответ на основе [адаптивных карт](https://adaptivecards.io/). С помощью [шаблона адаптивной карты](https://adaptivecards.io/designer) клиенты могут отрисовки различных результатов поиска на разных холстах.

Клиенты могут настроить тип результатов поиска в центре администрирования [Microsoft 365](https://admin.microsoft.com/Adminportal/Home#/MicrosoftSearch/resulttypes).

## <a name="request-example"></a>Пример запроса

В следующем примере показано, как получить макеты или шаблоны результатов отображения результатов поиска, задав свойство **enableResultTemplate** `true` в контракте на запрос.

В reponse показаны три поисковых хита, два из которых связаны с **результатомTemplateId** 1603900360618_5XCBK2OXG, а другой с **результатомTemplateId** 1603900360618_5XCBK2OXP. Эти ID совпадают с одним из ключей двух макетов отображения, содержащихся в словаре **resultTemplates** , включенном в контракт на ответ. С помощью ID-кода шаблона результатов можно определить, какой макет отображения использовать для отрисовки каждого результата поиска.

### <a name="request"></a>Запрос

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "externalItem"
            ],
            "contentSources": [
                "Connectors"
            ],
            "query": {
                "queryString": "*"
            },
            "resultTemplateOptions": {
                "enableResultTemplate": true
            }
        }
    ]
}
```

### <a name="response"></a>Отклик


```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "searchTerms": [],
            "hitsContainers": [
                {
                    "total": 1201701,
                    "moreResultsAvailable": true,
                    "hits": [
                        {
                            "hitId": "85437765-b430-434f-a945-38eceead5b93",
                            "rank": 1,
                            "summary": "",
                            "resultTemplateId": "1603900360618_5XCBK2OXG",
                            "resource": {
                                "@odata.type": "#microsoft.graph.externalItem",
                                "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17397",
                                "Title": "[SM00186] Number of tests - Liquid",
                                "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                            }
                        },
                        {
                            "hitId": "85437765-5430-434f-a945-38eceead5b94",
                            "rank": 2,
                            "summary": "",
                            "resultTemplateId": "1603900360618_5XCBK2OXP",
                            "resource": {
                                "@odata.type": "#microsoft.graph.externalItem",
                                "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17398",
                                "Title": "[SM00186] Number of tests - Liquid 2",
                                "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                            }
                        },
                        {
                            "hitId": "85437765-b430-434f-a945-38eceead5b95",
                            "rank": 3,
                            "summary": "",
                            "resultTemplateId": "1603900360618_5XCBK2OXG",
                            "resource": {
                                "@odata.type": "#microsoft.graph.externalItem",
                                "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17399",
                                "Title": "[SM00186] Number of tests - Liquid 3",
                                "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                            }
                        }
                    ]
                }
            ],
            "resultTemplates": {
                "1603900360618_5XCBK2OXG": {
                    "displayName": "Liquid-3",
                    "body": {
                        "type": "AdaptiveCard",
                        "version": "1.0",
                        "body": [
                            {
                                "type": "ColumnSet",
                                "columns": [
                                    {
                                        "type": "Column",
                                        "width": "auto",
                                        "items": [
                                            {
                                                "type": "Image",
                                                "url": "https://searchuxcdn.azureedge.net/designerapp/images/LiquidLogo.png",
                                                "horizontalAlignment": "Center",
                                                "size": "Small"
                                            }
                                        ],
                                        "horizontalAlignment": "Center"
                                    },
                                    {
                                        "type": "Column",
                                        "width": 10,
                                        "items": [
                                            {
                                                "type": "TextBlock",
                                                "text": "[{Title}]({URL})",
                                                "weight": "Bolder",
                                                "color": "Accent",
                                                "size": "Medium",
                                                "maxLines": 3
                                            },
                                            {
                                                "type": "TextBlock",
                                                "text": "{ResultSnippet}",
                                                "maxLines": 3,
                                                "wrap": true
                                            }
                                        ],
                                        "spacing": "Medium"
                                    }
                                ]
                            }
                        ],
                        "$schema": "http://adaptivecards.io/schemas/adaptive-card.json"
                    }
                },
                "1603900360618_5XCBK2OXP": {
                    "displayName": "Liquid-2",
                    "body": {
                        "type": "AdaptiveCard",
                        "version": "1.0",
                        "body": [
                            {
                                "type": "ColumnSet",
                                "columns": [
                                    {
                                        "type": "Column",
                                        "width": "auto",
                                        "items": [
                                            {
                                                "type": "Image",
                                                "url": "https://searchuxcdn.azureedge.net/designerapp/images/LiquidLogo.png",
                                                "horizontalAlignment": "Center",
                                                "size": "Small"
                                            }
                                        ],
                                        "horizontalAlignment": "Center"
                                    },
                                    {
                                        "type": "Column",
                                        "width": 10,
                                        "items": [
                                            {
                                                "type": "TextBlock",
                                                "text": "[{Title}]({URL})",
                                                "weight": "Bolder",
                                                "color": "Accent",
                                                "size": "Medium",
                                                "maxLines": 3
                                            },
                                            {
                                                "type": "TextBlock",
                                                "text": "{ResultSnippet}",
                                                "maxLines": 3,
                                                "wrap": true
                                            }
                                        ],
                                        "spacing": "Medium"
                                    }
                                ]
                            }
                        ],
                        "$schema": "http://adaptivecards.io/schemas/adaptive-card.json"
                    }
                }
            }
        }
    ]
}

```

## <a name="web-component-example"></a>Пример веб-компонентов

В следующем примере показано, как использовать шаблон адаптивной карты для отрисовки результатов поиска.

> [!IMPORTANT] 
> 
> В этом примере используется версия шаблона адаптивной карты раньше выпуска **в мае 2020 г**. Дополнительные сведения см. в статьях:
> - [Шаблонирование адаптивной карты](/adaptive-cards/templating/)
> - [Адаптивная карта с шаблонированием SDK](/adaptive-cards/templating/sdk)


<!-- markdownlint-disable MD024 -->
```HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="utf-8" />
    <title>Adaptive Cards Example</title>

    <script src="https://unpkg.com/markdown-it@8.4.0/dist/markdown-it.js"></script>
    <script src="https://unpkg.com/adaptivecards/dist/adaptivecards.min.js"></script>

    <script src="https://unpkg.com/adaptivecards-templating@0.1.0-alpha1/dist/adaptivecards-templating.min.js"></script>
    <script src="https://code.jquery.com/jquery-3.6.0.js"
        integrity="sha256-H+K7U5CnXl1h5ywQfKtSj8PCmoN9aaq30gDh27Xc0jk=" crossorigin="anonymous"></script>

    <style type="text/css">
        #exampleDiv {
            border: solid 1px black;
        }
    </style>

    <script type="text/javascript">

       function renderCard() {
            var mockdata = this.getMockData();
            var renderTemplates = [];

            // Convert object to map
            var templateDictionary = new Map(Object.entries( mockdata.value[0].resultTemplates));

            for (let hit of mockdata.value[0].hitsContainers[0].hits) {
                renderTemplates.push(this.renderACT(hit, templateDictionary));
            }

            for(let template of renderTemplates){
                document.getElementById('exampleDiv').appendChild(template);
            }
        }

        function renderACT(hit, templateDictionary) {
            var templateId = hit.resultTemplateId;
            // Define a template payload
            var templatePayload = templateDictionary.get(templateId).body;
            var template = new ACData.Template(templatePayload);

            // Expand the template with your `$root` data object.
            // This binds it to the data and produces the final Adaptive Card payload

            console.log(hit.resource);

            // Create a data binding context, and set its $root property to the
            // data object to bind the template to
            var context = new ACData.EvaluationContext();
            context.$root = hit.resource;

            console.log(context);
            var card = template.expand(context);
            // OPTIONAL: Render the card (requires that the adaptivecards library be loaded)

            var adaptiveCard = new AdaptiveCards.AdaptiveCard();
            adaptiveCard.parse(card);
            return adaptiveCard.render();
        }

        function getMockData() {
            return {
                "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.searchResponse)",
                "value": [
                    {
                        "searchTerms": [],
                        "hitsContainers": [
                            {
                                "total": 1201701,
                                "moreResultsAvailable": true,
                                "hits": [
                                    {
                                        "hitId": "85437765-b430-434f-a945-38eceead5b93",
                                        "rank": 1,
                                        "summary": "",
                                        "resultTemplateId": "1603900360618_5XCBK2OXG",
                                        "resource": {
                                            "@odata.type": "#microsoft.graph.externalItem",
                                            "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17397",
                                            "Title": "[SM00186] Number of tests - Liquid",
                                            "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                                        }
                                    },
                                    {
                                        "hitId": "85437765-5430-434f-a945-38eceead5b94",
                                        "rank": 2,
                                        "summary": "",
                                        "resultTemplateId": "1603900360618_5XCBK2OXP",
                                        "resource": {
                                            "@odata.type": "#microsoft.graph.externalItem",
                                            "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17398",
                                            "Title": "[SM00186] Number of tests - Liquid 2",
                                            "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                                        }
                                    },
                                    {
                                        "hitId": "85437765-b430-434f-a945-38eceead5b95",
                                        "rank": 3,
                                        "summary": "",
                                        "resultTemplateId": "1603900360618_5XCBK2OXG",
                                        "resource": {
                                            "@odata.type": "#microsoft.graph.externalItem",
                                            "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17399",
                                            "Title": "[SM00186] Number of tests - Liquid 3",
                                            "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                                        }
                                    }
                                ]
                            }
                        ],
                        "resultTemplates": {
                            "1603900360618_5XCBK2OXG": {
                                "displayName": "Liquid-3",
                                "body": {
                                    "type": "AdaptiveCard",
                                    "version": "1.0",
                                    "body": [
                                        {
                                            "type": "ColumnSet",
                                            "columns": [
                                                {
                                                    "type": "Column",
                                                    "width": "auto",
                                                    "items": [
                                                        {
                                                            "type": "Image",
                                                            "url": "https://searchuxcdn.azureedge.net/designerapp/images/LiquidLogo.png",
                                                            "horizontalAlignment": "Center",
                                                            "size": "Small"
                                                        }
                                                    ],
                                                    "horizontalAlignment": "Center"
                                                },
                                                {
                                                    "type": "Column",
                                                    "width": 10,
                                                    "items": [
                                                        {
                                                            "type": "TextBlock",
                                                            "text": "[{Title}]({URL})",
                                                            "weight": "Bolder",
                                                            "color": "Accent",
                                                            "size": "Medium",
                                                            "maxLines": 3
                                                        },
                                                        {
                                                            "type": "TextBlock",
                                                            "text": "{ResultSnippet}",
                                                            "maxLines": 3,
                                                            "wrap": true
                                                        }
                                                    ],
                                                    "spacing": "Medium"
                                                }
                                            ]
                                        }
                                    ],
                                    "$schema": "http://adaptivecards.io/schemas/adaptive-card.json"
                                }
                            },
                            "1603900360618_5XCBK2OXP": {
                                "displayName": "Liquid-2",
                                "body": {
                                    "type": "AdaptiveCard",
                                    "version": "1.0",
                                    "body": [
                                        {
                                            "type": "ColumnSet",
                                            "columns": [
                                                {
                                                    "type": "Column",
                                                    "width": "auto",
                                                    "items": [
                                                        {
                                                            "type": "Image",
                                                            "url": "https://searchuxcdn.azureedge.net/designerapp/images/LiquidLogo.png",
                                                            "horizontalAlignment": "Center",
                                                            "size": "Small"
                                                        }
                                                    ],
                                                    "horizontalAlignment": "Center"
                                                },
                                                {
                                                    "type": "Column",
                                                    "width": 10,
                                                    "items": [
                                                        {
                                                            "type": "TextBlock",
                                                            "text": "[{Title}]({URL})",
                                                            "weight": "Bolder",
                                                            "color": "Accent",
                                                            "size": "Medium",
                                                            "maxLines": 3
                                                        },
                                                        {
                                                            "type": "TextBlock",
                                                            "text": "{ResultSnippet}",
                                                            "maxLines": 3,
                                                            "wrap": true
                                                        }
                                                    ],
                                                    "spacing": "Medium"
                                                }
                                            ]
                                        }
                                    ],
                                    "$schema": "http://adaptivecards.io/schemas/adaptive-card.json"
                                }
                            }
                        }
                    }
                ]
            }

        }

    </script>

</head>

<body onload="renderCard()">
    <h1>Adaptive Cards Data Binding Example</h1>
    <div id="exampleDiv"></div>
</body>

</html>
```

## <a name="see-also"></a>См. также

- [Создание макета для настройки результатов поиска](/microsoftsearch/customize-results-layout)
- [Используйте API поиска Майкрософт](/graph/api/resources/search-api-overview)
