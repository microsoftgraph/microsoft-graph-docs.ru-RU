---
title: тип ресурса teamworkHardwareDetail
description: Представляет сведения о свойствах оборудования устройства с Microsoft Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ec4c292666a8889a34d1dce85c9a3d70630825a7
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262560"
---
# <a name="teamworkhardwaredetail-resource-type"></a>тип ресурса teamworkHardwareDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о свойствах оборудования устройства с Microsoft Teams с [включенной поддержкой](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|macAddresses|Коллекция строк|MAC-адрес.|
|manufacturer|String|Производитель устройств.|
|model|String|Модель Devie.|
|serialNumber|String|Серийный номер устройства.|
|uniqueId|String|Уникальный идентификатор устройства.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkHardwareDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHardwareDetail",
  "macAddresses": [
    "String"
  ],
  "manufacturer": "String",
  "model": "String",
  "serialNumber": "String",
  "uniqueId": "String"
}
```

