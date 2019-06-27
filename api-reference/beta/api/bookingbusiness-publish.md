---
title: 'Букингбусинесс: публикация'
description: Сделайте страницу планирования для этого бизнеса доступной внешним клиентам.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f533a9759db0b2e47c57b1ab55282804f4acf235
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258004"
---
# <a name="bookingbusiness-publish"></a>Букингбусинесс: публикация

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сделайте страницу планирования для этого бизнеса доступной внешним клиентам.

Задайте для свойства **публикации** значение true, а свойству **публикурл** — URL-адрес страницы планирования.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Резервирования. Manage. ALL   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.   |
|Для приложений | Не поддерживается.  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
