---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 794e0cb0a461a9ff23c7c3351925dd3efd7ebf89
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437149"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a>Тип ресурса mediaContentRatingUnitedKingdom

Пространство имен: microsoft.graph

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



