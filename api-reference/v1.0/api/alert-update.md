---
title: Обновление оповещения
description: Обновление редактируемого свойства **оповещения** в любом интегрированном решении для обеспечения синхронизации состояния и назначений оповещений между решениями. Этот метод обновляет любое решение, имеющее запись идентификатора оповещения, на который указывает ссылка.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: f2fd2f03e85f8a21067f10ff2c5fa76778cc730f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443849"
---
# <a name="update-alert"></a>Обновление оповещения

Обновление редактируемого свойства **оповещения** в любом интегрированном решении для обеспечения синхронизации состояния и назначений оповещений между решениями. Этот метод обновляет любое решение, имеющее запись идентификатора оповещения, на который указывает ссылка.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | SecurityEvents.ReadWrite.All        |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                      |
| Для приложений                            | SecurityEvents.ReadWrite.All        |

## <a name="http-request"></a>HTTP-запрос

> **Примечание:** Необходимо включить идентификатор **оповещения** в качестве параметра и вендоринформатион, содержащего метод `provider` и `vendor` с этим методом.

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание              |
|:--------------|:-------------------------|
| Авторизация | Bearer {код}. Обязательно. |
| Prefer        | Возврат = представление    |

## <a name="request-body"></a>Тело запроса

В тексте запроса добавьте представление значений в формате JSON для соответствующих полей, которые необходимо обновить. Текст **должен** содержать `vendorInformation` свойство Valid `provider` и `vendor` Fields. В следующей таблице перечислены поля, которые можно обновить для оповещения. Значения для существующих свойств, не включенных в текст запроса, не изменятся. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство          | Тип                                                                   | Описание |
|:------------------|:-----------------------------------------------------------------------|:--|
| assignedTo        | String                                                                 | Имя аналитика, которому назначено оповещение для рассмотрения, исследования или исправления. |
| closedDateTime    | DateTimeOffset                                                         | Время закрытия оповещения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. |
| comments          | Коллекция String                                                      | Комментарии аналитика в оповещении (для управления оповещениями клиентов). |
| feedback          | alertFeedback                                                          | Отзыв аналитика об оповещении. Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`. |
| status            | alertStatus                                                            | Состояние жизненного цикла оповещений (Stage). Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`. |
| tags              | Коллекция String                                                      | Определяемые пользователями метки, которые могут быть применены к оповещению и могут использоваться в качестве условий фильтрации (например, "Хва", "показано"). |
| vendorInformation | [securityVendorInformation](../resources/securityvendorinformation.md) | Сложный тип, содержащий подробные сведения о безопасности продавца продукта или услуги, поставщика субпоставщика (например, продавец = Майкрософт; поставщик = ATP в Защитнике Windows; субпоставщик = AppLocker). **Требуются поля поставщика и поставщика.** |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

Если используется заголовок необязательного запроса, метод возвращает код `200 OK` отклика и обновленный объект [Alert](../resources/alert.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-request-without-prefer-header"></a>Пример 1: запрос без верхнего колонтитула

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

### <a name="example-2-request-with-prefer-header"></a>Пример 2: запрос с заголовком предпочтения

#### <a name="request"></a>Запрос

В приведенном ниже примере показан запрос, включающий заголовок `Prefer` запроса.

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика при использовании заголовка необязательного `Prefer: return=representation` запроса.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

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
<!-- {
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
