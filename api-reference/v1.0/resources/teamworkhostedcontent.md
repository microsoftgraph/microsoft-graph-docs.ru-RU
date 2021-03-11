---
title: тип ресурса teamworkHostedContent
description: Представляет богатый контент, на который ведется Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0a4a4d0a553f77766dd4ddb1f68e27b440fdbf2f
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50634329"
---
# <a name="teamworkhostedcontent-resource-type"></a>тип ресурса teamworkHostedContent

Пространство имен: microsoft.graph

Представляет богатый контент, например изображения и фрагменты кода в Microsoft Teams. Для богатого [контента в сообщениях](chatMessage.md)каналов и чатов см. [в странице chatMessageHostedContent.](chatMessageHostedContent.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|contentBytes|Двоичный|Только напишите. Bytes for the hosted content (such as images).|
|contentType|String|Только напишите. Тип контента. sicj as image/png, image/jpg.|
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
