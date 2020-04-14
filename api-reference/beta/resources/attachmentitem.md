---
title: Тип ресурса Аттачментитем
description: Представляет атрибуты элемента, который необходимо присоединить.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7402a22665fec8716156395f4a783c804a42febb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461025"
---
# <a name="attachmentitem-resource-type"></a><span data-ttu-id="ff52e-103">Тип ресурса Аттачментитем</span><span class="sxs-lookup"><span data-stu-id="ff52e-103">attachmentItem resource type</span></span>

<span data-ttu-id="ff52e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff52e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff52e-105">Представляет атрибуты элемента, который необходимо присоединить.</span><span class="sxs-lookup"><span data-stu-id="ff52e-105">Represents attributes of an item to be attached.</span></span>

## <a name="properties"></a><span data-ttu-id="ff52e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff52e-106">Properties</span></span>

| <span data-ttu-id="ff52e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff52e-107">Property</span></span>     | <span data-ttu-id="ff52e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ff52e-108">Type</span></span>        | <span data-ttu-id="ff52e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ff52e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff52e-110">attachmentType</span><span class="sxs-lookup"><span data-stu-id="ff52e-110">attachmentType</span></span>|<span data-ttu-id="ff52e-111">String</span><span class="sxs-lookup"><span data-stu-id="ff52e-111">String</span></span>| <span data-ttu-id="ff52e-112">Тип вложения.</span><span class="sxs-lookup"><span data-stu-id="ff52e-112">The type of attachment.</span></span> <span data-ttu-id="ff52e-113">Возможные значения: `file`, `item`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="ff52e-113">Possible values are: `file`, `item`, `reference`.</span></span> <span data-ttu-id="ff52e-114">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="ff52e-114">Required.</span></span>|
|<span data-ttu-id="ff52e-115">contentType</span><span class="sxs-lookup"><span data-stu-id="ff52e-115">contentType</span></span>|<span data-ttu-id="ff52e-116">String</span><span class="sxs-lookup"><span data-stu-id="ff52e-116">String</span></span>|<span data-ttu-id="ff52e-117">Характер данных во вложении.</span><span class="sxs-lookup"><span data-stu-id="ff52e-117">The nature of the data in the attachment.</span></span> <span data-ttu-id="ff52e-118">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="ff52e-118">Optional.</span></span>|
|<span data-ttu-id="ff52e-119">isInline</span><span class="sxs-lookup"><span data-stu-id="ff52e-119">isInline</span></span>|<span data-ttu-id="ff52e-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff52e-120">Boolean</span></span>|<span data-ttu-id="ff52e-121">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="ff52e-121">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span> <span data-ttu-id="ff52e-122">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="ff52e-122">Optional.</span></span>|
|<span data-ttu-id="ff52e-123">name</span><span class="sxs-lookup"><span data-stu-id="ff52e-123">name</span></span>|<span data-ttu-id="ff52e-124">String</span><span class="sxs-lookup"><span data-stu-id="ff52e-124">String</span></span>|<span data-ttu-id="ff52e-125">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="ff52e-125">The display name of the attachment.</span></span> <span data-ttu-id="ff52e-126">Это может быть строка с описанием и не обязательно должно быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="ff52e-126">This can be a descriptive string and does not have to be the actual file name.</span></span> <span data-ttu-id="ff52e-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ff52e-127">Required.</span></span>|
|<span data-ttu-id="ff52e-128">size</span><span class="sxs-lookup"><span data-stu-id="ff52e-128">size</span></span>|<span data-ttu-id="ff52e-129">Int64</span><span class="sxs-lookup"><span data-stu-id="ff52e-129">Int64</span></span>|<span data-ttu-id="ff52e-130">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="ff52e-130">The length of the attachment in bytes.</span></span> <span data-ttu-id="ff52e-131">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="ff52e-131">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff52e-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff52e-132">JSON representation</span></span>

<span data-ttu-id="ff52e-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff52e-133">The following is a JSON representation of the resource.</span></span>

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