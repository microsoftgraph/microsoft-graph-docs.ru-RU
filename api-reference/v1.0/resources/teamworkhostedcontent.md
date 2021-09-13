---
title: тип ресурса teamworkHostedContent
description: Представляет богатый контент, который Microsoft Teams.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8d53614b4d4f699890be7d244d78f7f1ec01890c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128183"
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

## <a name="relationships"></a>Отношения
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
  "id": "String (identifier)",
  "contentBytes": "Binary",
  "contentType": "String"
}
```
