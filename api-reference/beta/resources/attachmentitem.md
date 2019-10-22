---
title: Тип ресурса Аттачментитем
description: Представляет атрибуты элемента, который необходимо присоединить.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: b6570b44bab06c0ab4b8b6788ea585276b43c3cc
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621640"
---
# <a name="attachmentitem-resource-type"></a><span data-ttu-id="c957e-103">Тип ресурса Аттачментитем</span><span class="sxs-lookup"><span data-stu-id="c957e-103">attachmentItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c957e-104">Представляет атрибуты элемента, который необходимо присоединить.</span><span class="sxs-lookup"><span data-stu-id="c957e-104">Represents attributes of an item to be attached.</span></span>

## <a name="properties"></a><span data-ttu-id="c957e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c957e-105">Properties</span></span>

| <span data-ttu-id="c957e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c957e-106">Property</span></span>     | <span data-ttu-id="c957e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c957e-107">Type</span></span>        | <span data-ttu-id="c957e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c957e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c957e-109">attachmentType</span><span class="sxs-lookup"><span data-stu-id="c957e-109">attachmentType</span></span>|<span data-ttu-id="c957e-110">String</span><span class="sxs-lookup"><span data-stu-id="c957e-110">String</span></span>| <span data-ttu-id="c957e-111">Тип вложения.</span><span class="sxs-lookup"><span data-stu-id="c957e-111">The type of attachment.</span></span> <span data-ttu-id="c957e-112">Возможные значения: `file`, `item`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="c957e-112">Possible values are: `file`, `item`, `reference`.</span></span> <span data-ttu-id="c957e-113">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="c957e-113">Required.</span></span>|
|<span data-ttu-id="c957e-114">contentType</span><span class="sxs-lookup"><span data-stu-id="c957e-114">contentType</span></span>|<span data-ttu-id="c957e-115">String</span><span class="sxs-lookup"><span data-stu-id="c957e-115">String</span></span>|<span data-ttu-id="c957e-116">Характер данных во вложении.</span><span class="sxs-lookup"><span data-stu-id="c957e-116">The nature of the data in the attachment.</span></span> <span data-ttu-id="c957e-117">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c957e-117">Optional.</span></span>|
|<span data-ttu-id="c957e-118">isInline</span><span class="sxs-lookup"><span data-stu-id="c957e-118">isInline</span></span>|<span data-ttu-id="c957e-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="c957e-119">Boolean</span></span>|<span data-ttu-id="c957e-120">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="c957e-120">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span> <span data-ttu-id="c957e-121">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c957e-121">Optional.</span></span>|
|<span data-ttu-id="c957e-122">name</span><span class="sxs-lookup"><span data-stu-id="c957e-122">name</span></span>|<span data-ttu-id="c957e-123">String</span><span class="sxs-lookup"><span data-stu-id="c957e-123">String</span></span>|<span data-ttu-id="c957e-124">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="c957e-124">The display name of the attachment.</span></span> <span data-ttu-id="c957e-125">Это может быть строка с описанием и не обязательно должно быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="c957e-125">This can be a descriptive string and does not have to be the actual file name.</span></span> <span data-ttu-id="c957e-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c957e-126">Required.</span></span>|
|<span data-ttu-id="c957e-127">size</span><span class="sxs-lookup"><span data-stu-id="c957e-127">size</span></span>|<span data-ttu-id="c957e-128">Int64</span><span class="sxs-lookup"><span data-stu-id="c957e-128">Int64</span></span>|<span data-ttu-id="c957e-129">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="c957e-129">The length of the attachment in bytes.</span></span> <span data-ttu-id="c957e-130">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="c957e-130">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c957e-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c957e-131">JSON representation</span></span>

<span data-ttu-id="c957e-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c957e-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentType",
    "isInline"
  ],
  "@odata.type": "microsoft.graph.attachmentItem",
  "baseType": null
}-->

```json
{
  "attachmentType": "String",
  "contentType": "String",
  "isInline": true,
  "name": "String",
  "size": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachmentItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->