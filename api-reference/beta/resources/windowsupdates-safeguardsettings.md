---
title: тип ресурса safeguardSettings
description: Управление гарантиями, которые служба применяет к устройствам в развертывании.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: d3c276a07483b42e513266077ef1ada3bc516d47
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792122"
---
# <a name="safeguardsettings-resource-type"></a>тип ресурса safeguardSettings

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Управление гарантиями, которые служба применяет к устройствам в развертывании.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|disabledSafeguardProfiles|[коллекция microsoft.graph.windowsUpdates.safeguardProfile](../resources/windowsupdates-safeguardprofile.md)|Список гарантий, которые необходимо игнорировать на устройстве.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.safeguardSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.safeguardSettings",
  "disabledSafeguardProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.safeguardProfile"
    }
  ]
}
```

