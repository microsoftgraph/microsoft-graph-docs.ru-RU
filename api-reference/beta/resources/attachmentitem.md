---
title: Тип ресурса attachmentItem
description: Представляет атрибуты вложенного элемента.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a469ff035b63c16b422a23d4ffad91dbc361157f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130292"
---
# <a name="attachmentitem-resource-type"></a><span data-ttu-id="11f79-103">Тип ресурса attachmentItem</span><span class="sxs-lookup"><span data-stu-id="11f79-103">attachmentItem resource type</span></span>

<span data-ttu-id="11f79-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11f79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11f79-105">Представляет атрибуты вложенного элемента.</span><span class="sxs-lookup"><span data-stu-id="11f79-105">Represents attributes of an item to be attached.</span></span>

## <a name="properties"></a><span data-ttu-id="11f79-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="11f79-106">Properties</span></span>

| <span data-ttu-id="11f79-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="11f79-107">Property</span></span>     | <span data-ttu-id="11f79-108">Тип</span><span class="sxs-lookup"><span data-stu-id="11f79-108">Type</span></span>        | <span data-ttu-id="11f79-109">Описание</span><span class="sxs-lookup"><span data-stu-id="11f79-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="11f79-110">attachmentType</span><span class="sxs-lookup"><span data-stu-id="11f79-110">attachmentType</span></span>|<span data-ttu-id="11f79-111">Строка</span><span class="sxs-lookup"><span data-stu-id="11f79-111">String</span></span>| <span data-ttu-id="11f79-112">Тип вложения.</span><span class="sxs-lookup"><span data-stu-id="11f79-112">The type of attachment.</span></span> <span data-ttu-id="11f79-113">Возможные значения: `file`, `item`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="11f79-113">Possible values are: `file`, `item`, `reference`.</span></span> <span data-ttu-id="11f79-114">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="11f79-114">Required.</span></span>|
|<span data-ttu-id="11f79-115">contentType</span><span class="sxs-lookup"><span data-stu-id="11f79-115">contentType</span></span>|<span data-ttu-id="11f79-116">String</span><span class="sxs-lookup"><span data-stu-id="11f79-116">String</span></span>|<span data-ttu-id="11f79-117">Характер данных во вложении.</span><span class="sxs-lookup"><span data-stu-id="11f79-117">The nature of the data in the attachment.</span></span> <span data-ttu-id="11f79-118">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="11f79-118">Optional.</span></span>|
|<span data-ttu-id="11f79-119">isInline</span><span class="sxs-lookup"><span data-stu-id="11f79-119">isInline</span></span>|<span data-ttu-id="11f79-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="11f79-120">Boolean</span></span>|<span data-ttu-id="11f79-121">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="11f79-121">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span> <span data-ttu-id="11f79-122">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="11f79-122">Optional.</span></span>|
|<span data-ttu-id="11f79-123">name</span><span class="sxs-lookup"><span data-stu-id="11f79-123">name</span></span>|<span data-ttu-id="11f79-124">String</span><span class="sxs-lookup"><span data-stu-id="11f79-124">String</span></span>|<span data-ttu-id="11f79-125">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="11f79-125">The display name of the attachment.</span></span> <span data-ttu-id="11f79-126">Это может быть описательная строка, которая не должна быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="11f79-126">This can be a descriptive string and does not have to be the actual file name.</span></span> <span data-ttu-id="11f79-127">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="11f79-127">Required.</span></span>|
|<span data-ttu-id="11f79-128">size</span><span class="sxs-lookup"><span data-stu-id="11f79-128">size</span></span>|<span data-ttu-id="11f79-129">Int64</span><span class="sxs-lookup"><span data-stu-id="11f79-129">Int64</span></span>|<span data-ttu-id="11f79-130">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="11f79-130">The length of the attachment in bytes.</span></span> <span data-ttu-id="11f79-131">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="11f79-131">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11f79-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11f79-132">JSON representation</span></span>

<span data-ttu-id="11f79-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11f79-133">The following is a JSON representation of the resource.</span></span>

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

