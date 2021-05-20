---
title: Тип ресурса assignedLicense
description: Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта user представляет собой коллекцию объектов **assignedLicense**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 9d957f2bfa5c7c9e4390e5c4df06d084a3e49e6f
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547254"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="7e3b3-104">Тип ресурса assignedLicense</span><span class="sxs-lookup"><span data-stu-id="7e3b3-104">assignedLicense resource type</span></span>

<span data-ttu-id="7e3b3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e3b3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e3b3-p102">Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта [user](user.md) представляет собой коллекцию объектов **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="7e3b3-p102">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="7e3b3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e3b3-108">Properties</span></span>
| <span data-ttu-id="7e3b3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e3b3-109">Property</span></span>     | <span data-ttu-id="7e3b3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7e3b3-110">Type</span></span>   |<span data-ttu-id="7e3b3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7e3b3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e3b3-112">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="7e3b3-112">disabledPlans</span></span>|<span data-ttu-id="7e3b3-113">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="7e3b3-113">Guid collection</span></span>|<span data-ttu-id="7e3b3-114">Коллекция уникальных идентификаторов отключенных планов.</span><span class="sxs-lookup"><span data-stu-id="7e3b3-114">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="7e3b3-115">skuId</span><span class="sxs-lookup"><span data-stu-id="7e3b3-115">skuId</span></span>|<span data-ttu-id="7e3b3-116">Guid</span><span class="sxs-lookup"><span data-stu-id="7e3b3-116">Guid</span></span>|<span data-ttu-id="7e3b3-117">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="7e3b3-117">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e3b3-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e3b3-118">JSON representation</span></span>

<span data-ttu-id="7e3b3-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e3b3-119">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


