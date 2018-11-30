---
title: Тип ресурса mediaContentRatingIreland
description: Н/Д
ms.openlocfilehash: b4348e6f73730d59e6e67b3e102b9ad9caa98add
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024726"
---
# <a name="mediacontentratingireland-resource-type"></a>Тип ресурса mediaContentRatingIreland

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|movieRating|[ratingIrelandMoviesType](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|Оценка выбранных для Ирландия фильмы. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.|
|tvRating|[ratingIrelandTelevisionType](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|Оценка TV, выбранной для Ирландия. Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



