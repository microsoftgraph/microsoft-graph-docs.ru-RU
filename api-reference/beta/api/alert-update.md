---
title: Обновление оповещения
description: Обновление редактируемого свойства оповещения в любом интегрированном решении для обеспечения синхронизации состояния и назначений оповещений между решениями.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 3ad81e698c43e8863d3081d6995fc29b1b9a9dc3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258543"
---
# <a name="update-alert"></a>Обновление оповещения

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление редактируемого свойства **оповещения** в любом интегрированном решении для обеспечения синхронизации состояния и назначений оповещений между решениями. Этот метод обновляет любое решение, имеющее запись идентификатора оповещения, на который указывает ссылка.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |   SecurityEvents.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Для приложений | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

> **Примечание:** Необходимо включить идентификатор **оповещения** в качестве параметра и вендоринформатион, содержащего метод `provider` и `vendor` с этим методом.
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Bearer {код}. Обязательно.|
|Prefer | Возврат = представление |

## <a name="request-body"></a>Тело запроса

В тексте запроса добавьте представление значений в формате JSON для соответствующих полей, которые необходимо обновить. Текст **должен** содержать `vendorInformation` свойство Valid `provider` и `vendor` Fields. В следующей таблице перечислены поля, которые можно обновить для оповещения. Значения для существующих свойств, не включенных в текст запроса, не изменятся. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|assignedTo|String|Имя аналитика, которому назначено оповещение для рассмотрения, исследования или исправления.|
|closedDateTime|DateTimeOffset|Время закрытия оповещения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|comments|Коллекция String|Комментарии аналитика в оповещении (для управления оповещениями клиентов).|
|feedback|Перечисление Алертфидбакк|Отзыв аналитика об оповещении. Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.|
|status|Перечисление Алертстатус|Состояние жизненного цикла оповещений (Stage). Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.|
|tags|Коллекция String|Определяемые пользователями метки, которые могут быть применены к оповещению и могут использоваться в качестве условий фильтрации (например, "Хва", "показано").|
|vendorInformation |[securityVendorInformation](../resources/securityvendorinformation.md)|Сложный тип, содержащий подробные сведения о безопасности продавца продукта или услуги, поставщика субпоставщика (например, продавец = Майкрософт; поставщик = ATP в Защитнике Windows; субпоставщик = AppLocker). **Требуются поля поставщика и поставщика.**|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

Если используется заголовок необязательного запроса, метод возвращает код `200 OK` отклика и обновленный объект [Alert](../resources/alert.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-request-without-prefer-header"></a>Пример 1: запрос без верхнего колонтитула

#### <a name="request"></a>Запрос

Ниже приведен пример запроса без `Prefer` заголовка.
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Отклик

Ниже представлен пример успешного отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/update_alert-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_alert-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_alert-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-request-with-prefer-header"></a>Пример 2: запрос с заголовком предпочтения

#### <a name="request"></a>Запрос

В приведенном ниже примере показан запрос, включающий заголовок `Prefer` запроса.

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика при использовании заголовка необязательного `Prefer: return=representation` запроса.

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
