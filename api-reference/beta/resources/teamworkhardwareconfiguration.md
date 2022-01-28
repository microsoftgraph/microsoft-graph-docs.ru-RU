---
title: тип ресурса teamworkHardwareConfiguration
description: Представляет сведения о конфигурации оборудования для устройства с Microsoft Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 118c2cda70a9751ce8c02a9af52d89982141dfef
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262591"
---
# <a name="teamworkhardwareconfiguration-resource-type"></a>тип ресурса teamworkHardwareConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о конфигурации оборудования для устройства с Microsoft Teams включенной [поддержкой](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|processorModel|String|Модель ЦП на устройстве.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|compute|[teamworkPeripheral](../resources/teamworkperipheral.md)|Сведения о системе для [teamworkDevice](../resources/teamworkdevice.md).|
|hdmiIngest|[teamworkPeripheral](../resources/teamworkperipheral.md)|Сведения о том, как hdMI гнается на устройстве.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkHardwareConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHardwareConfiguration",
  "processorModel": "String"
}
```

