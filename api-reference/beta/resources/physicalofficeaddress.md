---
title: Тип ресурса physicalOfficeAddress
description: Представляет рабочего адреса ресурсов, таких как события или контакта.
ms.openlocfilehash: 472e4dfd03670f5fd4ff6b5c5c53342fff5c391a
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2018
ms.locfileid: "27284100"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="74b79-103">Тип ресурса physicalOfficeAddress</span><span class="sxs-lookup"><span data-stu-id="74b79-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="74b79-104">Представляет рабочего адреса ресурсов, таких как организационные контакта.</span><span class="sxs-lookup"><span data-stu-id="74b79-104">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="74b79-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="74b79-105">Properties</span></span>

| <span data-ttu-id="74b79-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="74b79-106">Property</span></span>     | <span data-ttu-id="74b79-107">Тип</span><span class="sxs-lookup"><span data-stu-id="74b79-107">Type</span></span>   |<span data-ttu-id="74b79-108">Описание</span><span class="sxs-lookup"><span data-stu-id="74b79-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74b79-109">city</span><span class="sxs-lookup"><span data-stu-id="74b79-109">city</span></span>|<span data-ttu-id="74b79-110">String</span><span class="sxs-lookup"><span data-stu-id="74b79-110">String</span></span>|<span data-ttu-id="74b79-111">Город.</span><span class="sxs-lookup"><span data-stu-id="74b79-111">The city.</span></span>|
|<span data-ttu-id="74b79-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="74b79-112">countryOrRegion</span></span>|<span data-ttu-id="74b79-113">String</span><span class="sxs-lookup"><span data-stu-id="74b79-113">String</span></span>|<span data-ttu-id="74b79-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="74b79-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="74b79-116">officeLocation</span><span class="sxs-lookup"><span data-stu-id="74b79-116">officeLocation</span></span>  | <span data-ttu-id="74b79-117">String</span><span class="sxs-lookup"><span data-stu-id="74b79-117">String</span></span> | <span data-ttu-id="74b79-118">Расположение комнаты, например номер построения и office для организации контакта.</span><span class="sxs-lookup"><span data-stu-id="74b79-118">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="74b79-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="74b79-119">postalCode</span></span>|<span data-ttu-id="74b79-120">String</span><span class="sxs-lookup"><span data-stu-id="74b79-120">String</span></span>|<span data-ttu-id="74b79-121">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="74b79-121">The postal code.</span></span>|
|<span data-ttu-id="74b79-122">state</span><span class="sxs-lookup"><span data-stu-id="74b79-122">state</span></span>|<span data-ttu-id="74b79-123">String</span><span class="sxs-lookup"><span data-stu-id="74b79-123">String</span></span>|<span data-ttu-id="74b79-124">Штат.</span><span class="sxs-lookup"><span data-stu-id="74b79-124">The state.</span></span>|
|<span data-ttu-id="74b79-125">street</span><span class="sxs-lookup"><span data-stu-id="74b79-125">street</span></span>|<span data-ttu-id="74b79-126">String</span><span class="sxs-lookup"><span data-stu-id="74b79-126">String</span></span>|<span data-ttu-id="74b79-127">Улица.</span><span class="sxs-lookup"><span data-stu-id="74b79-127">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74b79-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74b79-128">JSON representation</span></span>

<span data-ttu-id="74b79-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74b79-129">Here is a JSON representation of the resource</span></span>

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
