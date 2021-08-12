---
title: тип ресурса teamworkHostedContent
description: Представляет богатый контент, который Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7fca2d17db16e101edb22bd1ddfa31e4234e35ec6817f226209429f6cb97757a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189256"
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
