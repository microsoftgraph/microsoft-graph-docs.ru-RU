---
title: тип ресурса safeguardSettings
description: Управление гарантиями, которые служба применяет к устройствам в развертывании.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: af40a9aaa8001bda15f442dd7f79baac014168a2
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695627"
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

