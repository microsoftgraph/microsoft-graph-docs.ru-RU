---
title: Обновление объекта calendarGroup.
description: Обновление свойств объекта calendarGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: dc1e31227bd31c073ffe86166c8626b0b24e9bb5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864998"
---
# <a name="update-calendargroup"></a>Обновление объекта calendarGroup.

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта calendarGroup.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Calendars.ReadWrite                         |
| Делегированные (личная учетная запись Майкрософт) | Calendars.ReadWrite                         |
| Для приложений                            | Calendars.ReadWrite                         |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                       |
| :------------ | :-------------------------- |
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство | Тип   | Описание     |
| :------- | :----- | :-------------- |
| name     | String | Имя группы. |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [calendarGroup](../resources/calendargroup.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик

Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
