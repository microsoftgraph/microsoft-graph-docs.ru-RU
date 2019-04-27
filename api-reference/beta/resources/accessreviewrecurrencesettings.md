---
title: Тип ресурса Акцессревиеврекурренцесеттингс
description: ''
localization_priority: Normal
ms.openlocfilehash: 1a5235639209830d36cf69c027cfd309fab09c3e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348421"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>Тип ресурса Акцессревиеврекурренцесеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| recurrenceType | string |  |
| Рекурренцеендтипе | string |  |
| Дуратиониндайс | Int32 |  |
| Рекурренцекаунт | Int32 |  |

## <a name="relationships"></a>Отношения
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}-->
``` json
{
    "recurrenceType":"string",
    "recurrenceEndType":"string",
    "durationInDays":"Int32",
    "recurrenceCount":"Int32"
}
```



