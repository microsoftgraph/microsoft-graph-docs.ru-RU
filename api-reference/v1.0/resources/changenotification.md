---
title: Тип ресурса changeNotification
description: Представляет уведомление об изменении, отправленного абоненту.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 2d0563a77710b5553f9ace2d58a8c695259a81cf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104252"
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
| changeType | changeType | Указывает тип изменения, которое поднимет уведомление об изменении. Поддерживаемые значения: `created`, `updated`, `deleted`. Обязательный. |
| clientState | string | Значение свойства **clientState,** отправленного в запросе подписки (если таково). Максимальная длина: 255 символов. Клиент может проверить, пришло ли уведомление об изменении из службы, сравнивая значения свойства **clientState.** Значение свойства **clientState,** отправленного с подпиской, сравнивается со значением свойства **clientState,** полученного с каждым уведомлением об изменении. Необязательное. |
| encryptedContent | [changeNotificationEncryptedContent](changenotificationencryptedcontent.md) | (Предварительный просмотр) Зашифрованное содержимое, прикрепленное с уведомлением об изменении. Только если **шифрованиеCertificate** и **includeResourceData** было определено во время запроса подписки и если ресурс поддерживает его. Необязательное. |
| id | string | Уникальный ID для уведомления. Необязательное. |
| lifecycleEvent | lifecycleEventType| Тип уведомления жизненного цикла, если текущее уведомление является уведомлением жизненного цикла. Необязательное. Поддерживаемые значения `missed` : `subscriptionRemoved` , `reauthorizationRequired` . |
| resource | string | URI ресурса, излучающего уведомление об изменении относительно `https://graph.microsoft.com` . Обязательное. |
| resourceData | [resourceData](resourcedata.md) | Содержимое этого свойства зависит от типа связанного с ним ресурса. Обязательное. |
| subscriptionExpirationDateTime | DateTimeOffset | Время окончания срока действия подписки. Обязательный. |
| subscriptionId | GUID | Уникальный идентификатор подписки, которая породила уведомление. |
| tenantId | GUID | Уникальный идентификатор клиента, из которого возникло уведомление об изменении. |

## <a name="relationships"></a>Отношения

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

