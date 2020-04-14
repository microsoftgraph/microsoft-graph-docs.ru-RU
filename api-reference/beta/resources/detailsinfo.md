---
title: Тип ресурса Детаилсинфо
description: Контейнер свойств, который может содержать любую информацию о связанном идентификаторе или системе.
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f62a773bb65f5d323ad6f906e53467366f7956d0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463055"
---
# <a name="detailsinfo-resource-type"></a>Тип ресурса Детаилсинфо

Пространство имен: microsoft.graph

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
