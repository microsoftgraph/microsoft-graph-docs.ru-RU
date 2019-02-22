---
title: Тип ресурса mediaContentRatingJapan
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b10d498edd03850a52aa09ba29e352a143a77c5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163443"
---
# <a name="mediacontentratingjapan-resource-type"></a>Тип ресурса mediaContentRatingJapan

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|movieRating|[Ратингжапанмовиестипе](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|Оценка фильмов выбрана для Японии. Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.|
|tvRating|[Ратингжапантелевисионтипе](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|Рейтинг для телевизора выбран для Японии. Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.|

## <a name="relationships"></a>Связи
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




