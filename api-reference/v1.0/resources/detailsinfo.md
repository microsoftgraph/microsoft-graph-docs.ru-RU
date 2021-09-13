---
title: detailsInfo resource type
description: Пакет свойств, который может содержать любую информацию о связанном удостоверении или системе.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: f755e7014e1a381697874e3e8da1afe72fa51fe0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104217"
---
# <a name="detailsinfo-resource-type"></a>detailsInfo resource type

Пространство имен: microsoft.graph

Пакет свойств, который может содержать любую информацию о связанном удостоверении или системе. Это может включать сведения о свойствах, которые в настоящее время подготовка или источник / целевая система.

## <a name="properties"></a>Свойства
Ресурс **detailsInfo** — это строка JSON, которая содержит дополнительные свойства, такие как **ApplicationId,** **ObjectId** и **UPN.** Набор свойств зависит от типа ресурса, который будет создан. [В примере list provisioningObjectSummary.](../api/provisioningobjectsummary-list.md)

## <a name="relationships"></a>Отношения
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.detailsInfo",
  "openType": true,
 "optionalProperties": [
 
 ],
}-->
``` json
{
  "@odata.type": "microsoft.graph.detailsInfo"
}
```


