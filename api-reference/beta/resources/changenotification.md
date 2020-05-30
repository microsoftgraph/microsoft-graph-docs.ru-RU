---
title: Тип ресурса Чанженотификатион
description: Представляет уведомление об изменении, отправляемое подписчику.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 117bd9c6ab25ca1db00233a15b8d984f6bb512a4
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/30/2020
ms.locfileid: "44430615"
---
# <a name="changenotification-resource-type"></a>Тип ресурса Чанженотификатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет уведомление, отправленное подписчику.

Дополнительные сведения см. [в статье Использование API Microsoft Graph для получения уведомлений об изменениях](webhooks.md).

## <a name="methods"></a>Методы

Отсутствуют.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| changeType | string | Указывает тип изменения, которое вызовет уведомление об изменении. Поддерживаемые значения: `created`, `updated`, `deleted`. Обязательный элемент. |
| clientState | string | Значение свойства **clientState** , указанное в запросе на подписку (при наличии). Максимальная длина: 255 символов. Клиент может проверить, что уведомление об изменении поступило из службы, сравнив значение свойства **clientState** , отправленного с подпиской, со значением свойства **clientState** , полученного с каждым уведомлением об изменении. Необязательное свойство. |
| енкриптедконтент | [Microsoft. Graph. Чанженотификатионенкриптедконтент](changenotificationencryptedcontent.md) | Просмотреть Зашифрованное содержимое, связанное с уведомлением об изменении. Предоставляется только в том случае, если **енкриптионцертификате** и **инклудересаурцедата** определены во время запроса на подписку, и если он поддерживается ресурсом. Необязательный |
| лифецикливент | string | Тип уведомления о жизненном цикле, если текущее уведомление является уведомлением жизненного цикла. Необязательное свойство. Поддерживаемые значения: `missed` , `removed` , `reauthorizationRequired` . |
| id | строка | Уникальный идентификатор уведомления. Необязательное свойство. |
| resource | string | URI ресурса, который выдал уведомление об изменении относительно `https://graph.microsoft.com` . Обязательный элемент. |
| resourceData | [Microsoft. Graph. resourceData](resourcedata.md) | Содержимое этого свойства зависит от типа связанного с ним ресурса. Обязательный элемент. |
| sequenceNumber | int | Можно использовать, чтобы получать уведомления по порядку. Необязательное свойство. |
| subscriptionExpirationDateTime | [дата и время](https://tools.ietf.org/html/rfc3339) | Время окончания срока действия подписки. Обязательный элемент. |
| subscriptionId | string | Уникальный идентификатор подписки, создавшей уведомление. |
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
  // Other properties typical in a resource change notification
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
