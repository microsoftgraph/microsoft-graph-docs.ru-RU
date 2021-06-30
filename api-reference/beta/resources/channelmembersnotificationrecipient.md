---
title: тип ресурса channelMembersNotificationRecipient
description: Представляет получателя уведомления, отправленного в канале Microsoft Teams действий. Получатель состоит из участников канала.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 821d4f2ee41c15cb93cd3d53b9af9cf1e63db97b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211403"
---
# <a name="channelmembersnotificationrecipient-resource-type"></a>тип ресурса channelMembersNotificationRecipient

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет получателя уведомления, отправленного в канале Microsoft Teams действий. Получатель состоит из участников канала.

Наследует [от teamworkNotificationRecipient](teamworknotificationrecipient.md).

## <a name="properties"></a>Свойства
| Свойство  | Тип   | Описание                                            |
| :-------- | :----- | :----------------------------------------------------- |
| teamId    | String | Идентификатор группы, под которым находится канал. |
| channelId | String | Идентификатор канала.                              |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelMembersNotificationRecipient"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.channelMembersNotificationRecipient",
  "teamId": "String",
  "channelId": "String"
}
```
