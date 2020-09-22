---
title: Тип ресурса Детаилсинфо
description: Контейнер свойств, который может содержать любую информацию о связанном идентификаторе или системе.
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c08dcb867f92bd65449be891bf0ae0e8a12a2459
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049879"
---
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="2d3ab-103">Тип ресурса Детаилсинфо</span><span class="sxs-lookup"><span data-stu-id="2d3ab-103">detailsInfo resource type</span></span>

<span data-ttu-id="2d3ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d3ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d3ab-105">Контейнер свойств, который может содержать любую информацию о связанном идентификаторе или системе.</span><span class="sxs-lookup"><span data-stu-id="2d3ab-105">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="2d3ab-106">Сюда могут относиться сведения о свойстве, которое подготавливается или является источником/целевой системой.</span><span class="sxs-lookup"><span data-stu-id="2d3ab-106">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="2d3ab-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d3ab-107">Properties</span></span>
<span data-ttu-id="2d3ab-108">Ресурс **детаилсинфо** — это строка JSON, содержащая дополнительные свойства, такие как **applicationId**, **ObjectID**и **UPN**.</span><span class="sxs-lookup"><span data-stu-id="2d3ab-108">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="2d3ab-109">Набор свойств зависит от типа ресурса, который подготавливается к работе.</span><span class="sxs-lookup"><span data-stu-id="2d3ab-109">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="2d3ab-110">В [списке провисионингобжектсуммари](../api/provisioningobjectsummary-list.md) показан пример этого.</span><span class="sxs-lookup"><span data-stu-id="2d3ab-110">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="2d3ab-111">Связи</span><span class="sxs-lookup"><span data-stu-id="2d3ab-111">Relationships</span></span>
<span data-ttu-id="2d3ab-112">Нет</span><span class="sxs-lookup"><span data-stu-id="2d3ab-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2d3ab-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d3ab-113">JSON Representation</span></span>
<span data-ttu-id="2d3ab-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d3ab-114">Here is a JSON representation of the resource.</span></span>
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


