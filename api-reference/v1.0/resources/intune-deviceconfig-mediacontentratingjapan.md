---
title: Тип ресурса mediaContentRatingJapan
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c4e4268857f2d76e1dcf01e047a492f80492a89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031390"
---
# <a name="mediacontentratingjapan-resource-type"></a>Тип ресурса mediaContentRatingJapan

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|movieRating|[Ратингжапанмовиестипе](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|Оценка фильмов выбрана для Японии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.|
|tvRating|[Ратингжапантелевисионтипе](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|Рейтинг для телевизора выбран для Японии. Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



