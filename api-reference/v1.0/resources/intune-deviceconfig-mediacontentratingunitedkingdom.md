---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 947fd12d8219215b0828ef1c05d2d8b36f970f16
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572306"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a>Тип ресурса mediaContentRatingUnitedKingdom

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|movieRating|[Ратингунитедкингдоммовиестипе](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|Оценка фильмов выбрана для Великобритании. Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.|
|tvRating|[Ратингунитедкингдомтелевисионтипе](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|Рейтинг для телевизора выбран для Великобритании. Возможные значения: `allAllowed`, `allBlocked`, `caution`.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



