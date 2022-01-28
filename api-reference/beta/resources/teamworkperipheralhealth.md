---
title: тип ресурса teamworkPeripheralHealth
description: Представляет сведения о состоянии здоровья для периферийного устройства, подключенного к устройству с Microsoft Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 914165343623fea7f807b5dc5f8146b79714c90e
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262578"
---
# <a name="teamworkperipheralhealth-resource-type"></a>тип ресурса teamworkPeripheralHealth

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о состоянии здоровья для периферийного устройства, подключенного Microsoft Teams с включенным [устройством](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|подключение|[teamworkConnection](../resources/teamworkconnection.md)|Подключенное состояние и время с момента подключения периферийного устройства.|
|isOptional|Логическое|`True` если периферийное устройство является необязательным. Используется для вычислений для здоровья.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|периферийный|[teamworkPeripheral](../resources/teamworkperipheral.md)|Сведения о периферийных устройствах.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkPeripheralHealth",
  "connection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  },
  "isOptional": "Boolean"
}
```

