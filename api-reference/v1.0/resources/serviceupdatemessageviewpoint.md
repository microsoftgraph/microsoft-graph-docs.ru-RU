---
title: тип ресурса serviceUpdateMessageViewpoint
description: Представляет данные точек представления пользователей для службыUpdateMessage".
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 57d5bf64069d0799514eafc78fbfb5d221ccf82b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58250893"
---
# <a name="serviceupdatemessageviewpoint-resource-type"></a>тип ресурса serviceUpdateMessageViewpoint

Пространство имен: microsoft.graph

Представляет данные точек представления пользователей для [службыUpdateMessage.](../resources/serviceupdatemessage.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isArchived|Boolean|Указывает, архивировать ли сообщение пользователь.|
|isFavorited|Логический|Указывает, отметил ли пользователь сообщение как избранное.|
|isRead|Boolean|Указывает, читал ли пользователь сообщение.|

## <a name="relationships"></a>Связи
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