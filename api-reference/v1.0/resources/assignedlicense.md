---
title: Тип ресурса assignedLicense
description: Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта user представляет собой коллекцию объектов **assignedLicense**.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cd551085dac72b2f63e2cb67d9ada978746c0b5c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030081"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="94322-104">Тип ресурса assignedLicense</span><span class="sxs-lookup"><span data-stu-id="94322-104">assignedLicense resource type</span></span>

<span data-ttu-id="94322-105">Представляет лицензию, назначенную пользователю.</span><span class="sxs-lookup"><span data-stu-id="94322-105">Represents a license assigned to a user.</span></span> <span data-ttu-id="94322-106">Свойство **assignedLicenses** объекта [user](user.md) представляет собой коллекцию объектов **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="94322-106">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="94322-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="94322-107">Properties</span></span>
| <span data-ttu-id="94322-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="94322-108">Property</span></span>     | <span data-ttu-id="94322-109">Тип</span><span class="sxs-lookup"><span data-stu-id="94322-109">Type</span></span>   |<span data-ttu-id="94322-110">Описание</span><span class="sxs-lookup"><span data-stu-id="94322-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94322-111">Дисабледпланс</span><span class="sxs-lookup"><span data-stu-id="94322-111">disabledPlans</span></span>|<span data-ttu-id="94322-112">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="94322-112">Guid collection</span></span>|<span data-ttu-id="94322-113">Коллекция уникальных идентификаторов отключенных планов.</span><span class="sxs-lookup"><span data-stu-id="94322-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="94322-114">skuId</span><span class="sxs-lookup"><span data-stu-id="94322-114">skuId</span></span>|<span data-ttu-id="94322-115">Guid</span><span class="sxs-lookup"><span data-stu-id="94322-115">Guid</span></span>|<span data-ttu-id="94322-116">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="94322-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94322-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94322-117">JSON representation</span></span>

<span data-ttu-id="94322-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94322-118">Here is a JSON representation of the resource</span></span>

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
