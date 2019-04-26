---
title: Перечисление оповещений
description: Получение списка объектов оповещений.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: ab9ec3c42b0a46279e43660e241fb3cde52e83a9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322700"
---
# <a name="list-alerts"></a>Перечисление оповещений

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [оповещений](../resources/alert.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Приложение | Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL |

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

Этот метод поддерживает следующие [Параметры запроса OData](/graph/query-parameters) для настройки отклика:

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- `$top`Возвращает сводные результаты из каждого поставщика API безопасности.

Чтобы получить альтернативный набор свойств, используйте параметр запроса `$select` OData, чтобы указать требуемый набор свойств **оповещения** .  Например, чтобы вернуть свойства **assignedTo**, **Category**и **Severity** , добавьте в запрос следующее: `$select=assignedTo,category,severity`.

> **Примечание:** `$top` ограничено 1000 оповещений, а их `$top`  +  `$skip` комбинация не может превышать 6000. Например, `/security/alerts?$top=10&$skip=5990` возвращает код `200 OK` отклика, но `/security/alerts?$top=10&$skip=5991` возвратит код `400 Bad Request` отклика.  Дополнительные сведения см. в разделе [ответ об ошибках API безопасности Microsoft Graph](../resources/security-error-codes.md).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Authorization  | Bearer {Code}. Обязательно.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода. Текст запроса будет игнорироваться.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов **Alert** в тексте отклика. Если поставщик возвращает код состояния, отличный от 2xx или 404, или если время ожидания поставщика истекло, ответ будет кодом `206 Partial Content` состояния с ответом поставщика в заголовке предупреждения. Дополнительные сведения см. в разделе [ответ об ошибках API безопасности Microsoft Graph](../resources/security-error-codes.md).

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
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
  "suppressions": []
}
-->
