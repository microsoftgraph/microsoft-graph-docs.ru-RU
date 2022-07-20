---
title: Перечисление learningContents
description: Получение списка объектов learningContent и их свойств.
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: apiPageType
ms.openlocfilehash: 1194ec4331a8e8a9bb4b28d1269a5ba4b8ca2e8b
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883370"
---
# <a name="list-learningcontents"></a>Перечисление learningContents
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка ресурсов [learningContent](../resources/learningcontent.md) и их свойств.

Этот список представляет метаданные содержимого указанного поставщика в Viva Обучение.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|LearningContent.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|LearningContent.Read.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /employeeExperience/learningProviders/{learningProviderId}/learningContents
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [learningContent](../resources/learningcontent.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "list_learningcontent"
}
-->
``` http
GET /employeeExperience/learningProviders/13727311-e7bb-470d-8b20-6a23d9030d70/learningContents 
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.learningContent",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#learningProviders('13727311-e7bb-470d-8b20-6a23d9030d70')/learningContents",
    "value": [
        {
            "externalId": "LP4771",
            "title": "Manage classes, resources, assessment, and planning in Microsoft Teams with Beedle",
            "description": "A module to guide users through the various teaching and learning enhancements that Beedle provides within Microsoft Teams, with many examples of everyday application.",
            "contentWebUrl": "https://docs.microsoft.com/en-us/learn/modules/manage-classes-resources-assessment-planning-beedle/",
            "sourceName": "MSLibrary",
            "thumbnailWebUrl": "https://syndetics.com/index.aspx?isbn=9783319672175/LC.GIF",
            "languageTag": "en-us",
            "numberOfPages": 10,
            "duration": "PDT1H",
            "format": "Book",
            "createdDateTime": "2018-01-01T00:00:00",
            "lastModifiedDateTime": "2021-04-01T04:26:06.1995367Z",
            "contributor": "Scott Simpson",
            "additionalTags": [
                "Create private or public teams",
                "Add members to teams"
            ],
            "skillTags": [
                "Create teams",
                "Teams channels",
                "Teams members"
            ],
            "isActive": true,
            "isPremium": false,
            "isSearchable": false
        },
        {
            "externalId": "LP4772",
            "title": "Manage classes, resources, assessment, and planning in Microsoft Teams with Beedle",
            "description": "A module to guide users through the various teaching and learning enhancements that Beedle provides within Microsoft Teams, with many examples of everyday application.",
            "contentWebUrl": "https://docs.microsoft.com/en-us/learn/modules/manage-classes-resources-assessment-planning-beedle/",
            "sourceName": "MSLibrary",
            "thumbnailWebUrl": "https://syndetics.com/index.aspx?isbn=9783319672175/LC.GIF",
            "languageTag": "en-us",
            "numberOfPages": 10,
            "duration": "PDT1H",
            "format": "Book",
            "createdDateTime": "2018-01-01T00:00:00",
            "lastModifiedDateTime": "2021-04-01T04:26:06.1995367Z",
            "contributor": "Scott Simpson",
            "additionalTags": [
                "Create private or public teams",
                "Add members to teams"
            ],
            "skillTags": [
                "Create teams",
                "Teams channels",
                "Teams members"
            ],
            "isActive": true,
            "isPremium": false,
            "isSearchable": false
        }
    ]
}
```
