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
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="f8a1a-103">Тип ресурса Детаилсинфо</span><span class="sxs-lookup"><span data-stu-id="f8a1a-103">detailsInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8a1a-104">Контейнер свойств, который может содержать любую информацию о связанном идентификаторе или системе.</span><span class="sxs-lookup"><span data-stu-id="f8a1a-104">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="f8a1a-105">Сюда могут относиться сведения о свойстве, которое подготавливается или является источником/целевой системой.</span><span class="sxs-lookup"><span data-stu-id="f8a1a-105">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="f8a1a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8a1a-106">Properties</span></span>
<span data-ttu-id="f8a1a-107">Ресурс **детаилсинфо** — это строка JSON, содержащая дополнительные свойства, такие как **applicationId**, **ObjectID**и **UPN**.</span><span class="sxs-lookup"><span data-stu-id="f8a1a-107">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="f8a1a-108">Набор свойств зависит от типа ресурса, который подготавливается к работе.</span><span class="sxs-lookup"><span data-stu-id="f8a1a-108">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="f8a1a-109">В [списке провисионингобжектсуммари](../api/provisioningobjectsummary-list.md) показан пример этого.</span><span class="sxs-lookup"><span data-stu-id="f8a1a-109">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="f8a1a-110">Отношения</span><span class="sxs-lookup"><span data-stu-id="f8a1a-110">Relationships</span></span>
<span data-ttu-id="f8a1a-111">Нет</span><span class="sxs-lookup"><span data-stu-id="f8a1a-111">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f8a1a-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8a1a-112">JSON Representation</span></span>
<span data-ttu-id="f8a1a-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8a1a-113">Here is a JSON representation of the resource.</span></span>
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
