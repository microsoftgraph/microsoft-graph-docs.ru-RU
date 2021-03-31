---
title: Тип ресурса changeNotification
description: Представляет уведомление об изменении, отправленного абоненту.
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 613e7f7bc29f3fbf54db357de7d203d912056acc
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469355"
---
# <a name="changenotification-resource-type"></a>Тип ресурса changeNotification

Пространство имен: microsoft.graph

Представляет уведомление, отправленные абоненту.

Подробности см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| changeType | string | Указывает тип изменения, которое поднимет уведомление об изменении. Поддерживаемые значения: `created`, `updated`, `deleted`. Обязательное. |
| clientState | string | Значение свойства **clientState,** отправленного в запросе подписки (если таково). Максимальная длина: 255 символов. Клиент может проверить, пришло ли уведомление об изменении из службы, сравнивая значения свойства **clientState.** Значение свойства **clientState,** отправленного с подпиской, сравнивается со значением свойства **clientState,** полученного с каждым уведомлением об изменении. Необязательное свойство. |
| lifecycleEvent | Строка | Тип уведомления жизненного цикла, если текущее уведомление является уведомлением жизненного цикла. Необязательное свойство. Поддерживаемые значения `missed` : `removed` , `reauthorizationRequired` . |
| encryptedContent | [microsoft.graph.changeNotificationEncryptedContent](changenotificationencryptedcontent.md) | (Предварительный просмотр) Зашифрованное содержимое, прикрепленное с уведомлением об изменении. Только если **шифрованиеCertificate** и **includeResourceData** было определено во время запроса подписки и если ресурс поддерживает его. Необязательное свойство. |
| id | string | Уникальный ID для уведомления. Необязательное свойство. |
| resource | string | URI ресурса, излучающего уведомление об изменении относительно `https://graph.microsoft.com` . Обязательное. |
| resourceData | [microsoft.graph.resourceData](resourcedata.md) | Содержимое этого свойства зависит от типа связанного с ним ресурса. Обязательное. |
| subscriptionExpirationDateTime | [дата и время](https://tools.ietf.org/html/rfc3339) | Время окончания срока действия подписки. Обязательное. |
| subscriptionId | строка | Уникальный идентификатор подписки, которая породила уведомление. |
| tenantId | guid | Уникальный идентификатор клиента, из которого возникло уведомление об изменении. |

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

