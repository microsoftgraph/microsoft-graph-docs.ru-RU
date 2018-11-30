---
title: Тип ресурса physicalAddress
description: Представляет почтовый адрес ресурса, например контакта или события.
ms.openlocfilehash: eb2c1ea6a73d7f6eb5d3d43b877f50dc39a2b17e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026279"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="dfeb0-103">Тип ресурса physicalAddress</span><span class="sxs-lookup"><span data-stu-id="dfeb0-103">physicalAddress resource type</span></span>

<span data-ttu-id="dfeb0-104">Представляет почтовый адрес ресурса, например контакта или события.</span><span class="sxs-lookup"><span data-stu-id="dfeb0-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="dfeb0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfeb0-105">Properties</span></span>
| <span data-ttu-id="dfeb0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfeb0-106">Property</span></span>     | <span data-ttu-id="dfeb0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="dfeb0-107">Type</span></span>   |<span data-ttu-id="dfeb0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="dfeb0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfeb0-109">city</span><span class="sxs-lookup"><span data-stu-id="dfeb0-109">city</span></span>|<span data-ttu-id="dfeb0-110">String</span><span class="sxs-lookup"><span data-stu-id="dfeb0-110">String</span></span>|<span data-ttu-id="dfeb0-111">Город.</span><span class="sxs-lookup"><span data-stu-id="dfeb0-111">The city.</span></span>|
|<span data-ttu-id="dfeb0-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="dfeb0-112">countryOrRegion</span></span>|<span data-ttu-id="dfeb0-113">String</span><span class="sxs-lookup"><span data-stu-id="dfeb0-113">String</span></span>|<span data-ttu-id="dfeb0-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="dfeb0-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="dfeb0-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="dfeb0-116">postalCode</span></span>|<span data-ttu-id="dfeb0-117">String</span><span class="sxs-lookup"><span data-stu-id="dfeb0-117">String</span></span>|<span data-ttu-id="dfeb0-118">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="dfeb0-118">The postal code.</span></span>|
|<span data-ttu-id="dfeb0-119">state</span><span class="sxs-lookup"><span data-stu-id="dfeb0-119">state</span></span>|<span data-ttu-id="dfeb0-120">String</span><span class="sxs-lookup"><span data-stu-id="dfeb0-120">String</span></span>|<span data-ttu-id="dfeb0-121">Штат.</span><span class="sxs-lookup"><span data-stu-id="dfeb0-121">The state.</span></span>|
|<span data-ttu-id="dfeb0-122">street</span><span class="sxs-lookup"><span data-stu-id="dfeb0-122">street</span></span>|<span data-ttu-id="dfeb0-123">String</span><span class="sxs-lookup"><span data-stu-id="dfeb0-123">String</span></span>|<span data-ttu-id="dfeb0-124">Улица.</span><span class="sxs-lookup"><span data-stu-id="dfeb0-124">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dfeb0-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dfeb0-125">JSON representation</span></span>

<span data-ttu-id="dfeb0-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfeb0-126">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
