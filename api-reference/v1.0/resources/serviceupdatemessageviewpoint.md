---
title: тип ресурса serviceUpdateMessageViewpoint
description: Представляет данные точек представления пользователей для службыUpdateMessage".
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 080d739d2111d383c5e5d7cf8ec3ec510e1cb5ba
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108767"
---
# <a name="serviceupdatemessageviewpoint-resource-type"></a>тип ресурса serviceUpdateMessageViewpoint

Пространство имен: microsoft.graph

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
