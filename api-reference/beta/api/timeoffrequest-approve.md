---
title: 'timeOffRequest: утверждение'
description: Утверждение объекта timeoffrequest".
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 291a3e764ebcd84d181b5441405c4579cf798dc2
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787326"
---
# <a name="timeoffrequest-approve"></a>timeOffRequest: утверждение

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Утверждение [timeoffrequest](../resources/timeoffrequest.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Group.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение | Schedule.ReadWrite.All*  |

>\***Важно:** Разрешения приложения в настоящее время доступны только в закрытом режиме и недоступны для общего пользования.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип        | Описание |
|:-------------|:------------|:------------|
|message|String|Настраиваемые сообщения утверждения.|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `200, OK`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

Ниже приводится пример вызова этого API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


