---
title: тип ресурса cloudPcStatusDetails
description: Сведения о состоянии облачного КОМПЬЮТЕРА.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ae9054e92279d976d65aafc72ac2c38190c88b84
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507818"
---
# <a name="cloudpcstatusdetails-resource-type"></a>тип ресурса cloudPcStatusDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о состоянии облачного КОМПЬЮТЕРА.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|code|String|Код, связанный с состоянием облачного КОМПЬЮТЕРА.|
|message|String|Сообщение о состоянии.|
|additionalInformation|[Коллекция KeyValuePair](../resources/keyvaluepair.md)|Любые дополнительные сведения о состоянии облачного КОМПЬЮТЕРА.|

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
