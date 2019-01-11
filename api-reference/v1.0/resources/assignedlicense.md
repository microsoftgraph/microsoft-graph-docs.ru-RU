---
title: Тип ресурса assignedLicense
description: Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта user представляет собой коллекцию объектов **assignedLicense**.
localization_priority: Normal
ms.openlocfilehash: 1e190060d0aafa4d494240f691b354b28e7697c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885346"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="a195e-104">Тип ресурса assignedLicense</span><span class="sxs-lookup"><span data-stu-id="a195e-104">assignedLicense resource type</span></span>

<span data-ttu-id="a195e-p102">Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта [user](user.md) представляет собой коллекцию объектов **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="a195e-p102">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="a195e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a195e-107">Properties</span></span>
| <span data-ttu-id="a195e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a195e-108">Property</span></span>     | <span data-ttu-id="a195e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a195e-109">Type</span></span>   |<span data-ttu-id="a195e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a195e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a195e-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="a195e-111">disabledPlans</span></span>|<span data-ttu-id="a195e-112">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="a195e-112">Guid collection</span></span>|<span data-ttu-id="a195e-113">Коллекция уникальных идентификаторов отключенных планов.</span><span class="sxs-lookup"><span data-stu-id="a195e-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="a195e-114">skuId</span><span class="sxs-lookup"><span data-stu-id="a195e-114">skuId</span></span>|<span data-ttu-id="a195e-115">Guid</span><span class="sxs-lookup"><span data-stu-id="a195e-115">Guid</span></span>|<span data-ttu-id="a195e-116">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="a195e-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a195e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a195e-117">JSON representation</span></span>

<span data-ttu-id="a195e-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a195e-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
