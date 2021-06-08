---
title: Тип ресурса mediaContentRatingNewZealand
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4fc7374d8e71714a5c66da1b2dc66aa5175c3e33
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760253"
---
# <a name="mediacontentratingnewzealand-resource-type"></a>Тип ресурса mediaContentRatingNewZealand

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|movieRating|[ratingNewZealandMoviesType](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|Рейтинг фильмов, выбранный для Новой Зеландии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.|
|tvRating|[ratingNewZealandTelevisionType](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|Телевизионный рейтинг, выбранный для Новой Зеландии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.|

## <a name="relationships"></a>Связи
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




