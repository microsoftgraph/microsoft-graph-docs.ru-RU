---
title: Определения списков
description: Список объектов teamTemplateDefinition, связанных с teamTemplate.
author: Charlieforce
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 5e4b629399fa8e8e927028f4c212e8438ba1fa6f
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690165"
---
# <a name="list-definitions"></a>Определения списков
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список объектов [teamTemplateDefinition](../resources/teamstemplate.md) , связанных с [teamTemplate](../resources/teamtemplate.md). 

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Team.Create|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Для приложений|Team.Create|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/teamTemplates?$expand=definitions
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметр запроса `$expand``$filter`[OData](/graph/query-parameters) `$skipToken` и , чтобы настроить ответ.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [teamTemplateDefinition](../resources/teamtemplatedefinition.md) . 

## <a name="examples"></a>Примеры

### <a name="example-1-use-extend-and-filter-to-get-teamtemplatedefinitions-for-en-us-locale"></a>Пример 1. Использование $extend и $filter для получения teamTemplateDefinitions для языкового стандарта en-US

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "list_teamtemplatedefinitions"
}
-->
```http
GET https://graph.microsoft.com/beta/teamwork/teamTemplates?$expand=definitions&filter=definitions/any(a:a/languageTag eq 'en-US')
```

#### <a name="response"></a>Отклик
Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamtemplatedefinition)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "id": "com.microsoft.teams.template.ManageAProject",
            "definitions": [
                {
                    "id": "Y29tLm1pY3Jvc29mdC50ZWFtcy50ZW1wbGF0ZS5NYW5hZ2VBUHJvamVjdCMjUHVibGljIyNlbi1VUw==",
                    "parentTemplateId": "com.microsoft.teams.template.ManageAProject",
                    "displayName": "Manage a Project",
                    "languageTag": "en-US",
                    "audience": "public",
                    "description": "Manage tasks, share documents, conduct project meetings and document risks and decisions with this template for general project management.",
                    "shortDescription": "Coordinate your project.",
                    "lastModifiedDateTime": "0001-01-01T00:00:00Z",
                    "publisherName": "Microsoft",
                    "categories": [
                        "General"
                    ],
                    "lastModifiedBy": null
                }
            ]
        },
        {
            "id": "com.microsoft.teams.template.ManageAnEvent",
            "definitions": [
                {
                    "id": "Y29tLm1pY3Jvc29mdC50ZWFtcy50ZW1wbGF0ZS5NYW5hZ2VBbkV2ZW50IyNQdWJsaWMjI2VuLVVT",
                    "parentTemplateId": "com.microsoft.teams.template.ManageAnEvent",
                    "displayName": "Manage an Event",
                    "languageTag": "en-US",
                    "audience": "public",
                    "description": "Manage tasks, documents, and collaborate on everything you need to deliver a compelling event. Invite guest users to have a secure collaboration inside and outside of your company.",
                    "shortDescription": "Improve your event management and collaboration.",
                    "lastModifiedDateTime": "0001-01-01T00:00:00Z",
                    "publisherName": "Microsoft",
                    "categories": [
                        "General"
                    ],
                    "lastModifiedBy": null
                }
            ]
        },
    ]
}
```
