---
title: Тип ресурса detailsInfo
description: Пакет свойств, который может содержать любые сведения о связанном удостоверении или системе.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 25441071581af0b9e35ef941d8c82998bdea7b38
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135662"
---
# <a name="detailsinfo-resource-type"></a>Тип ресурса detailsInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Пакет свойств, который может содержать любые сведения о связанном удостоверении или системе. Это может включать сведения о свойстве, которое необходимо получить, или источник/целевая система.

## <a name="properties"></a>Свойства
Ресурс **detailsInfo —** это строка JSON, которая содержит дополнительные свойства, такие как **ApplicationId,** **ObjectId** и **UPN.** Набор свойств зависит от типа ресурса, который необходимо создать. [Пример этого показан в списке provisioningObjectSummary.](../api/provisioningobjectsummary-list.md)

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


