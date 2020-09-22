---
title: Тип ресурса changeNotification
description: Представляет уведомление об изменении, отправляемое подписчику.
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: a1be7569f6fb7f96b28d34f8e319df78f14a6ae9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037901"
---
# <a name="changenotification-resource-type"></a>Тип ресурса changeNotification

Пространство имен: microsoft.graph

Представляет уведомление, отправленное подписчику.

Дополнительные сведения см. [в статье Использование API Microsoft Graph для получения уведомлений об изменениях](webhooks.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| changeType | string | Указывает тип изменения, которое вызывает уведомление об изменении. Поддерживаемые значения: `created`, `updated`, `deleted`. Обязательно. |
| clientState | string | Значение свойства **clientState** , которое отправляется в запросе на подписку (при наличии). Максимальная длина: 255 символов. Клиент может проверить, поступило ли уведомление об изменении из службы, сравнив значения свойства **clientState** . Значение свойства **clientState** , отправляемого с подпиской, сравнивается со значением свойства **clientState** , полученного при каждом уведомлении об изменении. Необязательный параметр. |
| id | string | Уникальный идентификатор уведомления. Необязательный параметр. |
| resource | string | URI ресурса, который выдал уведомление об изменении относительно `https://graph.microsoft.com` . Обязательно. |
| resourceData | [Microsoft. Graph. resourceData](resourcedata.md) | Содержимое этого свойства зависит от типа связанного с ним ресурса. Обязательно. |
| subscriptionExpirationDateTime | [дата и время](https://tools.ietf.org/html/rfc3339) | Время окончания срока действия подписки. Обязательно. |
| subscriptionId | строка | Уникальный идентификатор подписки, создавшей уведомление. |
| tenantId | кодом | Уникальный идентификатор клиента, с которого поступило уведомление об изменении. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotification"
}-->

```json
{
  "subscriptionId": "76222963-cc7b-42d2-882d-8aaa69cb2ba3",
  "changeType": "created",
  "clientState": "client state provided when creating subscription",
  "id": "15ee1d1f-af7b-42d9-885b-9d00db065dd9",
  "tenantId": "2c937fad-a8a7-496c-b0e4-bf77dcc7eb2a",
  "subscriptionExpirationDateTime": "2020-04-12T23:20:50.52Z",
  "resource": "teams('d29828b8-c04d-4e2a-b2f6-07da6982f0f0')/channels('19:f127a8c55ad949d1a238464d22f0f99e@thread.skype')/messages('1565045424600')/replies('1565047490246')",
  "resourceData": {
    "id": "1565293727947",
    "@odata.type": "#Microsoft.Graph.ChatMessage",
    "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
  }
}
```

<!-- uuid: 15ee1d1f-af7b-42d9-885b-9d00db065dd9
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

