---
title: тип ресурса serviceHealthIssuePost
description: Представляет историческую должность в проблеме со здоровьем службы.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 3216f0a4510b6dd66a0ce5c7a96834dbf289b378
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126676"
---
# <a name="servicehealthissuepost-resource-type"></a>тип ресурса serviceHealthIssuePost

Пространство имен: microsoft.graph

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

