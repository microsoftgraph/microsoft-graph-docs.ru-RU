---
title: Тип ресурса Фисикалоффицеаддресс
description: Представляет рабочий адрес ресурса, например контакт или событие.
localization_priority: Normal
ms.openlocfilehash: bd4274e29b2ef0f9e7e8318528d18103be19fabc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573734"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="c044d-103">Тип ресурса Фисикалоффицеаддресс</span><span class="sxs-lookup"><span data-stu-id="c044d-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="c044d-104">Представляет рабочий адрес ресурса, например контакта в Организации.</span><span class="sxs-lookup"><span data-stu-id="c044d-104">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="c044d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c044d-105">Properties</span></span>

| <span data-ttu-id="c044d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c044d-106">Property</span></span>     | <span data-ttu-id="c044d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c044d-107">Type</span></span>   |<span data-ttu-id="c044d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c044d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c044d-109">city</span><span class="sxs-lookup"><span data-stu-id="c044d-109">city</span></span>|<span data-ttu-id="c044d-110">String</span><span class="sxs-lookup"><span data-stu-id="c044d-110">String</span></span>|<span data-ttu-id="c044d-111">Город.</span><span class="sxs-lookup"><span data-stu-id="c044d-111">The city.</span></span>|
|<span data-ttu-id="c044d-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="c044d-112">countryOrRegion</span></span>|<span data-ttu-id="c044d-113">String</span><span class="sxs-lookup"><span data-stu-id="c044d-113">String</span></span>|<span data-ttu-id="c044d-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="c044d-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="c044d-116">officeLocation</span><span class="sxs-lookup"><span data-stu-id="c044d-116">officeLocation</span></span>  | <span data-ttu-id="c044d-117">String</span><span class="sxs-lookup"><span data-stu-id="c044d-117">String</span></span> | <span data-ttu-id="c044d-118">Местоположение Office, например здание и номер офиса для контакта в Организации.</span><span class="sxs-lookup"><span data-stu-id="c044d-118">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="c044d-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="c044d-119">postalCode</span></span>|<span data-ttu-id="c044d-120">String</span><span class="sxs-lookup"><span data-stu-id="c044d-120">String</span></span>|<span data-ttu-id="c044d-121">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="c044d-121">The postal code.</span></span>|
|<span data-ttu-id="c044d-122">state</span><span class="sxs-lookup"><span data-stu-id="c044d-122">state</span></span>|<span data-ttu-id="c044d-123">String</span><span class="sxs-lookup"><span data-stu-id="c044d-123">String</span></span>|<span data-ttu-id="c044d-124">Штат.</span><span class="sxs-lookup"><span data-stu-id="c044d-124">The state.</span></span>|
|<span data-ttu-id="c044d-125">street</span><span class="sxs-lookup"><span data-stu-id="c044d-125">street</span></span>|<span data-ttu-id="c044d-126">String</span><span class="sxs-lookup"><span data-stu-id="c044d-126">String</span></span>|<span data-ttu-id="c044d-127">Улица.</span><span class="sxs-lookup"><span data-stu-id="c044d-127">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c044d-128">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c044d-128">JSON representation</span></span>

<span data-ttu-id="c044d-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c044d-129">Here is a JSON representation of the resource</span></span>

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
