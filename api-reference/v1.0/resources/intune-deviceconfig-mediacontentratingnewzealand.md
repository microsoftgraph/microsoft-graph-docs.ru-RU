---
title: Тип ресурса mediaContentRatingNewZealand
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 943a2d12ea1774bff6f12acd958b22f884cfa749
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532442"
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




