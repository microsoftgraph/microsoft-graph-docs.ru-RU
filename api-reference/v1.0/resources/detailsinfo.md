---
title: detailsInfo resource type
description: Пакет свойств, который может содержать любую информацию о связанном удостоверении или системе.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1841c513651131c4bf624c07ee117fae32df79f7
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240778"
---
# <a name="detailsinfo-resource-type"></a>detailsInfo resource type

Пространство имен: microsoft.graph

Пакет свойств, который может содержать любую информацию о связанном удостоверении или системе. Это может включать сведения о свойствах, которые в настоящее время подготовка или источник / целевая система.

## <a name="properties"></a>Свойства
Ресурс **detailsInfo** — это строка JSON, которая содержит дополнительные свойства, такие как **ApplicationId,** **ObjectId** и **UPN.** Набор свойств зависит от типа ресурса, который будет создан. [В примере list provisioningObjectSummary.](../api/provisioningobjectsummary-list.md)

## <a name="relationships"></a>Связи
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


