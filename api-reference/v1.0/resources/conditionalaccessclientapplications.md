---
title: Тип ресурса conditionalAccessClientApplications
description: Представляет клиентские приложения (субъекты-службы и удостоверения рабочей нагрузки), включенные в область политики и исключаемые из нее.
author: calebb
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0afcbcc68291d73aa83f9d730d81c257932c1dd7
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819064"
---
# <a name="conditionalaccessclientapplications-resource-type"></a>Тип ресурса conditionalAccessClientApplications

Пространство имен: microsoft.graph

Представляет клиентские приложения (субъекты-службы и удостоверения рабочей нагрузки), включенные в область политики и исключаемые из нее.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|excludeServicePrincipals|Коллекция строк|Идентификаторы субъекта-службы, исключенные из области политики.|
|includeServicePrincipals|Коллекция String|Идентификаторы субъекта-службы, включенные в область политики, или `ServicePrincipalsInMyTenant`. |

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

