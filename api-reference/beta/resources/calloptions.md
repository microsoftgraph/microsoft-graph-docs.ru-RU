---
title: Тип ресурса callOptions
description: Абстрактный базовый класс, содержащий дополнительные функции для вызова.
author: satyakonmsft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 53d845d7667f04f5b028fdde01b2658e578a7a25
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917959"
---
# <a name="calloptions-resource-type"></a>Тип ресурса callOptions

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный базовый класс, содержащий дополнительные функции для вызова.

## <a name="properties"></a>Свойства

|Свойство                 |Тип                      |Описание                                                                        |
|:---                     |:---                      |:---                                                                               |
|isContentSharingNotificationEnabled   |Boolean                   |Указывает, следует ли включить уведомления об общем доступе к содержимому для вызова.    |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callOptions",
  "isContentSharingNotificationEnabled": "Boolean"
}
```
