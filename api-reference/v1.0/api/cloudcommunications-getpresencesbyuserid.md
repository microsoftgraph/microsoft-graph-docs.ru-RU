---
title: 'Клаудкоммуникатионс: Жетпресенцесбюсерид'
description: Получение сведений о присутствии для нескольких пользователей.
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: e06c1403b1d96a42a670f4c6d53c3bf5251d3b8a
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581238"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a>Клаудкоммуникатионс: Жетпресенцесбюсерид

Пространство имен: microsoft.graph

Получение сведений о [присутствии](../resources/presence.md) для нескольких пользователей.

## <a name="permissions"></a>Permissions
Для вызова этих API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий)                  |
| :-------------- | :----------------------------------------------------------- |
| Делегированное (рабочая или учебная учетная запись)     | Presence.Read.All                         |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается.                         |
| Приложение                            | Не поддерживается.                                  |

> **Примечание.**
> * Для каждого запроса API поддерживается не более 650 идентификаторов пользователей.
> * Максимальная частота запросов для этого API составляет 1500 запросов API в течение 30-секундного периода на приложение для каждого клиента.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |
|Content-Type | application/json. Обязательный. |


## <a name="request-body"></a>Текст запроса

В тексте запроса укажите объект JSON со следующим параметром.

| Параметр      | Тип    |Описание|
|:---------------|:--------|:----------|
|ids|Коллекция String|Идентификаторы объектов пользователя.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [присутствия](../resources/presence.md) в тексте отклика.


## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже показан пример запроса.

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

---

### <a name="response"></a>Отклик
Ниже показан пример отклика.

> **Примечание:** Объекты ответа могут быть сокращены для удобочитаемости. При фактическом вызове будут возвращены все свойства.

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


