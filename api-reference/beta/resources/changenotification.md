---
title: Тип ресурса changeNotification
description: Представляет уведомление об изменении, отправленного абоненту.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 9099c2599f63a117e4f963143cfb8570ef6aee46
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335292"
---
# <a name="changenotification-resource-type"></a>Тип ресурса changeNotification

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет уведомление, отправленные абоненту. Все свойства этого ресурса являются только для чтения.

Подробности см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| changeType | changeType | Указывает тип изменения, которое поднимет уведомление об изменении. Поддерживаемые значения: `created`, `updated`, `deleted`. Обязательный элемент. |
| clientState | string | Значение свойства **clientState** , отправленного в запросе подписки (если таково). Максимальная длина: 255 символов. Клиент может проверить, пришло ли уведомление об изменении из службы, сравнивая значения свойства **clientState** . Значение свойства **clientState** , отправленного с подпиской, сравнивается со значением свойства **clientState** , полученного с каждым уведомлением об изменении. Необязательное свойство. |
| encryptedContent | [changeNotificationEncryptedContent](changenotificationencryptedcontent.md) | (Предварительный просмотр) Зашифрованное содержимое, прикрепленное с уведомлением об изменении. Только если **шифрованиеCertificate** и **includeResourceData** было определено во время запроса подписки и если ресурс поддерживает его. Необязательное свойство. |
| id | string | Уникальный ID для уведомления. Необязательное свойство. |
| lifecycleEvent | lifecycleEventType | Тип уведомления жизненного цикла, если текущее уведомление является уведомлением жизненного цикла. Необязательное свойство. Поддерживаемые значения : `missed`, `reauthorizationRequired``subscriptionRemoved`. Необязательное свойство. |
| resource | string | URI ресурса, излучающего уведомление об изменении относительно `https://graph.microsoft.com`. Обязательный элемент. |
| resourceData | [resourceData](resourcedata.md) | Содержимое этого свойства зависит от типа связанного с ним ресурса. Необязательное свойство. |
| subscriptionExpirationDateTime | DateTimeOffset | Время окончания срока действия подписки. Обязательный элемент. |
| subscriptionId | Guid | Уникальный идентификатор подписки, которая породила уведомление. Обязательный элемент.|
| tenantId | Guid | Уникальный идентификатор клиента, из которого возникло уведомление об изменении. Обязательный.|

## <a name="relationships"></a>Связи

Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.changeNotification"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.changeNotification",
  "id": "String (identifier)",
  "subscriptionId": "Guid",
  "subscriptionExpirationDateTime": "String (timestamp)",
  "clientState": "String",
  "changeType": "String",
  "resource": "String",
  "tenantId": "Guid",
  "encryptedContent": {
    "@odata.type": "microsoft.graph.changeNotificationEncryptedContent"
  },
  "lifecycleEvent": "String",
  "resourceData": {
    "@odata.type": "microsoft.graph.resourceData"
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


