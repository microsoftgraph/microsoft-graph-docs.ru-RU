---
title: Список "Популярные"
description: Расчетные данные, возвращающие список элементов, популярных в окружении пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 9261db7230c1655398f61f5f37d9f6792f79d066
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051363"
---
# <a name="list-trending"></a>Список "Популярные"

Пространство имен: microsoft.graph

Вычисляемая информация, которая включает список документов, включающих тенденции вокруг пользователя.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
Получите список документов, которые будут ходить по пользователю или указанному пользователю:

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

Расширение ресурса, на который ссылается **трендовая** информация:

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

Параметр запроса можно использовать для `$filter` фильтрации элементов тренда. Например, в зависимости от **типа:**

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

Или на основе **containerType:**

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

В [resourceVisualization](../resources/insights-resourcevisualization.md)см. доступные типы и типы контейнеров, которые можно фильтровать.


## <a name="request-headers"></a>Заголовки запросов
| Заголовок       |  Значение|
|:-------------|:------|
| Авторизация  | Bearer {токен}. Обязательный.|
| Accept  | application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и список элементов `200 OK` [тренда](../resources/insights-trending.md) в тексте ответа. Каждый элемент содержит свойства визуализации для отображения элемента в вашем опыте.

## <a name="example"></a>Пример
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.
```http
GET https://graph.microsoft.com/v1.0/me/insights/trending
```
#### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. В нижней части страницы см. пример не усеченного ответа.
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "AWMiSOpKHlJCpP_ZoVJQXi9ees4wFhDQQqF55Pm5DlaMzvtd2zra4UWSTEvpTldvb6EhQ289G4BAsxnrajQyjW1jIkjqSh5SQqT_2aFSUF4vBQ",
            "weight": "0.1583399742569597",
            "resourceVisualization": {
                "title": "LiveCaptions",
                "type": "Image",
                "mediaType": "application/octet-stream",
                "previewImageUrl": "https://contoso.sharepoint.com/_api/v2.0/drives/b!YyJI6koeUkKk_9mhUlBeL156zjAWENBCoXnk-bkOVozO-13bOtrhRZJMS-lOV29v/items/01H273TR5BEFBW6PI3QBALGGPLNI2DFDLN/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerWebUrl": "https://contoso.sharepoint.com/sites/Mark8ProjectTeam/Shared Documents/Go to Market Plan",
                "containerDisplayName": "Mark 8 Project Team",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://contoso.sharepoint.com/sites/Mark8ProjectTeam/Shared%20Documents/Go%20to%20Market%20Plan/LiveCaptions.gif",
                "id": "drives/b!YyJI6koeUkKk_9mhUlBeL156zjAWENBCoXnk-bkOVozO-13bOtrhRZJMS-lOV29v/items/01H273TR5BEFBW6PI3QBALGGPLNI2DFDLN",
                "type": "microsoft.graph.driveItem"
            }
        }
    ]
}
```
