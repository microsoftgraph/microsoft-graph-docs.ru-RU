---
title: Получение участников
description: Извлечение свойств и связи объекта **участника** .
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: bdcf52f844ea000458d35aa211e7c32a5c6566e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837697"
---
# <a name="get-participant"></a>Получение участников

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Извлечение свойств и связи объекта **участника** .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
| :-------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается        |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается        |
| Application     | Нет                                        |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /applications/{id}/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [участника](../resources/participant.md) в теле ответа.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос
Ниже показан пример запроса.
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}
```

##### <a name="response"></a>Ответ

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "initiatedBy": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "languageId-value",
      "region": "region-value"
    },
    "status": "recordingCapable"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
