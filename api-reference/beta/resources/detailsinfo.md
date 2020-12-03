---
title: Тип ресурса Детаилсинфо
description: Контейнер свойств, который может содержать любую информацию о связанном идентификаторе или системе.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9325942a9419a13be92b41bf4d726efcf926041d
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523373"
---
# <a name="detailsinfo-resource-type"></a>Тип ресурса Детаилсинфо

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер свойств, который может содержать любую информацию о связанном идентификаторе или системе. Сюда могут относиться сведения о свойстве, которое подготавливается или является источником/целевой системой.

## <a name="properties"></a>Свойства
Ресурс **детаилсинфо** — это строка JSON, содержащая дополнительные свойства, такие как **applicationId**, **ObjectID** и **UPN**. Набор свойств зависит от типа ресурса, который подготавливается к работе. В [списке провисионингобжектсуммари](../api/provisioningobjectsummary-list.md) показан пример этого.

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


