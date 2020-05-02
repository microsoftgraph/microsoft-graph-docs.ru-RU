---
title: Тип ресурса Аттачментитем
description: Представляет атрибуты элемента, который необходимо присоединить.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5df3abd262ae9b09fa1843648906c70d07e6ec51
ms.sourcegitcommit: feebe30e62aa19ce5cb8e8338e043326e464ed9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991870"
---
# <a name="attachmentitem-resource-type"></a><span data-ttu-id="8207a-103">Тип ресурса Аттачментитем</span><span class="sxs-lookup"><span data-stu-id="8207a-103">attachmentItem resource type</span></span>

<span data-ttu-id="8207a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8207a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8207a-105">Представляет атрибуты элемента, который необходимо присоединить.</span><span class="sxs-lookup"><span data-stu-id="8207a-105">Represents attributes of an item to be attached.</span></span>

## <a name="properties"></a><span data-ttu-id="8207a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8207a-106">Properties</span></span>

| <span data-ttu-id="8207a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8207a-107">Property</span></span>     | <span data-ttu-id="8207a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8207a-108">Type</span></span>        | <span data-ttu-id="8207a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8207a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8207a-110">attachmentType</span><span class="sxs-lookup"><span data-stu-id="8207a-110">attachmentType</span></span>|<span data-ttu-id="8207a-111">String</span><span class="sxs-lookup"><span data-stu-id="8207a-111">String</span></span>| <span data-ttu-id="8207a-112">Тип вложения.</span><span class="sxs-lookup"><span data-stu-id="8207a-112">The type of attachment.</span></span> <span data-ttu-id="8207a-113">Возможные значения: `file`, `item`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="8207a-113">Possible values are: `file`, `item`, `reference`.</span></span> <span data-ttu-id="8207a-114">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="8207a-114">Required.</span></span>|
|<span data-ttu-id="8207a-115">contentType</span><span class="sxs-lookup"><span data-stu-id="8207a-115">contentType</span></span>|<span data-ttu-id="8207a-116">String</span><span class="sxs-lookup"><span data-stu-id="8207a-116">String</span></span>|<span data-ttu-id="8207a-117">Характер данных во вложении.</span><span class="sxs-lookup"><span data-stu-id="8207a-117">The nature of the data in the attachment.</span></span> <span data-ttu-id="8207a-118">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8207a-118">Optional.</span></span>|
|<span data-ttu-id="8207a-119">isInline</span><span class="sxs-lookup"><span data-stu-id="8207a-119">isInline</span></span>|<span data-ttu-id="8207a-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="8207a-120">Boolean</span></span>|<span data-ttu-id="8207a-121">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="8207a-121">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span> <span data-ttu-id="8207a-122">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8207a-122">Optional.</span></span>|
|<span data-ttu-id="8207a-123">name</span><span class="sxs-lookup"><span data-stu-id="8207a-123">name</span></span>|<span data-ttu-id="8207a-124">String</span><span class="sxs-lookup"><span data-stu-id="8207a-124">String</span></span>|<span data-ttu-id="8207a-125">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="8207a-125">The display name of the attachment.</span></span> <span data-ttu-id="8207a-126">Это может быть строка с описанием и не обязательно должно быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="8207a-126">This can be a descriptive string and does not have to be the actual file name.</span></span> <span data-ttu-id="8207a-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8207a-127">Required.</span></span>|
|<span data-ttu-id="8207a-128">size</span><span class="sxs-lookup"><span data-stu-id="8207a-128">size</span></span>|<span data-ttu-id="8207a-129">Int64</span><span class="sxs-lookup"><span data-stu-id="8207a-129">Int64</span></span>|<span data-ttu-id="8207a-130">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="8207a-130">The length of the attachment in bytes.</span></span> <span data-ttu-id="8207a-131">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="8207a-131">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8207a-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8207a-132">JSON representation</span></span>

<span data-ttu-id="8207a-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8207a-133">The following is a JSON representation of the resource.</span></span>

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