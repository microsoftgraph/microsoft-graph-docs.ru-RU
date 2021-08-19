---
title: тип ресурса serviceHealthIssuePost
description: Представляет историческую должность в проблеме со здоровьем службы.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: a53f09c6fc32de1c65e52e2554aa89b634f2b0e3
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266900"
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

## <a name="relationships"></a>Связи
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

