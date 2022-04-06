---
title: тип ресурса conditionalAccessClientApplications
description: Представляет клиентские приложения (директора служб и удостоверения рабочей нагрузки), включенные и исключенные из области политики.
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f53d79f311d5f6be8b3d9ee0781636eb4c62c686
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672754"
---
# <a name="conditionalaccessclientapplications-resource-type"></a>тип ресурса conditionalAccessClientApplications

Пространство имен: microsoft.graph

Представляет клиентские приложения (директора служб и удостоверения рабочей нагрузки), включенные и исключенные из области политики.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|excludeServicePrincipals|Коллекция объектов string|Основные ID службы исключены из области политики.|
|includeServicePrincipals|Коллекция объектов string|Основные ID-службы, включенные в область политики, или `ServicePrincipalsInMyTenant`. |

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

