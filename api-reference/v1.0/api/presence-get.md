---
title: Получение сведений о присутствии
description: Получение сведений о присутствии пользователя.
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: a82c03e9b63d83f8aab8b3556e75b17d926ff3e6
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581249"
---
# <a name="get-presence"></a>Получение сведений о присутствии

Пространство имен: microsoft.graph

Получение сведений о [присутствии](../resources/presence.md) пользователя.

## <a name="permissions"></a>Permissions
Для вызова этих API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий)                  |
| :-------------- | :----------------------------------------------------------- |
| Делегированное (рабочая или учебная учетная запись)     | Presence.Read, Presence.Read.All      |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается.                        |
| Приложение                            | Не поддерживается.                        |

> **Примечание:** Максимальная частота запросов для этого API составляет 1500 запросов API в течение 30-секундного периода на приложение для каждого клиента.

## <a name="http-requests"></a>HTTP-запросы
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |


## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
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
GET https://graph.microsoft.com/v1.0/me/presence
```

---


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
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```

---


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

### <a name="example-3-get-the-presence-information-of-another-user"></a>Пример 3: получение сведений о присутствии другого пользователя

В приведенном ниже примере показано, как получить сведения о присутствии для другого пользователя. Для выполнения этой операции требуется разрешение на присутствие. Read. ALL.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "name": "get-user-presences",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
            "availability": "Away",
            "activity": "BeRightBack"
        }
    ]
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


