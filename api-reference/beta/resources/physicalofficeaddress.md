---
title: Тип ресурса Фисикалоффицеаддресс
description: Представляет рабочий адрес ресурса, например контакт или событие.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8299f72032cfb7910583fcd4dbefe914f054648e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966099"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="8b106-103">Тип ресурса Фисикалоффицеаддресс</span><span class="sxs-lookup"><span data-stu-id="8b106-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="8b106-104">Представляет рабочий адрес ресурса, например контакта в Организации.</span><span class="sxs-lookup"><span data-stu-id="8b106-104">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="8b106-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b106-105">Properties</span></span>

| <span data-ttu-id="8b106-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b106-106">Property</span></span>     | <span data-ttu-id="8b106-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8b106-107">Type</span></span>   |<span data-ttu-id="8b106-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8b106-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b106-109">city</span><span class="sxs-lookup"><span data-stu-id="8b106-109">city</span></span>|<span data-ttu-id="8b106-110">String</span><span class="sxs-lookup"><span data-stu-id="8b106-110">String</span></span>|<span data-ttu-id="8b106-111">Город.</span><span class="sxs-lookup"><span data-stu-id="8b106-111">The city.</span></span>|
|<span data-ttu-id="8b106-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="8b106-112">countryOrRegion</span></span>|<span data-ttu-id="8b106-113">String</span><span class="sxs-lookup"><span data-stu-id="8b106-113">String</span></span>|<span data-ttu-id="8b106-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="8b106-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="8b106-116">officeLocation</span><span class="sxs-lookup"><span data-stu-id="8b106-116">officeLocation</span></span>  | <span data-ttu-id="8b106-117">String</span><span class="sxs-lookup"><span data-stu-id="8b106-117">String</span></span> | <span data-ttu-id="8b106-118">Местоположение Office, например здание и номер офиса для контакта в Организации.</span><span class="sxs-lookup"><span data-stu-id="8b106-118">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="8b106-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="8b106-119">postalCode</span></span>|<span data-ttu-id="8b106-120">String</span><span class="sxs-lookup"><span data-stu-id="8b106-120">String</span></span>|<span data-ttu-id="8b106-121">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="8b106-121">The postal code.</span></span>|
|<span data-ttu-id="8b106-122">state</span><span class="sxs-lookup"><span data-stu-id="8b106-122">state</span></span>|<span data-ttu-id="8b106-123">String</span><span class="sxs-lookup"><span data-stu-id="8b106-123">String</span></span>|<span data-ttu-id="8b106-124">Штат.</span><span class="sxs-lookup"><span data-stu-id="8b106-124">The state.</span></span>|
|<span data-ttu-id="8b106-125">street</span><span class="sxs-lookup"><span data-stu-id="8b106-125">street</span></span>|<span data-ttu-id="8b106-126">String</span><span class="sxs-lookup"><span data-stu-id="8b106-126">String</span></span>|<span data-ttu-id="8b106-127">Улица.</span><span class="sxs-lookup"><span data-stu-id="8b106-127">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b106-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b106-128">JSON representation</span></span>

<span data-ttu-id="8b106-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b106-129">Here is a JSON representation of the resource</span></span>

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
