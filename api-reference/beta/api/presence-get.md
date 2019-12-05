---
title: Получение сведений о присутствии
description: Получение сведений о присутствии пользователя.
author: VinodRavichandran
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 3d1b56dc8266eea42c773596c8e78e9e0ece5b6b
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844185"
---
# <a name="get-presence"></a>Получение сведений о присутствии

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение сведений о [присутствии](../resources/presence.md) пользователя.

## <a name="permissions"></a>Разрешения
Для вызова этих API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий)                  |
| :-------------- | :----------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Присутствие. Read, присутствие. Read. ALL                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                         |
| Application                            | Не поддерживается.                                  |

## <a name="http-requests"></a>HTTP-запросы
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
```

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |


## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [присутствия](../resources/presence.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-get-your-own-presence-information"></a>Пример 1: получение собственных сведений о присутствии

В приведенном ниже примере показано, как получить сведения о присутствии. Для выполнения этой операции требуется разрешение на присутствие. чтение.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "name": "get-your-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{  
    "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "availability": "Available",
    "activity": "Available"
}
```

### <a name="example-2-get-the-presence-information-of-another-user"></a>Пример 2: получение сведений о присутствии другого пользователя

В приведенном ниже примере показано, как получить сведения о присутствии для другого пользователя. Для выполнения этой операции требуется разрешение на присутствие. Read. ALL.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```http
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "name": "get-user-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
    "id": "66825e03-7ef5-42da-9069-724602c31f6b",
    "availability": "DoNotDisturb",
    "activity": "Presenting"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Presence",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
