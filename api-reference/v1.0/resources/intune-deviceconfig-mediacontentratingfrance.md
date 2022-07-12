---
title: Тип ресурса mediaContentRatingFrance
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 39ef6f85bc1de4d8d9cbf752c4087df2b5ff7117
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734755"
---
# <a name="mediacontentratingfrance-resource-type"></a>Тип ресурса mediaContentRatingFrance

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|movieRating|[ratingFranceMoviesType](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|Рейтинг фильмов, выбранный для Франции. Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.|
|tvRating|[RatingFranceTelevisionType](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|Рейтинг телевизора, выбранный для Франции. Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```





