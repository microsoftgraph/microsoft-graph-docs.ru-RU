---
title: тип ресурса serviceHealthIssuePost
description: Представляет историческую должность в проблеме со здоровьем службы.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c005beb7b27956cad6f42c7251bb15be7024415c5096d8f012a88049534b6cad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243038"
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

