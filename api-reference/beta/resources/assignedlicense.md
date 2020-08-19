---
title: Тип ресурса assignedLicense
description: Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта user представляет собой коллекцию объектов **assignedLicense**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: 29dec5abd28969871376de5a55a932cea9297848
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809875"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="b8185-104">Тип ресурса assignedLicense</span><span class="sxs-lookup"><span data-stu-id="b8185-104">assignedLicense resource type</span></span>

<span data-ttu-id="b8185-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8185-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8185-106">Представляет лицензию, назначенную пользователю.</span><span class="sxs-lookup"><span data-stu-id="b8185-106">Represents a license assigned to a user.</span></span> <span data-ttu-id="b8185-107">Свойство **assignedLicenses** объекта [user](user.md) представляет собой коллекцию объектов **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="b8185-107">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="b8185-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8185-108">Properties</span></span>
| <span data-ttu-id="b8185-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8185-109">Property</span></span>     | <span data-ttu-id="b8185-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b8185-110">Type</span></span>   |<span data-ttu-id="b8185-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b8185-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8185-112">дисабледпланс</span><span class="sxs-lookup"><span data-stu-id="b8185-112">disabledPlans</span></span>|<span data-ttu-id="b8185-113">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="b8185-113">Guid collection</span></span>|<span data-ttu-id="b8185-114">Коллекция уникальных идентификаторов отключенных планов.</span><span class="sxs-lookup"><span data-stu-id="b8185-114">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="b8185-115">skuId</span><span class="sxs-lookup"><span data-stu-id="b8185-115">skuId</span></span>|<span data-ttu-id="b8185-116">Guid</span><span class="sxs-lookup"><span data-stu-id="b8185-116">Guid</span></span>|<span data-ttu-id="b8185-117">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="b8185-117">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8185-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b8185-118">JSON representation</span></span>

<span data-ttu-id="b8185-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8185-119">Here is a JSON representation of the resource</span></span>

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
