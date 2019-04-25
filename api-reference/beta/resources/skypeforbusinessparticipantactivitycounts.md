---
title: Тип ресурса СкипефорбусинесспартиЦипантактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: de86c49da34c9af48478a912a6ab042a354a7bf5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568091"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a>Тип ресурса СкипефорбусинесспартиЦипантактивитикаунтс

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| im                | Int64  |
| Audiovideohttp        | Int64  |
| Аппшаринг        | Int64  |
| web               | Int64  |
| dialInOut3rdParty | Int64  |
| Репортрефрешдате | Дата   |
| reportDate        | Дата   |
| Репортпериод      | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
