---
title: Тип ресурса mediaContentRatingUnitedStates
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: baa5d98f0fcb1d267221c95c0b27be988d3a197f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254732"
---
# <a name="mediacontentratingunitedstates-resource-type"></a>Тип ресурса mediaContentRatingUnitedStates

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|movieRating|[Ратингунитедстатесмовиестипе](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|Оценка фильмов, выбранных для США. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.|
|tvRating|[Ратингунитедстатестелевисионтипе](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|Рейтинг для телевизора выбран для США. Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



