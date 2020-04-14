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
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="9aa5a-103">Тип ресурса Детаилсинфо</span><span class="sxs-lookup"><span data-stu-id="9aa5a-103">detailsInfo resource type</span></span>

<span data-ttu-id="9aa5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9aa5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9aa5a-105">Контейнер свойств, который может содержать любую информацию о связанном идентификаторе или системе.</span><span class="sxs-lookup"><span data-stu-id="9aa5a-105">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="9aa5a-106">Сюда могут относиться сведения о свойстве, которое подготавливается или является источником/целевой системой.</span><span class="sxs-lookup"><span data-stu-id="9aa5a-106">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="9aa5a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9aa5a-107">Properties</span></span>
<span data-ttu-id="9aa5a-108">Ресурс **детаилсинфо** — это строка JSON, содержащая дополнительные свойства, такие как **applicationId**, **ObjectID**и **UPN**.</span><span class="sxs-lookup"><span data-stu-id="9aa5a-108">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="9aa5a-109">Набор свойств зависит от типа ресурса, который подготавливается к работе.</span><span class="sxs-lookup"><span data-stu-id="9aa5a-109">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="9aa5a-110">В [списке провисионингобжектсуммари](../api/provisioningobjectsummary-list.md) показан пример этого.</span><span class="sxs-lookup"><span data-stu-id="9aa5a-110">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="9aa5a-111">Отношения</span><span class="sxs-lookup"><span data-stu-id="9aa5a-111">Relationships</span></span>
<span data-ttu-id="9aa5a-112">Нет</span><span class="sxs-lookup"><span data-stu-id="9aa5a-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9aa5a-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9aa5a-113">JSON Representation</span></span>
<span data-ttu-id="9aa5a-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9aa5a-114">Here is a JSON representation of the resource.</span></span>
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
