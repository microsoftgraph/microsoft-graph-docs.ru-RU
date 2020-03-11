---
title: Тип ресурса Аттачментитем
description: Представляет атрибуты элемента, который необходимо присоединить.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 23ae9ed8371ecc4f49f6eb4b7fae5a14964cd15f
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591546"
---
# <a name="attachmentitem-resource-type"></a><span data-ttu-id="602be-103">Тип ресурса Аттачментитем</span><span class="sxs-lookup"><span data-stu-id="602be-103">attachmentItem resource type</span></span>

<span data-ttu-id="602be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="602be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="602be-105">Представляет атрибуты элемента, который необходимо присоединить.</span><span class="sxs-lookup"><span data-stu-id="602be-105">Represents attributes of an item to be attached.</span></span>

## <a name="properties"></a><span data-ttu-id="602be-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="602be-106">Properties</span></span>

| <span data-ttu-id="602be-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="602be-107">Property</span></span>     | <span data-ttu-id="602be-108">Тип</span><span class="sxs-lookup"><span data-stu-id="602be-108">Type</span></span>        | <span data-ttu-id="602be-109">Описание</span><span class="sxs-lookup"><span data-stu-id="602be-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="602be-110">attachmentType</span><span class="sxs-lookup"><span data-stu-id="602be-110">attachmentType</span></span>|<span data-ttu-id="602be-111">String</span><span class="sxs-lookup"><span data-stu-id="602be-111">String</span></span>| <span data-ttu-id="602be-112">Тип вложения.</span><span class="sxs-lookup"><span data-stu-id="602be-112">The type of attachment.</span></span> <span data-ttu-id="602be-113">Возможные значения: `file`, `item`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="602be-113">Possible values are: `file`, `item`, `reference`.</span></span> <span data-ttu-id="602be-114">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="602be-114">Required.</span></span>|
|<span data-ttu-id="602be-115">contentType</span><span class="sxs-lookup"><span data-stu-id="602be-115">contentType</span></span>|<span data-ttu-id="602be-116">String</span><span class="sxs-lookup"><span data-stu-id="602be-116">String</span></span>|<span data-ttu-id="602be-117">Характер данных во вложении.</span><span class="sxs-lookup"><span data-stu-id="602be-117">The nature of the data in the attachment.</span></span> <span data-ttu-id="602be-118">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="602be-118">Optional.</span></span>|
|<span data-ttu-id="602be-119">isInline</span><span class="sxs-lookup"><span data-stu-id="602be-119">isInline</span></span>|<span data-ttu-id="602be-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="602be-120">Boolean</span></span>|<span data-ttu-id="602be-121">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="602be-121">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span> <span data-ttu-id="602be-122">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="602be-122">Optional.</span></span>|
|<span data-ttu-id="602be-123">name</span><span class="sxs-lookup"><span data-stu-id="602be-123">name</span></span>|<span data-ttu-id="602be-124">String</span><span class="sxs-lookup"><span data-stu-id="602be-124">String</span></span>|<span data-ttu-id="602be-125">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="602be-125">The display name of the attachment.</span></span> <span data-ttu-id="602be-126">Это может быть строка с описанием и не обязательно должно быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="602be-126">This can be a descriptive string and does not have to be the actual file name.</span></span> <span data-ttu-id="602be-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="602be-127">Required.</span></span>|
|<span data-ttu-id="602be-128">size</span><span class="sxs-lookup"><span data-stu-id="602be-128">size</span></span>|<span data-ttu-id="602be-129">Int64</span><span class="sxs-lookup"><span data-stu-id="602be-129">Int64</span></span>|<span data-ttu-id="602be-130">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="602be-130">The length of the attachment in bytes.</span></span> <span data-ttu-id="602be-131">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="602be-131">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="602be-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="602be-132">JSON representation</span></span>

<span data-ttu-id="602be-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="602be-133">The following is a JSON representation of the resource.</span></span>

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