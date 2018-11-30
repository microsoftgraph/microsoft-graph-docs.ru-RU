---
title: Тип ресурса assignedLicense
description: Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта user представляет собой коллекцию объектов **assignedLicense**.
ms.openlocfilehash: a41ece17882e6b85da009b4e29292e4b9a7965af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082122"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="04caa-104">Тип ресурса assignedLicense</span><span class="sxs-lookup"><span data-stu-id="04caa-104">assignedLicense resource type</span></span>

> <span data-ttu-id="04caa-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="04caa-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04caa-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04caa-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04caa-p103">Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта [user](user.md) представляет собой коллекцию объектов **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="04caa-p103">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="04caa-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="04caa-109">Properties</span></span>
| <span data-ttu-id="04caa-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="04caa-110">Property</span></span>     | <span data-ttu-id="04caa-111">Тип</span><span class="sxs-lookup"><span data-stu-id="04caa-111">Type</span></span>   |<span data-ttu-id="04caa-112">Описание</span><span class="sxs-lookup"><span data-stu-id="04caa-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04caa-113">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="04caa-113">disabledPlans</span></span>|<span data-ttu-id="04caa-114">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="04caa-114">Guid collection</span></span>|<span data-ttu-id="04caa-115">Коллекция уникальных идентификаторов отключенных планов.</span><span class="sxs-lookup"><span data-stu-id="04caa-115">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="04caa-116">skuId</span><span class="sxs-lookup"><span data-stu-id="04caa-116">skuId</span></span>|<span data-ttu-id="04caa-117">Guid</span><span class="sxs-lookup"><span data-stu-id="04caa-117">Guid</span></span>|<span data-ttu-id="04caa-118">Уникальный идентификатор SKU.</span><span class="sxs-lookup"><span data-stu-id="04caa-118">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04caa-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04caa-119">JSON representation</span></span>

<span data-ttu-id="04caa-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04caa-120">Here is a JSON representation of the resource</span></span>

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
