---
title: Список teamworkTags
description: Получите список объектов teamworkTag и их свойств.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 0a5e008e32565675982ec7d120be3d6d3bad98ed
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060722"
---
# <a name="list-teamworktags"></a>Список teamworkTags
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [тегов](../resources/teamworktag.md) и их свойств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Не поддерживается.|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|TeamworkTag.Read.All, TeamworkTag.ReadWrite.All|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|members|[коллекция teamworkTag](../resources/teamworktag.md)|Теги, присвоенные команде.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-Id}/tags
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [teamworkTag](../resources/teamworktag.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_teamworktag"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamworkTag)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "@odata.type": "#microsoft.graph.teamworkTag",
        "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
        "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
        "displayName": "Finance",
        "description": "Finance Team for Mach 8 Project",
        "memberCount": 2,
        "tagType": "standard"
    },
    {
        "@odata.type": "#microsoft.graph.teamworkTag",
        "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjIzk3ZjYyMzQ0LTU3ZGMtNDA5Yy04OGFkLWM0YWYxNDE1OGZmNQ==",
        "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
        "displayName": "Legal",
        "description": "Legal experts, ask us your legal questions",
        "memberCount": 4,
        "tagType": "standard"
    }
  ]
}
```

