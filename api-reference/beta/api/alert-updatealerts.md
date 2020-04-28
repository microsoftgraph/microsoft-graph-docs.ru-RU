---
title: 'Предупреждение: Упдатеалертс'
description: Обновление нескольких оповещений в одном запросе вместо нескольких запросов.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 684c96aeb0f297c783343001a1ab00bc82f9da63
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441636"
---
# <a name="alert-updatealerts"></a>Предупреждение: Упдатеалертс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление нескольких оповещений в одном запросе вместо нескольких запросов.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |   SecurityEvents.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Для приложений | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {code} |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами. У каждой сущности должны быть свойства **ID** и **вендоринформатион** . Для получения дополнительных сведений о свойствах, которые можно обновить, ознакомьтесь со статьей [Обновление оповещения](alert-update.md).

| Параметр    | Тип        | Описание |
|:-------------|:------------|:------------|
|значение|Коллекция [alert](../resources/alert.md)| Коллекция оповещений, которые необходимо обновить. Каждая сущность должна иметь **идентификатор**, **вендоринформатион**и другие редактируемые свойства, которые необходимо обновить.|

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод `200, OK` возвращает код отклика и объект коллекции [Alerts](../resources/alert.md) в тексте отклика.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "alert_updatealerts",
   "isCollection": "true"
}-->

```http
POST https://graph.microsoft.com/beta/security/alerts/updateAlerts
Content-type: application/json

{
  "value": [
    {
      "assignedTo": "String",
      "closedDateTime": "String (timestamp)",
      "comments": ["String"],
      "feedback": {"@odata.type": "microsoft.graph.alertFeedback"},
      "id": "String (identifier)",
      "status": {"@odata.type": "microsoft.graph.alertStatus"},
      "tags": ["String"],
      "vendorInformation":
        {
          "provider": "String",
          "vendor": "String"
        }
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/alert-updatealerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/alert-updatealerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/alert-updatealerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> [!NOTE]
> Объект Response, показанный здесь, может быть укорочен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert: updateAlerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
