---
title: тип ресурса serviceHealthIssuePost
description: Представляет историческую должность в проблеме со здоровьем службы.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 910236d2059f951169bea314a0b38ae2516b1918
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107840"
---
# <a name="servicehealthissuepost-resource-type"></a>тип ресурса serviceHealthIssuePost

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет исторический пост в проблеме [со здоровьем службы.](../resources/servicehealthissue.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Опубликовано время публикации.|
|description|[itemBody](../resources/itembody.md)|Содержимое сообщения о проблеме службы.|
|postType|postType|Тип столба исторической публикации службы. Возможные значения: `regular`, `quick`, `strategic`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceHealthIssuePost"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealthIssuePost",
  "createdDateTime": "String (timestamp)",
  "postType": "String",
  "description": {
    "@odata.type": "microsoft.graph.itemBody"
  }
}
```

