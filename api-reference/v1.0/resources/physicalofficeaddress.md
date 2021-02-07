---
title: Тип ресурса physicalOfficeAddress
description: Представляет бизнес-адрес ресурса, например контакт или событие.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6ba8e82f1ba8641a0b1966586744ffd4721b9b81
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135718"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="1f5ec-103">Тип ресурса physicalOfficeAddress</span><span class="sxs-lookup"><span data-stu-id="1f5ec-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="1f5ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f5ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f5ec-105">Представляет бизнес-адрес ресурса, например контакта организации.</span><span class="sxs-lookup"><span data-stu-id="1f5ec-105">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="1f5ec-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f5ec-106">Properties</span></span>

| <span data-ttu-id="1f5ec-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f5ec-107">Property</span></span>     | <span data-ttu-id="1f5ec-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1f5ec-108">Type</span></span>   |<span data-ttu-id="1f5ec-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1f5ec-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f5ec-110">city</span><span class="sxs-lookup"><span data-stu-id="1f5ec-110">city</span></span>|<span data-ttu-id="1f5ec-111">String</span><span class="sxs-lookup"><span data-stu-id="1f5ec-111">String</span></span>|<span data-ttu-id="1f5ec-112">Город.</span><span class="sxs-lookup"><span data-stu-id="1f5ec-112">The city.</span></span>|
|<span data-ttu-id="1f5ec-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="1f5ec-113">countryOrRegion</span></span>|<span data-ttu-id="1f5ec-114">String</span><span class="sxs-lookup"><span data-stu-id="1f5ec-114">String</span></span>|<span data-ttu-id="1f5ec-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="1f5ec-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="1f5ec-117">officeLocation</span><span class="sxs-lookup"><span data-stu-id="1f5ec-117">officeLocation</span></span>  | <span data-ttu-id="1f5ec-118">String</span><span class="sxs-lookup"><span data-stu-id="1f5ec-118">String</span></span> | <span data-ttu-id="1f5ec-119">Расположение Office, например номер здания и офиса для контакта организации.</span><span class="sxs-lookup"><span data-stu-id="1f5ec-119">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="1f5ec-120">postalCode</span><span class="sxs-lookup"><span data-stu-id="1f5ec-120">postalCode</span></span>|<span data-ttu-id="1f5ec-121">String</span><span class="sxs-lookup"><span data-stu-id="1f5ec-121">String</span></span>|<span data-ttu-id="1f5ec-122">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="1f5ec-122">The postal code.</span></span>|
|<span data-ttu-id="1f5ec-123">state</span><span class="sxs-lookup"><span data-stu-id="1f5ec-123">state</span></span>|<span data-ttu-id="1f5ec-124">String</span><span class="sxs-lookup"><span data-stu-id="1f5ec-124">String</span></span>|<span data-ttu-id="1f5ec-125">Штат.</span><span class="sxs-lookup"><span data-stu-id="1f5ec-125">The state.</span></span>|
|<span data-ttu-id="1f5ec-126">street</span><span class="sxs-lookup"><span data-stu-id="1f5ec-126">street</span></span>|<span data-ttu-id="1f5ec-127">String</span><span class="sxs-lookup"><span data-stu-id="1f5ec-127">String</span></span>|<span data-ttu-id="1f5ec-128">Улица.</span><span class="sxs-lookup"><span data-stu-id="1f5ec-128">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1f5ec-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f5ec-129">JSON representation</span></span>

<span data-ttu-id="1f5ec-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f5ec-130">Here is a JSON representation of the resource</span></span>

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

