---
title: Тип ресурса Детаилсинфо
description: Контейнер свойств, который может содержать любую информацию о связанном идентификаторе или системе.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d3a6726c2151376d858f7962527e4dc6f9b53e7
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349436"
---
# <a name="detailsinfo-resource-type"></a>Тип ресурса Детаилсинфо

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер свойств, который может содержать любую информацию о связанном идентификаторе или системе. Сюда могут относиться сведения о свойстве, которое подготавливается или является источником/целевой системой.

## <a name="properties"></a>Свойства
Ресурс **детаилсинфо** — это строка JSON, содержащая дополнительные свойства, такие как **applicationId**, **ObjectID**и **UPN**. Набор свойств зависит от типа ресурса, который подготавливается к работе. В [списке провисионингобжектсуммари](../api/provisioningobjectsummary-list.md) показан пример этого.

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
