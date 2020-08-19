---
title: Тип ресурса СкипефорбусинесспартиЦипантактивитюсеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: e53ef85ce3fbe0be2a36adc218d565bdb78f64a0
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811072"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a>Тип ресурса СкипефорбусинесспартиЦипантактивитюсеркаунтс

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| im                | Int64  |
| Audiovideohttp        | Int64  |
| аппшаринг        | Int64  |
| web               | Int64  |
| dialInOut3rdParty | Int64  |
| репортрефрешдате | Дата   |
| reportDate        | Дата   |
| репортпериод      | String |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```json
{
  "im": 1024,
  "audioVideo": 196,
  "appSharing": 196,
  "web": 196,
  "dialInOut3rdParty": 196,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
