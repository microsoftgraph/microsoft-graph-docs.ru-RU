---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc6be04b245e07d9dea11dae750ff5e56b68a5e0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788557"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a>Тип ресурса mediaContentRatingUnitedKingdom

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|movieRating|[ратингунитедкингдоммовиестипе](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|Оценка фильмов выбрана для Великобритании. Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.|
|tvRating|[ратингунитедкингдомтелевисионтипе](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|Рейтинг для телевизора выбран для Великобритании. Возможные значения: `allAllowed`, `allBlocked`, `caution`.|

## <a name="relationships"></a>Связи
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



