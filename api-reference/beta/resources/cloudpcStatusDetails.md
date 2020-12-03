---
title: Тип ресурса Клаудпкстатусдетаилс
description: Сведения о состоянии облачного компьютера.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 61260bc7f3437fe1f10575afc616462eec2e47dc
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563863"
---
# <a name="cloudpcstatusdetails-resource-type"></a>Тип ресурса Клаудпкстатусдетаилс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о состоянии облачного компьютера.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|code|String|Код, связанный с состоянием Cloud PC.|
|message|String|Сообщение о состоянии.|
|аддитионалинформатион|Коллекция [KeyValuePair](../resources/keyvaluepair.md)|Любые дополнительные сведения о состоянии Cloud PC.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcStatusDetails",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcStatusDetails",
  "code": "String",
  "message": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```
