---
title: Тип ресурса Имажеинфо
description: Сложный тип для представления свойства " **атрибуты** " в части висуалинфо объекта Activity.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: d4ed317b987d461c9ef6816e9d05aae0de358ec7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037201"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="65f4f-103">Тип ресурса Имажеинфо</span><span class="sxs-lookup"><span data-stu-id="65f4f-103">imageInfo resource type</span></span>

<span data-ttu-id="65f4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65f4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65f4f-105">Сложный тип для представления свойства " **атрибуты** " в части [висуалинфо](../resources/projectrome-visualinfo.md) объекта [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="65f4f-105">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="65f4f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="65f4f-106">Properties</span></span>

|<span data-ttu-id="65f4f-107">Имя</span><span class="sxs-lookup"><span data-stu-id="65f4f-107">Name</span></span> | <span data-ttu-id="65f4f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="65f4f-108">Type</span></span> | <span data-ttu-id="65f4f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="65f4f-109">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="65f4f-110">iconUrl</span><span class="sxs-lookup"><span data-stu-id="65f4f-110">iconUrl</span></span> | <span data-ttu-id="65f4f-111">String</span><span class="sxs-lookup"><span data-stu-id="65f4f-111">String</span></span> | <span data-ttu-id="65f4f-112">Необязательно URI, указывающий на значок, представляющий приложение, используемое для создания действия.</span><span class="sxs-lookup"><span data-stu-id="65f4f-112">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="65f4f-113">алтернатетекст</span><span class="sxs-lookup"><span data-stu-id="65f4f-113">alternateText</span></span> | <span data-ttu-id="65f4f-114">String</span><span class="sxs-lookup"><span data-stu-id="65f4f-114">String</span></span> | <span data-ttu-id="65f4f-115">Необязательно доступное для изображения содержимое с замещающим текстом</span><span class="sxs-lookup"><span data-stu-id="65f4f-115">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="65f4f-116">аддимажекуери</span><span class="sxs-lookup"><span data-stu-id="65f4f-116">addImageQuery</span></span> | <span data-ttu-id="65f4f-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="65f4f-117">Boolean</span></span> | <span data-ttu-id="65f4f-118">Необязательно параметр, указывающий на то, что сервер может динамически отображать изображение в ответ на параметризация.</span><span class="sxs-lookup"><span data-stu-id="65f4f-118">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="65f4f-119">Например, изображение с высокой контрастностью</span><span class="sxs-lookup"><span data-stu-id="65f4f-119">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65f4f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65f4f-120">JSON Representation</span></span>

<span data-ttu-id="65f4f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65f4f-121">Here is a JSON representation of the resource</span></span>

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

