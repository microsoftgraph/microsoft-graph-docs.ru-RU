---
title: Тип ресурса Акцессревиеврекурренцесеттингс
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: markwahl-msft
ms.openlocfilehash: 7c45a0b57d869acdb49c5a37f235232c70e8ec6f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472238"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>Тип ресурса Акцессревиеврекурренцесеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| recurrenceType | string |  |
| рекурренцеендтипе | string |  |
| дуратиониндайс | Int32 |  |
| рекурренцекаунт | Int32 |  |

## <a name="relationships"></a>Связи
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



