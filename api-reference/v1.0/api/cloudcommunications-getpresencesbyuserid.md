---
title: 'cloudCommunications: getPresencesByUserId'
description: Получите сведения о присутствии для нескольких пользователей.
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 1eae5f86955732829c3eed56be531588f5155eb5
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689164"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a>cloudCommunications: getPresencesByUserId

Пространство имен: microsoft.graph

Получите сведения [о](../resources/presence.md) присутствии для нескольких пользователей.

## <a name="permissions"></a>Разрешения
Для вызова этих API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий)                  |
| :-------------- | :----------------------------------------------------------- |
| Делегированное (рабочая или учебная учетная запись)     | Presence.Read.All                         |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается.                         |
| Приложение                            | Не поддерживается.                                  |

> **Примечания:**
> * Для каждого запроса API поддерживается не более 650 пользовательских ИД.
> * Максимальная скорость запросов этого API составляет 1500 запросов API в течение 30 секунд для каждого приложения на клиента.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a>Заглавные запросы
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |
|Content-Type | application/json. Обязательный. |


## <a name="request-body"></a>Текст запроса

В теле запроса укажу объект JSON со следующим параметром.

| Параметр      | Тип    |Описание|
|:---------------|:--------|:----------|
|ids|Коллекция String|ИД объектов пользователя.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [присутствия](../resources/presence.md) в тексте отклика.


## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже показан пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-presence-multiple-users"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/getPresencesByUserId
Content-Type: application/json

{
    "ids": ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-presence-multiple-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a>Отклик
Ниже показан пример отклика.

> **Примечание.** Объекты ответа могут быть сокращены для учитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "name": "get-presence-multiple-users",
  "truncated": "true",
  "@odata.type": "microsoft.graph.presence"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574
```
```json
{
    "value": [{
            "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
            "availability": "Busy",
            "activity": "InAMeeting"
        },
        {
            "id": "66825e03-7ef5-42da-9069-724602c31f6b",
            "availability": "Away",
            "activity": "Away"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List Presence Information",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


