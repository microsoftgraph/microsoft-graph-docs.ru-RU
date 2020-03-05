---
title: Тип ресурса Имажеинфо
description: Сложный тип для представления свойства " **атрибуты** " в части висуалинфо объекта Activity.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: resourcePageType
ms.openlocfilehash: 35b4ad8573fe588c8e58123a36cc3acd97122fe2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447054"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="edc93-103">Тип ресурса Имажеинфо</span><span class="sxs-lookup"><span data-stu-id="edc93-103">imageInfo resource type</span></span>

<span data-ttu-id="edc93-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="edc93-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="edc93-105">Сложный тип для представления свойства " **атрибуты** " в части [висуалинфо](../resources/projectrome-visualinfo.md) объекта [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="edc93-105">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="edc93-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="edc93-106">Properties</span></span>

|<span data-ttu-id="edc93-107">Имя</span><span class="sxs-lookup"><span data-stu-id="edc93-107">Name</span></span> | <span data-ttu-id="edc93-108">Тип</span><span class="sxs-lookup"><span data-stu-id="edc93-108">Type</span></span> | <span data-ttu-id="edc93-109">Описание</span><span class="sxs-lookup"><span data-stu-id="edc93-109">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="edc93-110">iconUrl</span><span class="sxs-lookup"><span data-stu-id="edc93-110">iconUrl</span></span> | <span data-ttu-id="edc93-111">String</span><span class="sxs-lookup"><span data-stu-id="edc93-111">String</span></span> | <span data-ttu-id="edc93-112">Необязательно URI, указывающий на значок, представляющий приложение, используемое для создания действия.</span><span class="sxs-lookup"><span data-stu-id="edc93-112">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="edc93-113">алтернатетекст</span><span class="sxs-lookup"><span data-stu-id="edc93-113">alternateText</span></span> | <span data-ttu-id="edc93-114">String</span><span class="sxs-lookup"><span data-stu-id="edc93-114">String</span></span> | <span data-ttu-id="edc93-115">Необязательно доступное для изображения содержимое с замещающим текстом</span><span class="sxs-lookup"><span data-stu-id="edc93-115">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="edc93-116">аддимажекуери</span><span class="sxs-lookup"><span data-stu-id="edc93-116">addImageQuery</span></span> | <span data-ttu-id="edc93-117">Логический</span><span class="sxs-lookup"><span data-stu-id="edc93-117">Boolean</span></span> | <span data-ttu-id="edc93-118">Необязательно параметр, указывающий на то, что сервер может динамически отображать изображение в ответ на параметризация.</span><span class="sxs-lookup"><span data-stu-id="edc93-118">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="edc93-119">Например, изображение с высокой контрастностью</span><span class="sxs-lookup"><span data-stu-id="edc93-119">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edc93-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edc93-120">JSON Representation</span></span>

<span data-ttu-id="edc93-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edc93-121">Here is a JSON representation of the resource</span></span>

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
