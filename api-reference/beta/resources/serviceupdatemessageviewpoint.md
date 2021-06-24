---
title: тип ресурса serviceUpdateMessageViewpoint
description: Представляет данные точек представления пользователей для службыUpdateMessage".
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c84a07691c2507a9ff74102ac6f4b1675cb382e7
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109223"
---
# <a name="serviceupdatemessageviewpoint-resource-type"></a>тип ресурса serviceUpdateMessageViewpoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет данные точек представления пользователей для [службыUpdateMessage.](../resources/serviceupdatemessage.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isArchived|Boolean|Указывает, архивировать ли сообщение пользователь.|
|isFavorited|Boolean|Указывает, отметил ли пользователь сообщение как избранное.|
|isRead|Boolean|Указывает, читал ли пользователь сообщение.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceUpdateMessageViewpoint",
  "isRead": "Boolean",
  "isArchived": "Boolean",
  "isFavorited": "Boolean"
}
```