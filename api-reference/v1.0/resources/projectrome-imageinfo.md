---
title: Тип ресурса Имажеинфо
description: Сложный тип для представления свойства " **атрибуты** " в части висуалинфо объекта Activity.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: resourcePageType
ms.openlocfilehash: e79bea73a5a7a81ad92eab159745d2cf64938483
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035016"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="fbd1c-103">Тип ресурса Имажеинфо</span><span class="sxs-lookup"><span data-stu-id="fbd1c-103">imageInfo resource type</span></span>

<span data-ttu-id="fbd1c-104">Сложный тип для представления свойства " **атрибуты** " в части [висуалинфо](../resources/projectrome-visualinfo.md) объекта [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="fbd1c-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="fbd1c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fbd1c-105">Properties</span></span>

|<span data-ttu-id="fbd1c-106">Имя</span><span class="sxs-lookup"><span data-stu-id="fbd1c-106">Name</span></span> | <span data-ttu-id="fbd1c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fbd1c-107">Type</span></span> | <span data-ttu-id="fbd1c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fbd1c-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="fbd1c-109">iconUrl</span><span class="sxs-lookup"><span data-stu-id="fbd1c-109">iconUrl</span></span> | <span data-ttu-id="fbd1c-110">String</span><span class="sxs-lookup"><span data-stu-id="fbd1c-110">String</span></span> | <span data-ttu-id="fbd1c-111">Необязательно URI, указывающий на значок, представляющий приложение, используемое для создания действия.</span><span class="sxs-lookup"><span data-stu-id="fbd1c-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="fbd1c-112">Алтернатетекст</span><span class="sxs-lookup"><span data-stu-id="fbd1c-112">alternateText</span></span> | <span data-ttu-id="fbd1c-113">String</span><span class="sxs-lookup"><span data-stu-id="fbd1c-113">String</span></span> | <span data-ttu-id="fbd1c-114">Необязательно доступное для изображения содержимое с замещающим текстом</span><span class="sxs-lookup"><span data-stu-id="fbd1c-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="fbd1c-115">Аддимажекуери</span><span class="sxs-lookup"><span data-stu-id="fbd1c-115">addImageQuery</span></span> | <span data-ttu-id="fbd1c-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbd1c-116">Boolean</span></span> | <span data-ttu-id="fbd1c-117">Необязательно параметр, указывающий на то, что сервер может динамически отображать изображение в ответ на параметризация.</span><span class="sxs-lookup"><span data-stu-id="fbd1c-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="fbd1c-118">Например, изображение с высокой контрастностью</span><span class="sxs-lookup"><span data-stu-id="fbd1c-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbd1c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fbd1c-119">JSON Representation</span></span>

<span data-ttu-id="fbd1c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbd1c-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
