---
title: тип ресурса teamworkContentCameraConfiguration
description: Представляет сведения о конфигурации для камеры контента, подключенной к устройству с Microsoft Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 00db0e0fbd61afe3f113a903d60aeb5bf02f6581
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262657"
---
# <a name="teamworkcontentcameraconfiguration-resource-type"></a>тип ресурса teamworkContentCameraConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о конфигурации для камеры контента, подключенной к устройству с Microsoft Teams включенной [поддержкой](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isContentCameraInverted|Логическое|`True` если камера контента перевернута.|
|isContentCameraOptional|Логическое|`True` если камера контента необязательна.|
|isContentEnhancementEnabled|Логическое|`True` если включено повышение контента.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkContentCameraConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkContentCameraConfiguration",
  "isContentCameraInverted": "Boolean",
  "isContentCameraOptional": "Boolean",
  "isContentEnhancementEnabled": "Boolean"
}
```

