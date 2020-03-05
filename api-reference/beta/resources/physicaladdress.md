---
title: Тип ресурса physicalAddress
description: Представляет почтовый адрес ресурса, например контакта или события.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 53b1e18bd1e7b78e7afb479cac3c5f6cc7ecff88
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521878"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="a016d-103">Тип ресурса physicalAddress</span><span class="sxs-lookup"><span data-stu-id="a016d-103">physicalAddress resource type</span></span>

<span data-ttu-id="a016d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a016d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a016d-105">Представляет почтовый адрес ресурса, например контакта или события.</span><span class="sxs-lookup"><span data-stu-id="a016d-105">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="a016d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a016d-106">Properties</span></span>
| <span data-ttu-id="a016d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a016d-107">Property</span></span>     | <span data-ttu-id="a016d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a016d-108">Type</span></span>   |<span data-ttu-id="a016d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a016d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a016d-110">city</span><span class="sxs-lookup"><span data-stu-id="a016d-110">city</span></span>|<span data-ttu-id="a016d-111">String</span><span class="sxs-lookup"><span data-stu-id="a016d-111">String</span></span>|<span data-ttu-id="a016d-112">Город.</span><span class="sxs-lookup"><span data-stu-id="a016d-112">The city.</span></span>|
|<span data-ttu-id="a016d-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="a016d-113">countryOrRegion</span></span>|<span data-ttu-id="a016d-114">String</span><span class="sxs-lookup"><span data-stu-id="a016d-114">String</span></span>|<span data-ttu-id="a016d-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="a016d-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="a016d-117">postalCode</span><span class="sxs-lookup"><span data-stu-id="a016d-117">postalCode</span></span>|<span data-ttu-id="a016d-118">String</span><span class="sxs-lookup"><span data-stu-id="a016d-118">String</span></span>|<span data-ttu-id="a016d-119">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="a016d-119">The postal code.</span></span>|
|<span data-ttu-id="a016d-120">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="a016d-120">postOfficeBox</span></span>|<span data-ttu-id="a016d-121">String</span><span class="sxs-lookup"><span data-stu-id="a016d-121">String</span></span>|<span data-ttu-id="a016d-122">Номер почтового ящика в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a016d-122">The post office box number.</span></span>|
|<span data-ttu-id="a016d-123">state</span><span class="sxs-lookup"><span data-stu-id="a016d-123">state</span></span>|<span data-ttu-id="a016d-124">String</span><span class="sxs-lookup"><span data-stu-id="a016d-124">String</span></span>|<span data-ttu-id="a016d-125">Штат.</span><span class="sxs-lookup"><span data-stu-id="a016d-125">The state.</span></span>|
|<span data-ttu-id="a016d-126">street</span><span class="sxs-lookup"><span data-stu-id="a016d-126">street</span></span>|<span data-ttu-id="a016d-127">String</span><span class="sxs-lookup"><span data-stu-id="a016d-127">String</span></span>|<span data-ttu-id="a016d-128">Улица.</span><span class="sxs-lookup"><span data-stu-id="a016d-128">The street.</span></span>|
|<span data-ttu-id="a016d-129">type</span><span class="sxs-lookup"><span data-stu-id="a016d-129">type</span></span>|<span data-ttu-id="a016d-130">physicalAddressType</span><span class="sxs-lookup"><span data-stu-id="a016d-130">physicalAddressType</span></span>|<span data-ttu-id="a016d-131">Тип адреса.</span><span class="sxs-lookup"><span data-stu-id="a016d-131">The type of address.</span></span> <span data-ttu-id="a016d-132">Возможные значения: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="a016d-132">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a016d-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a016d-133">JSON representation</span></span>

<span data-ttu-id="a016d-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a016d-134">Here is a JSON representation of the resource</span></span>

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
  "postOfficeBox": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
