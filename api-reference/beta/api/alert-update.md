---
title: обновление оповещения.
description: Обновите редактируемых свойств оповещения в любой интегрированное решение для синхронизации состояний оповещений и назначений в решениях.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fc0bc88dad83024d3da2d6f2adf3f16288719cb2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517416"
---
# <a name="update-alert"></a>обновление оповещения.

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите свойство редактируемого **оповещения** в любой интегрированное решение для синхронизации состояний оповещений и назначений в решениях. Этот метод обновляет все решения, имеет запись оповещения, указанный идентификатор.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |   SecurityEvents.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Для приложений | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

> **Примечание:** Необходимо указать код **оповещение о** как параметр и содержащий vendorInformation `provider` и `vendor` с помощью этого метода.
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Authorization  | В заголовке указывается "Bearer {код}". Обязательный.|
|Prefer | Возвращает = представление |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите представление JSON значений для соответствующие поля, которые должны обновляться. Текст, **должны** содержать `vendorInformation` свойство с допустимыми `provider` и `vendor` полей. В следующей таблице приведены поля, которые могут быть обновлены для оповещения. Значения для существующих свойств, которые не включены в тексте запроса остаются без изменений. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|AssignedTo|String|Имя аналитик оповещение будет назначен для рассмотрения исследования и исправления.|
|closedDateTime|DateTimeOffset|Время закрытия оповещение. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|comments|Коллекция String|Комментарии аналитик оповещения (для управления предупреждениями клиента).|
|Отзывы|Перечисление alertFeedback|Отзыв аналитик на оповещение. Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.|
|status|Перечисление alertStatus|Состояние оповещений жизненного цикла (рабочей области). Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.|
|tags|Коллекция String|Определяемые пользователем меток, которые могут применяться к оповещения и может выступать в качестве условий фильтра (например, «HVA», «ЗАФИКСИРОВАЛА).|
|vendorInformation |[securityVendorInformation](../resources/securityvendorinformation.md)|Сложный тип, содержащий сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker). **Поставщик и поставщика поля являются обязательными.**|

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

Если используется запрос на необязательный заголовок, метод возвращает `200 OK` код ответа и объект обновленные [оповещения](../resources/alert.md) в теле ответа.

## <a name="example-1"></a>Пример 1

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
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

### <a name="response"></a>Ответ

Ниже представлен пример успешного отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a>Пример 2

### <a name="request"></a>Запрос

В следующем примере показан запрос, который включает в себя `Prefer` заголовка запроса.

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

### <a name="response"></a>Ответ

Ниже приведен пример ответа при Дополнительно `Prefer: return=representation` используется заголовка запроса.

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
    "Error: /api-reference/beta/api/alert-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
