---
title: Тип ресурса Фисикалоффицеаддресс
description: Представляет рабочий адрес ресурса, например контакт или событие.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 46674ad9be3e86fd36f5a5beb52829959bbd340b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445548"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="c4aa5-103">Тип ресурса Фисикалоффицеаддресс</span><span class="sxs-lookup"><span data-stu-id="c4aa5-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="c4aa5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4aa5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4aa5-105">Представляет рабочий адрес ресурса, например контакта в Организации.</span><span class="sxs-lookup"><span data-stu-id="c4aa5-105">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="c4aa5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4aa5-106">Properties</span></span>

| <span data-ttu-id="c4aa5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4aa5-107">Property</span></span>     | <span data-ttu-id="c4aa5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c4aa5-108">Type</span></span>   |<span data-ttu-id="c4aa5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c4aa5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4aa5-110">city</span><span class="sxs-lookup"><span data-stu-id="c4aa5-110">city</span></span>|<span data-ttu-id="c4aa5-111">String</span><span class="sxs-lookup"><span data-stu-id="c4aa5-111">String</span></span>|<span data-ttu-id="c4aa5-112">Город.</span><span class="sxs-lookup"><span data-stu-id="c4aa5-112">The city.</span></span>|
|<span data-ttu-id="c4aa5-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="c4aa5-113">countryOrRegion</span></span>|<span data-ttu-id="c4aa5-114">String</span><span class="sxs-lookup"><span data-stu-id="c4aa5-114">String</span></span>|<span data-ttu-id="c4aa5-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="c4aa5-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="c4aa5-117">officeLocation</span><span class="sxs-lookup"><span data-stu-id="c4aa5-117">officeLocation</span></span>  | <span data-ttu-id="c4aa5-118">String</span><span class="sxs-lookup"><span data-stu-id="c4aa5-118">String</span></span> | <span data-ttu-id="c4aa5-119">Местоположение Office, например здание и номер офиса для контакта в Организации.</span><span class="sxs-lookup"><span data-stu-id="c4aa5-119">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="c4aa5-120">postalCode</span><span class="sxs-lookup"><span data-stu-id="c4aa5-120">postalCode</span></span>|<span data-ttu-id="c4aa5-121">String</span><span class="sxs-lookup"><span data-stu-id="c4aa5-121">String</span></span>|<span data-ttu-id="c4aa5-122">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="c4aa5-122">The postal code.</span></span>|
|<span data-ttu-id="c4aa5-123">state</span><span class="sxs-lookup"><span data-stu-id="c4aa5-123">state</span></span>|<span data-ttu-id="c4aa5-124">String</span><span class="sxs-lookup"><span data-stu-id="c4aa5-124">String</span></span>|<span data-ttu-id="c4aa5-125">Штат.</span><span class="sxs-lookup"><span data-stu-id="c4aa5-125">The state.</span></span>|
|<span data-ttu-id="c4aa5-126">street</span><span class="sxs-lookup"><span data-stu-id="c4aa5-126">street</span></span>|<span data-ttu-id="c4aa5-127">String</span><span class="sxs-lookup"><span data-stu-id="c4aa5-127">String</span></span>|<span data-ttu-id="c4aa5-128">Улица.</span><span class="sxs-lookup"><span data-stu-id="c4aa5-128">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4aa5-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4aa5-129">JSON representation</span></span>

<span data-ttu-id="c4aa5-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4aa5-130">Here is a JSON representation of the resource</span></span>

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
