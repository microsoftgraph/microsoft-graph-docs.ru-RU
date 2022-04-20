---
title: Тип ресурса extractSensitivityLabelsResult
description: Представляет формат ответа для API extractSensitivityLabels.
author: jaLuthra
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a3533cecf651c6b98deb81b01cf06d5a08f2dc36
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917940"
---
# <a name="extractsensitivitylabelsresult-resource-type"></a>Тип ресурса extractSensitivityLabelsResult

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет формат ответа для API [extractSensitivityLabels](../api/driveitem-extractsensitivitylabels.md) .

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Метки|[Коллекция sensitivityLabelAssignment](./sensitivitylabelassignment.md)|Список меток конфиденциальности, назначенных файлу.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extractSensitivityLabelsResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extractSensitivityLabelsResult",
  "labels": [
    {
      "@odata.type": "microsoft.graph.sensitivityLabelAssignment"
    }
  ]
}
```

