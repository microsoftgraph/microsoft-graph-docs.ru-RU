---
title: Список "Использованные"
description: Вычисляемое представление, которое возвращает список файлов, используемых с пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 31115a845c3b5af80aaba700e55e0ede05d922b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953075"
---
# <a name="list-used"></a>Список "Использованные"

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вычисляемое представление, которое возвращает список файлов, используемых с пользователем.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
```http
GET /me/insights/used
```
Запрос документов, использовавшихся другими пользователями возвращает результаты, отсортированные по адресу "lastModifiedDateTime", а для "свойство lastaccesseddatetime" задано значение "lastModifiedDateTime".
```http
GET /users/{id | userPrincipalName}/insights/used
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.

С помощью параметра `$filter` запроса можно отфильтровать используемые элементы. Например, на основе типа:

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

Или на основе типа контейнера:

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).


## <a name="request-headers"></a>Заголовки запросов
| Заголовок       |  Значение|
|:-------------|:------|
| Авторизация  | Bearer {токен}. Обязательный.|
| Accept  | application/json|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список [использованных](../resources/insights-used.md) элементов в теле отклика.
## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a>Отклик

Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства. 
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastused" : { 
                "lastAccessedDateTime" : "lastAccessedDateTime-value", 
                "lastModifiedDateTime": "lastModifiedDateTime-value" 
            },
            "resourceVisualization": { 
                "title" : "title-value, 
                "type"  : "type-value",
                "mediaType" : "mediaType-value",
                "previewImageUrl" : previewImageUrl-value, 
                "previewText" : "previewText-value", 
                "containerWebUrl" : "containerWebUrl-value", 
                "containerDisplayName" : "containerDisplayName-value", 
                "containerType" : "containerType-value" 
            }, 
            "resourceReference" : { 
                "webUrl" : "webUrl-value", 
                "id": "id-value", 
                "type: "type-value" 
            }
        }
    ]
}
```

### <a name="expanding-resource"></a>Расширение ресурса
Ресурс, на который ссылается использованная аналитика, может быть расширен.
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
