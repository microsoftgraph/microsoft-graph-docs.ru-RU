---
title: Тип ресурса Клаудпкстатусдетаилс
description: Сведения о состоянии облачного компьютера.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 647c13878e054fbac6c1f43f565bd2788d19a9de
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378642"
---
# <a name="cloudpcstatusdetails-resource-type"></a>Тип ресурса Клаудпкстатусдетаилс

Пространство имен: microsoft.graph

Сведения о состоянии облачного компьютера.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|code|Строка|Код, связанный с состоянием Cloud PC.|
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
