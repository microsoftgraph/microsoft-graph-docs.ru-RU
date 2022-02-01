---
title: Перечисление оповещений
description: Получение списка объектов alert.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 116f965baa0e64b55c4b748378165b0004c98a15
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290772"
---
# <a name="list-alerts"></a>Перечисление оповещений

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [alert](../resources/alert.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  SecurityEvents.Read.All, SecurityEvents.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Приложение | SecurityEvents.Read.All, SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает указанные ниже [параметры запросов OData](/graph/query-parameters) для настройки отклика.

- `$count`
- `$orderby`
- `$select`
- `$skip`
- `$top` – Возвращает объединенные лучшие результаты от каждого поставщика API безопасности.
- `$filter`

В таблице ниже перечислены ключевые слова `$filter` по именам поставщиков. Несмотря на то, что некоторые из этих продуктов поменяли название в ходе ребрендинга, API еще не обновлен. Ключевые слова фильтра будут продолжать использовать устаревшие названия до дальнейшего уведомления. Подробности см. в [журнале изменений](https://developer.microsoft.com/graph/changelog).

| Наименование поставщика      |ключевое слово $filter|
|:----------|:----------|
| Microsoft Defender для удостоверений | Расширенная защита от угроз Azure | 
| Центр безопасности Azure | ASC |
| Microsoft Defender for Cloud Apps | MCAS |
| Защита идентификации Azure Active Directory | IPC |
| Azure Sentinel | Azure Sentinel |
| Microsoft Defender для конечной точки | ATP в Защитнике Windows |
| Office 365 |  В настоящее время не поддерживается. |

Чтобы возвратить альтернативный набор свойств, используйте параметр запроса OData `$select`, чтобы указать нужный набор свойств **alert**.  Например, чтобы вернуть свойства **assignedTo**, **category** и **severity**, добавьте в свой запрос следующее: `$select=assignedTo,category,severity`.

> **Примечание.** Параметр запроса OData `$top` имеет ограничение в 1000 оповещений. В первый запрос GET рекомендуется включить только параметр `$top`, но не параметр `$skip`. Для разбивки на страницы можно использовать параметр `@odata.nextLink`. Если требуется применить параметр `$skip`, он имеет ограничение в 500 оповещений. Например, `/security/alerts?$top=10&$skip=500` вернет код отклика `200 OK`, но `/security/alerts?$top=10&$skip=501` вернет код отклика `400 Bad Request`. Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {код}. Обязательно.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода. Текст запроса будет игнорироваться.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов **alert** в тексте отклика. Если от поставщика возвращается код состояния, отличный от 2xx или 404, или истекло время ожидания поставщика, откликом будет код состояния `206 Partial Content` с ответом поставщика в заголовке предупреждения. Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/alerts
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-alerts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-alerts-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-alerts-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


