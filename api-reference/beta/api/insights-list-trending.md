---
title: Список подписок
description: Вычисляемые представление, которое возвращает список элементов, прибора вокруг пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: bc0dcd70ef8fb527096e8142f188f9c2cbf02193
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926220"
---
# <a name="list-trending"></a>Список подписок

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Вычисляемые представление, которое возвращает список элементов, прибора вокруг пользователя.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.

Можно использовать `$filter` параметр для фильтрации элементов тенденции запроса. Например на основе типа:

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

Или на основе типа контейнера:

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

В разделе Доступные типы контейнеров и типов можно фильтровать по в [resourceVisualization](../resources/insights-resourcevisualization.md).


## <a name="request-headers"></a>Заголовки запросов
| Заголовок       |  Значение|
|:-------------|:------|
| Авторизация  | Bearer {токен}. Обязательный.|
| Accept  | application/json|

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `200 OK` код ответа и список элементов [прибора](../resources/insights-trending.md) в теле ответа. Каждый элемент содержит свойства визуализации для отображения элемента в работу.

## <a name="example"></a>Пример
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a>Ответ
Ниже приведен пример отклика. Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства. В разделе Пример с усеченными ответа в нижней части страницы.
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 801

{
    "value": [
        {
            "id": "id-value",
            "weight": "weight-value",
            "resourceVisualization": {
                "title": "title-value",
                "type": "type-value",
                "mediaType": "mediaType-value",
                "previewImageUrl": "previewImageUrl-value",
                "previewText": "previewText-value",
                "containerWebUrl": "containerWebUrl-value",
                "containerDisplayName": "containerDisplayName-value",
                "containerType": "containerType-value"
            },
            "resourceReference": {
                "webUrl": "webUrl-value",
                "id": "id-value",
                "type": "type-value"
            }
        }
    ]
}
```

### <a name="expanding-resource"></a>Развертывание ресурсов
Можно развернуть ссылается тенденции понимание назначения ресурса.
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
