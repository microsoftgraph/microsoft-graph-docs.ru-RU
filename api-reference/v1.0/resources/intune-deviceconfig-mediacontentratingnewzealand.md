---
title: Тип ресурса mediaContentRatingNewZealand
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6787ec82cf70aa10c72a20ab60619449dbb14327
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473108"
---
# <a name="mediacontentratingnewzealand-resource-type"></a>Тип ресурса mediaContentRatingNewZealand

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|movieRating|[ратингневзеаландмовиестипе](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|Рейтинг фильмов, выбранный для Новой Зеландии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.|
|tvRating|[ратингневзеаландтелевисионтипе](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|Рейтинг для телевизора, выбранный для Новой Зеландии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```







