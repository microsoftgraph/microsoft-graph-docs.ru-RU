---
title: тип ресурса conditionalAccessClientApplications
description: Представляет клиентские приложения (директора служб и удостоверения рабочей нагрузки), включенные и исключенные из области политики.
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ad30e86d9c434641e197338613f5f58cf5d2a788
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2022
ms.locfileid: "62239377"
---
# <a name="conditionalaccessclientapplications-resource-type"></a>тип ресурса conditionalAccessClientApplications

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет клиентские приложения (директора служб и удостоверения рабочей нагрузки), включенные и исключенные из области политики.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|excludeServicePrincipals|Коллекция строк|Основные ID службы исключены из области политики.|
|includeServicePrincipals|Коллекция строк|Основные ID-службы, включенные в область политики, или `ServicePrincipalsInMyTenant` . |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessClientApplications"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessClientApplications",
  "includeServicePrincipals": [
    "String"
  ],
  "excludeServicePrincipals": [
    "String"
  ]
}
```

