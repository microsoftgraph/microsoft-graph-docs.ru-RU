---
title: Тип ресурса physicalOfficeAddress
description: Представляет рабочего адреса ресурсов, таких как события или контакта.
localization_priority: Normal
ms.openlocfilehash: bd4274e29b2ef0f9e7e8318528d18103be19fabc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817789"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="739e4-103">Тип ресурса physicalOfficeAddress</span><span class="sxs-lookup"><span data-stu-id="739e4-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="739e4-104">Представляет рабочего адреса ресурсов, таких как организационные контакта.</span><span class="sxs-lookup"><span data-stu-id="739e4-104">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="739e4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="739e4-105">Properties</span></span>

| <span data-ttu-id="739e4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="739e4-106">Property</span></span>     | <span data-ttu-id="739e4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="739e4-107">Type</span></span>   |<span data-ttu-id="739e4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="739e4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="739e4-109">city</span><span class="sxs-lookup"><span data-stu-id="739e4-109">city</span></span>|<span data-ttu-id="739e4-110">String</span><span class="sxs-lookup"><span data-stu-id="739e4-110">String</span></span>|<span data-ttu-id="739e4-111">Город.</span><span class="sxs-lookup"><span data-stu-id="739e4-111">The city.</span></span>|
|<span data-ttu-id="739e4-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="739e4-112">countryOrRegion</span></span>|<span data-ttu-id="739e4-113">String</span><span class="sxs-lookup"><span data-stu-id="739e4-113">String</span></span>|<span data-ttu-id="739e4-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="739e4-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="739e4-116">officeLocation</span><span class="sxs-lookup"><span data-stu-id="739e4-116">officeLocation</span></span>  | <span data-ttu-id="739e4-117">String</span><span class="sxs-lookup"><span data-stu-id="739e4-117">String</span></span> | <span data-ttu-id="739e4-118">Расположение комнаты, например номер построения и office для организации контакта.</span><span class="sxs-lookup"><span data-stu-id="739e4-118">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="739e4-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="739e4-119">postalCode</span></span>|<span data-ttu-id="739e4-120">String</span><span class="sxs-lookup"><span data-stu-id="739e4-120">String</span></span>|<span data-ttu-id="739e4-121">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="739e4-121">The postal code.</span></span>|
|<span data-ttu-id="739e4-122">state</span><span class="sxs-lookup"><span data-stu-id="739e4-122">state</span></span>|<span data-ttu-id="739e4-123">String</span><span class="sxs-lookup"><span data-stu-id="739e4-123">String</span></span>|<span data-ttu-id="739e4-124">Штат.</span><span class="sxs-lookup"><span data-stu-id="739e4-124">The state.</span></span>|
|<span data-ttu-id="739e4-125">street</span><span class="sxs-lookup"><span data-stu-id="739e4-125">street</span></span>|<span data-ttu-id="739e4-126">String</span><span class="sxs-lookup"><span data-stu-id="739e4-126">String</span></span>|<span data-ttu-id="739e4-127">Улица.</span><span class="sxs-lookup"><span data-stu-id="739e4-127">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="739e4-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="739e4-128">JSON representation</span></span>

<span data-ttu-id="739e4-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="739e4-129">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
