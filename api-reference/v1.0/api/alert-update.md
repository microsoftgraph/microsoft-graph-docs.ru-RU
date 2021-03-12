---
title: Обновление оповещения
description: Обновление свойства редактируемого **оповещения** в любом интегрированном решении, чтобы синхронизировать состояние оповещений и назначения между решениями. Этот метод обновляет любое решение, которое имеет запись ссылаемого ID оповещения.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 92edfc5e312b56170aa1c8924dad6b2b48970839
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721427"
---
# <a name="update-alert"></a>Обновление оповещения

Пространство имен: microsoft.graph

Обновление свойства редактируемого **оповещения** в любом интегрированном решении, чтобы синхронизировать состояние оповещений и назначения между решениями. Этот метод обновляет любое решение, которое имеет запись ссылаемого ID оповещения.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | SecurityEvents.ReadWrite.All        |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                      |
| Приложение                            | SecurityEvents.ReadWrite.All        |

## <a name="http-request"></a>HTTP-запрос

> **Примечание:** Необходимо включить **в** качестве параметра и поставщика ID оповещений, содержащего и `provider` с помощью этого `vendor` метода.

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание              |
|:--------------|:-------------------------|
| Авторизация | Bearer {код}. Обязательно. |
| Prefer        | return=representation. Необязательное свойство.   |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON значений для соответствующих полей, которые должны быть обновлены. Тело должно **содержать** свойство **vendorInformation** с допустимым и `provider` `vendor` полями. В следующей таблице перечислены поля, которые можно обновить для оповещения. Значения для существующих свойств, не включенных в тело запроса, не изменятся. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство          | Тип                                                                   | Описание |
|:------------------|:-----------------------------------------------------------------------|:--|
| assignedTo        | String                                                                 | Имя аналитика, на которое назначено оповещение для проверки, исследования или восстановления. |
| closedDateTime    | DateTimeOffset                                                         | Время закрытия оповещения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| comments          | Коллекция String                                                      | Аналитик комментирует оповещение (для управления оповещениями клиентов). Этот метод может обновлять поле комментариев только с помощью следующих значений: `Closed in IPC` , `Closed in MCAS` . |
| feedback          | alertFeedback                                                          | Отзыв аналитика об оповещении. Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`. |
| status            | alertStatus                                                            | Оповещение состояния жизненного цикла (этап). Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`. |
| tags              | Коллекция объектов string                                                      | Метки, вызываемые пользователем, которые можно применить к оповещению и могут служить условиями фильтра (например, "HVA", "SAW"). |
| vendorInformation | [securityVendorInformation](../resources/securityvendorinformation.md) | Сложный тип, содержащий подробные сведения о безопасности продавца продукта или услуги, поставщика субпоставщика (например, продавец = Майкрософт; поставщик = ATP в Защитнике Windows; субпоставщик = AppLocker). **Требуются поля поставщика и поставщика.** |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

Если используется необязательный заголовок запроса, метод возвращает код ответа и обновленный объект оповещения `200 OK` в тексте [](../resources/alert.md) ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-request-without-prefer-header"></a>Пример 1. Запрос без загона Prefer

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-java-snippets.md)]
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

### <a name="example-2-request-with-prefer-header"></a>Пример 2. Запрос с помощью загона Prefer

#### <a name="request"></a>Запрос

В следующем примере показан запрос, который включает заглавную `Prefer` головку запроса.

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

Ниже приводится пример ответа, когда используется необязательный `Prefer: return=representation` заглавной запрос.

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

