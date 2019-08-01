---
title: Тип ресурса physicalAddress
description: Представляет почтовый адрес ресурса, например контакта или события.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f301947d6d277cd4fd51b7db035ef4f7134a5e65
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035512"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="d6ae4-103">Тип ресурса physicalAddress</span><span class="sxs-lookup"><span data-stu-id="d6ae4-103">physicalAddress resource type</span></span>

<span data-ttu-id="d6ae4-104">Представляет почтовый адрес ресурса, например контакта или события.</span><span class="sxs-lookup"><span data-stu-id="d6ae4-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="d6ae4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6ae4-105">Properties</span></span>
| <span data-ttu-id="d6ae4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6ae4-106">Property</span></span>     | <span data-ttu-id="d6ae4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d6ae4-107">Type</span></span>   |<span data-ttu-id="d6ae4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d6ae4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6ae4-109">city</span><span class="sxs-lookup"><span data-stu-id="d6ae4-109">city</span></span>|<span data-ttu-id="d6ae4-110">String</span><span class="sxs-lookup"><span data-stu-id="d6ae4-110">String</span></span>|<span data-ttu-id="d6ae4-111">Город.</span><span class="sxs-lookup"><span data-stu-id="d6ae4-111">The city.</span></span>|
|<span data-ttu-id="d6ae4-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="d6ae4-112">countryOrRegion</span></span>|<span data-ttu-id="d6ae4-113">String</span><span class="sxs-lookup"><span data-stu-id="d6ae4-113">String</span></span>|<span data-ttu-id="d6ae4-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="d6ae4-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="d6ae4-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="d6ae4-116">postalCode</span></span>|<span data-ttu-id="d6ae4-117">String</span><span class="sxs-lookup"><span data-stu-id="d6ae4-117">String</span></span>|<span data-ttu-id="d6ae4-118">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="d6ae4-118">The postal code.</span></span>|
|<span data-ttu-id="d6ae4-119">state</span><span class="sxs-lookup"><span data-stu-id="d6ae4-119">state</span></span>|<span data-ttu-id="d6ae4-120">String</span><span class="sxs-lookup"><span data-stu-id="d6ae4-120">String</span></span>|<span data-ttu-id="d6ae4-121">Штат.</span><span class="sxs-lookup"><span data-stu-id="d6ae4-121">The state.</span></span>|
|<span data-ttu-id="d6ae4-122">street</span><span class="sxs-lookup"><span data-stu-id="d6ae4-122">street</span></span>|<span data-ttu-id="d6ae4-123">String</span><span class="sxs-lookup"><span data-stu-id="d6ae4-123">String</span></span>|<span data-ttu-id="d6ae4-124">Улица.</span><span class="sxs-lookup"><span data-stu-id="d6ae4-124">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6ae4-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6ae4-125">JSON representation</span></span>

<span data-ttu-id="d6ae4-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6ae4-126">Here is a JSON representation of the resource</span></span>

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
