---
title: Тип ресурса assignedLicense
description: Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта user представляет собой коллекцию объектов **assignedLicense**.
localization_priority: Normal
author: krbain
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b7d03a4f6fd9703a3a24900f12b2e522c6535452
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808398"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="d69eb-104">Тип ресурса assignedLicense</span><span class="sxs-lookup"><span data-stu-id="d69eb-104">assignedLicense resource type</span></span>

<span data-ttu-id="d69eb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d69eb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d69eb-106">Представляет лицензию, назначенную пользователю.</span><span class="sxs-lookup"><span data-stu-id="d69eb-106">Represents a license assigned to a user.</span></span> <span data-ttu-id="d69eb-107">Свойство **assignedLicenses** объекта [user](user.md) представляет собой коллекцию объектов **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="d69eb-107">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="d69eb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d69eb-108">Properties</span></span>
| <span data-ttu-id="d69eb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d69eb-109">Property</span></span>     | <span data-ttu-id="d69eb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d69eb-110">Type</span></span>   |<span data-ttu-id="d69eb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d69eb-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d69eb-112">дисабледпланс</span><span class="sxs-lookup"><span data-stu-id="d69eb-112">disabledPlans</span></span>|<span data-ttu-id="d69eb-113">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="d69eb-113">Guid collection</span></span>|<span data-ttu-id="d69eb-114">Коллекция уникальных идентификаторов отключенных планов.</span><span class="sxs-lookup"><span data-stu-id="d69eb-114">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="d69eb-115">skuId</span><span class="sxs-lookup"><span data-stu-id="d69eb-115">skuId</span></span>|<span data-ttu-id="d69eb-116">Guid</span><span class="sxs-lookup"><span data-stu-id="d69eb-116">Guid</span></span>|<span data-ttu-id="d69eb-117">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="d69eb-117">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d69eb-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d69eb-118">JSON representation</span></span>

<span data-ttu-id="d69eb-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d69eb-119">Here is a JSON representation of the resource</span></span>

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
