---
title: тип ресурса teamworkCameraConfiguration
description: Представляет сведения о конфигурации камеры для Комнаты Microsoft Teams устройства.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f10a0db06b158dda00f4db9e7df0e34e1ab6ac1c
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262566"
---
# <a name="teamworkcameraconfiguration-resource-type"></a>тип ресурса teamworkCameraConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о конфигурации камеры для Комнаты Microsoft Teams [устройства](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|contentCameraConfiguration|[teamworkContentCameraConfiguration](../resources/teamworkcontentcameraconfiguration.md)|Конфигурация для камеры контента.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|камеры|[teamworkPeripheral](../resources/teamworkperipheral.md) collection|Список подключенных камер.|
|defaultContentCamera|[teamworkPeripheral](../resources/teamworkperipheral.md)|Настроенная камера контента, используемая для обмена аналоговым контентом доски на собрании.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkCameraConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkCameraConfiguration",
  "contentCameraConfiguration": {
    "@odata.type": "microsoft.graph.teamworkContentCameraConfiguration"
  }
}
```

