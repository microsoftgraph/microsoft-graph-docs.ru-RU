---
title: тип ресурса callParticipantInfo
description: Представляет сведения для участника вызова.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 95b0e796092f2e9f2ddf480b586d9e50eead0380
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322707"
---
# <a name="callparticipantinfo-resource-type"></a>тип ресурса callParticipantInfo

Пространство имен: microsoft.graph

Представляет сведения для участника вызова.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|participant|[identitySet](../resources/identityset.md)|Удостоверение участника вызова.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callParticipantInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callParticipantInfo",
  "participant": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

