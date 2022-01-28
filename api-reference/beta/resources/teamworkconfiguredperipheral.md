---
title: teamworkConfiguredPeripheral resource type
description: Представляет сведения о периферийных устройствах, настроенных для устройства с Microsoft Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 07a25c847acb1b9b7e3584b2a1a5ef86d7bff046
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262662"
---
# <a name="teamworkconfiguredperipheral-resource-type"></a>teamworkConfiguredPeripheral resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о периферийных устройствах, настроенных для Microsoft Teams с [включенной поддержкой](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isOptional|Логическое|`True` если текущее периферийное устройство является необязательным. Если установлено `false`, это свойство также используется в качестве части вычисления состояния здоровья для устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|периферийный|[teamworkPeripheral](../resources/teamworkperipheral.md)|Сведения о присоединенных периферийных устройствах.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkConfiguredPeripheral"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkConfiguredPeripheral",
  "isOptional": "Boolean"
}
```

