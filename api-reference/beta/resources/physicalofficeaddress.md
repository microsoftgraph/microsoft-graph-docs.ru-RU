---
title: Тип ресурса physicalOfficeAddress
description: Представляет бизнес-адрес ресурса, например контакт или событие.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: dkershaw10
ms.openlocfilehash: 8ff1672b0960c68ef826c89b9217109bdeb7da76
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130825"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="efe35-103">Тип ресурса physicalOfficeAddress</span><span class="sxs-lookup"><span data-stu-id="efe35-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="efe35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efe35-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="efe35-105">Представляет бизнес-адрес ресурса, например контакта организации.</span><span class="sxs-lookup"><span data-stu-id="efe35-105">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="efe35-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="efe35-106">Properties</span></span>

| <span data-ttu-id="efe35-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="efe35-107">Property</span></span>     | <span data-ttu-id="efe35-108">Тип</span><span class="sxs-lookup"><span data-stu-id="efe35-108">Type</span></span>   |<span data-ttu-id="efe35-109">Описание</span><span class="sxs-lookup"><span data-stu-id="efe35-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efe35-110">city</span><span class="sxs-lookup"><span data-stu-id="efe35-110">city</span></span>|<span data-ttu-id="efe35-111">String</span><span class="sxs-lookup"><span data-stu-id="efe35-111">String</span></span>|<span data-ttu-id="efe35-112">Город.</span><span class="sxs-lookup"><span data-stu-id="efe35-112">The city.</span></span>|
|<span data-ttu-id="efe35-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="efe35-113">countryOrRegion</span></span>|<span data-ttu-id="efe35-114">String</span><span class="sxs-lookup"><span data-stu-id="efe35-114">String</span></span>|<span data-ttu-id="efe35-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="efe35-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="efe35-117">officeLocation</span><span class="sxs-lookup"><span data-stu-id="efe35-117">officeLocation</span></span>  | <span data-ttu-id="efe35-118">String</span><span class="sxs-lookup"><span data-stu-id="efe35-118">String</span></span> | <span data-ttu-id="efe35-119">Расположение Office, например номер здания и офиса для контакта организации.</span><span class="sxs-lookup"><span data-stu-id="efe35-119">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="efe35-120">postalCode</span><span class="sxs-lookup"><span data-stu-id="efe35-120">postalCode</span></span>|<span data-ttu-id="efe35-121">String</span><span class="sxs-lookup"><span data-stu-id="efe35-121">String</span></span>|<span data-ttu-id="efe35-122">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="efe35-122">The postal code.</span></span>|
|<span data-ttu-id="efe35-123">state</span><span class="sxs-lookup"><span data-stu-id="efe35-123">state</span></span>|<span data-ttu-id="efe35-124">String</span><span class="sxs-lookup"><span data-stu-id="efe35-124">String</span></span>|<span data-ttu-id="efe35-125">Штат.</span><span class="sxs-lookup"><span data-stu-id="efe35-125">The state.</span></span>|
|<span data-ttu-id="efe35-126">street</span><span class="sxs-lookup"><span data-stu-id="efe35-126">street</span></span>|<span data-ttu-id="efe35-127">String</span><span class="sxs-lookup"><span data-stu-id="efe35-127">String</span></span>|<span data-ttu-id="efe35-128">Улица.</span><span class="sxs-lookup"><span data-stu-id="efe35-128">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efe35-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="efe35-129">JSON representation</span></span>

<span data-ttu-id="efe35-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efe35-130">Here is a JSON representation of the resource</span></span>

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


