---
title: Удаление timeOffReason
description: Пометить timeOffReason как неактивное, задав свойство isActive.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4a53a677187373105e6a6b1cd3b884c6aa5e928e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787431"
---
# <a name="delete-timeoffreason"></a>Удаление timeOffReason

Пространство имен: microsoft.graph

[Пометить timeOffReason](../resources/timeoffreason.md) как неактивное, задав **свойство isActive.** Каждая команда должна включать по крайней мере одну причину времени.

Этот метод не удаляет указанный экземпляр [timeOffReason.](../resources/timeoffreason.md) [Экземпляры timeOffItem,](../resources/timeoffitem.md) которые были назначены по этой причине, остаются назначены по этой причине.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Schedule.ReadWrite.All, Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Schedule.ReadWrite.All |

> **Примечание**. Этот API поддерживает разрешения администратора. Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffreason-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Marks a timeOffReason as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

