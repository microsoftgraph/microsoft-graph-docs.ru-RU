---
title: Тип ресурса physicalAddress
description: Представляет почтовый адрес ресурса, например контакта или события.
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d3d0a998f317a0fa19e7c29aabda5bc8e3908f85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997832"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="fbb4b-103">Тип ресурса physicalAddress</span><span class="sxs-lookup"><span data-stu-id="fbb4b-103">physicalAddress resource type</span></span>

<span data-ttu-id="fbb4b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbb4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbb4b-105">Представляет почтовый адрес ресурса, например контакта или события.</span><span class="sxs-lookup"><span data-stu-id="fbb4b-105">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="fbb4b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fbb4b-106">Properties</span></span>
| <span data-ttu-id="fbb4b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbb4b-107">Property</span></span>     | <span data-ttu-id="fbb4b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fbb4b-108">Type</span></span>   |<span data-ttu-id="fbb4b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fbb4b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbb4b-110">city</span><span class="sxs-lookup"><span data-stu-id="fbb4b-110">city</span></span>|<span data-ttu-id="fbb4b-111">String</span><span class="sxs-lookup"><span data-stu-id="fbb4b-111">String</span></span>|<span data-ttu-id="fbb4b-112">Город.</span><span class="sxs-lookup"><span data-stu-id="fbb4b-112">The city.</span></span>|
|<span data-ttu-id="fbb4b-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="fbb4b-113">countryOrRegion</span></span>|<span data-ttu-id="fbb4b-114">String</span><span class="sxs-lookup"><span data-stu-id="fbb4b-114">String</span></span>|<span data-ttu-id="fbb4b-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="fbb4b-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="fbb4b-117">postalCode</span><span class="sxs-lookup"><span data-stu-id="fbb4b-117">postalCode</span></span>|<span data-ttu-id="fbb4b-118">String</span><span class="sxs-lookup"><span data-stu-id="fbb4b-118">String</span></span>|<span data-ttu-id="fbb4b-119">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="fbb4b-119">The postal code.</span></span>|
|<span data-ttu-id="fbb4b-120">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="fbb4b-120">postOfficeBox</span></span>|<span data-ttu-id="fbb4b-121">String</span><span class="sxs-lookup"><span data-stu-id="fbb4b-121">String</span></span>|<span data-ttu-id="fbb4b-122">Номер почтового ящика в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="fbb4b-122">The post office box number.</span></span>|
|<span data-ttu-id="fbb4b-123">state</span><span class="sxs-lookup"><span data-stu-id="fbb4b-123">state</span></span>|<span data-ttu-id="fbb4b-124">String</span><span class="sxs-lookup"><span data-stu-id="fbb4b-124">String</span></span>|<span data-ttu-id="fbb4b-125">Штат.</span><span class="sxs-lookup"><span data-stu-id="fbb4b-125">The state.</span></span>|
|<span data-ttu-id="fbb4b-126">street</span><span class="sxs-lookup"><span data-stu-id="fbb4b-126">street</span></span>|<span data-ttu-id="fbb4b-127">String</span><span class="sxs-lookup"><span data-stu-id="fbb4b-127">String</span></span>|<span data-ttu-id="fbb4b-128">Улица.</span><span class="sxs-lookup"><span data-stu-id="fbb4b-128">The street.</span></span>|
|<span data-ttu-id="fbb4b-129">type</span><span class="sxs-lookup"><span data-stu-id="fbb4b-129">type</span></span>|<span data-ttu-id="fbb4b-130">physicalAddressType</span><span class="sxs-lookup"><span data-stu-id="fbb4b-130">physicalAddressType</span></span>|<span data-ttu-id="fbb4b-131">Тип адреса.</span><span class="sxs-lookup"><span data-stu-id="fbb4b-131">The type of address.</span></span> <span data-ttu-id="fbb4b-132">Возможные значения: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="fbb4b-132">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fbb4b-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fbb4b-133">JSON representation</span></span>

<span data-ttu-id="fbb4b-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbb4b-134">Here is a JSON representation of the resource</span></span>

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


