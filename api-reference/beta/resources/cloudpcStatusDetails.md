---
title: тип ресурса cloudPcStatusDetails
description: Сведения о состоянии облачного КОМПЬЮТЕРА.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 28735467ef1bc233f5ba6d5ecc3144d64e31df3e
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780900"
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

## <a name="relationships"></a>Отношения

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
