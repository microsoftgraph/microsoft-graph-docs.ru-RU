---
title: Тип ресурса conditionalAccessClientApplications
description: Представляет клиентские приложения (субъекты-службы и удостоверения рабочей нагрузки), включенные в область политики и исключаемые из нее.
author: calebb
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 151ab019a145e19b18add198c4e824eb0952e314
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819449"
---
# <a name="conditionalaccessclientapplications-resource-type"></a>Тип ресурса conditionalAccessClientApplications

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

