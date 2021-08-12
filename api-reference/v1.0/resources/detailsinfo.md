---
title: detailsInfo resource type
description: Пакет свойств, который может содержать любую информацию о связанном удостоверении или системе.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e5beb5d281186b16acfa38087b6ee2d9ed3f0058f972aaeba2941467c545f523
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130382"
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


