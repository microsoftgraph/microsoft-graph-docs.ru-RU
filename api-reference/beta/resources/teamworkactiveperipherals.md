---
title: тип ресурса teamworkActivePeripherals
description: Представляет сведения об активных периферийных устройствах, присоединенных к устройству с Microsoft Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e1f740a347f4adc717588dccc49acafc145e42c8
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262735"
---
# <a name="teamworkactiveperipherals-resource-type"></a>тип ресурса teamworkActivePeripherals

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об активных периферийных устройствах, присоединенных к устройству с Microsoft Teams [включенной поддержкой](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|communicationSpeaker|[teamworkPeripheral](../resources/teamworkperipheral.md)|Связанные сведения о динамике связи.|
|contentCamera|[teamworkPeripheral](../resources/teamworkperipheral.md)|Связанные данные камеры контента.|
|микрофон|[teamworkPeripheral](../resources/teamworkperipheral.md)|Связанные сведения о микрофоне.|
|roomCamera|[teamworkPeripheral](../resources/teamworkperipheral.md)|Связанные сведения камеры комнаты.|
|динамик|[teamworkPeripheral](../resources/teamworkperipheral.md)|Связанные сведения о динамике.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkActivePeripherals"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkActivePeripherals"
}
```

