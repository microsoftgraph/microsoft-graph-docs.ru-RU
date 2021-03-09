---
title: тип ресурса teamworkHostedContent
description: Представляет богатый контент, который организован Microsoft Teams
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 93b3b4fc817c1fe3aa3973a112b9cf887c825b6e
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578862"
---
# <a name="teamworkhostedcontent-resource-type"></a>тип ресурса teamworkHostedContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет богатый контент, например изображения и фрагменты кода в Microsoft Teams. Для богатого [контента в сообщениях](chatMessage.md)каналов и чатов см. [в странице chatMessageHostedContent.](chatMessageHostedContent.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|contentBytes|Двоичный|Только напишите. Bytes for the hosted content (such as images).|
|contentType|String|Только напишите. Тип контента, например изображение/png, изображение/jpg.|
|id|String|ID хост-контента.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkHostedContent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHostedContent",
  "id": "String (identifier)",
  "contentBytes": "Binary",
  "contentType": "String"
}
```

