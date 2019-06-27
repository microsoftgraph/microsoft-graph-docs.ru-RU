---
title: Получение Рискюсер
description: Получение свойств и связей объекта **рискюсер** .
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cf7ed70149a5e377fe7c80eaa451b27f44246324
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267097"
---
# <a name="get-riskyuser"></a>Получение Рискюсер

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение свойств и связей объекта **рискюсер** .

>**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | IdentityRiskyUser.Read.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | IdentityRiskyUser.Read.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
```


## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Workbook-Session-Id  | Идентификатор сеанса книги, который определяет, сохраняются ли изменения. Необязательно.|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рискюсер](../resources/riskyuser.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isGuest": true,
  "isProcessing": true,
  "isDeleted": true,
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk",
  "userDisplayName": "Alex Wilbur",
  "userPrincipalName": "alexw@contoso.com"
}
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_riskyuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_riskyuser-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_riskyuser-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

