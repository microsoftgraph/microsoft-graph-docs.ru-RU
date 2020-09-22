---
title: Тип ресурса Акцессревиеврекурренцесеттингс
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: markwahl-msft
ms.openlocfilehash: e629bbe5affbf2f21b7c4041e62a3df68785dacc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024593"
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





