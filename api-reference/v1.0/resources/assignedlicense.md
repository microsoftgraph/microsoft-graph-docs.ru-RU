---
title: Тип ресурса assignedLicense
description: Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта user представляет собой коллекцию объектов **assignedLicense**.
ms.openlocfilehash: 48863a9acdcfa173a3f0c1a2a008516360ffdf9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025544"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="41e24-104">Тип ресурса assignedLicense</span><span class="sxs-lookup"><span data-stu-id="41e24-104">assignedLicense resource type</span></span>

<span data-ttu-id="41e24-p102">Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта [user](user.md) представляет собой коллекцию объектов **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="41e24-p102">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="41e24-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="41e24-107">Properties</span></span>
| <span data-ttu-id="41e24-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="41e24-108">Property</span></span>     | <span data-ttu-id="41e24-109">Тип</span><span class="sxs-lookup"><span data-stu-id="41e24-109">Type</span></span>   |<span data-ttu-id="41e24-110">Описание</span><span class="sxs-lookup"><span data-stu-id="41e24-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41e24-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="41e24-111">disabledPlans</span></span>|<span data-ttu-id="41e24-112">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="41e24-112">Guid collection</span></span>|<span data-ttu-id="41e24-113">Коллекция уникальных идентификаторов отключенных планов.</span><span class="sxs-lookup"><span data-stu-id="41e24-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="41e24-114">skuId</span><span class="sxs-lookup"><span data-stu-id="41e24-114">skuId</span></span>|<span data-ttu-id="41e24-115">Guid</span><span class="sxs-lookup"><span data-stu-id="41e24-115">Guid</span></span>|<span data-ttu-id="41e24-116">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="41e24-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41e24-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41e24-117">JSON representation</span></span>

<span data-ttu-id="41e24-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41e24-118">Here is a JSON representation of the resource</span></span>

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
