---
title: Тип ресурса outgoingCallOptions
description: Представляет класс, содержащий параметры для исходящего вызова.
author: satyakonmsft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: be522b19837e07095cacb3515e351c9dcef774bb
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917932"
---
# <a name="outgoingcalloptions-resource-type"></a>Тип ресурса outgoingCallOptions

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет класс, содержащий параметры для исходящего вызова.

Наследуется [от callOptions](calloptions.md).

## <a name="properties"></a>Свойства

|Свойство                 |Тип                      |Описание                                                                        |
|:---                     |:---                      |:---                                                                               |
|isContentSharingNotificationEnabled   |Boolean                   |Значение, указывающее, следует ли включить уведомления об общем доступе к содержимому для вызова. Наследуется [от callOptions](calloptions.md).    |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outgoingCallOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outgoingCallOptions",
  "isContentSharingNotificationEnabled": "Boolean"
}
```
