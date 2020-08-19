---
title: Тип ресурса Имажеинфо
description: Сложный тип для представления свойства " **атрибуты** " в части висуалинфо объекта Activity.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: 70d95d833518814f75d31227264be0dd5f85dba4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806886"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="140c6-103">Тип ресурса Имажеинфо</span><span class="sxs-lookup"><span data-stu-id="140c6-103">imageInfo resource type</span></span>

<span data-ttu-id="140c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="140c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="140c6-105">Сложный тип для представления свойства " **атрибуты** " в части [висуалинфо](../resources/projectrome-visualinfo.md) объекта [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="140c6-105">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="140c6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="140c6-106">Properties</span></span>

|<span data-ttu-id="140c6-107">Имя</span><span class="sxs-lookup"><span data-stu-id="140c6-107">Name</span></span> | <span data-ttu-id="140c6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="140c6-108">Type</span></span> | <span data-ttu-id="140c6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="140c6-109">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="140c6-110">iconUrl</span><span class="sxs-lookup"><span data-stu-id="140c6-110">iconUrl</span></span> | <span data-ttu-id="140c6-111">String</span><span class="sxs-lookup"><span data-stu-id="140c6-111">String</span></span> | <span data-ttu-id="140c6-112">Необязательно URI, указывающий на значок, представляющий приложение, используемое для создания действия.</span><span class="sxs-lookup"><span data-stu-id="140c6-112">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="140c6-113">алтернатетекст</span><span class="sxs-lookup"><span data-stu-id="140c6-113">alternateText</span></span> | <span data-ttu-id="140c6-114">String</span><span class="sxs-lookup"><span data-stu-id="140c6-114">String</span></span> | <span data-ttu-id="140c6-115">Необязательно доступное для изображения содержимое с замещающим текстом</span><span class="sxs-lookup"><span data-stu-id="140c6-115">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="140c6-116">аддимажекуери</span><span class="sxs-lookup"><span data-stu-id="140c6-116">addImageQuery</span></span> | <span data-ttu-id="140c6-117">Логический</span><span class="sxs-lookup"><span data-stu-id="140c6-117">Boolean</span></span> | <span data-ttu-id="140c6-118">Необязательно параметр, указывающий на то, что сервер может динамически отображать изображение в ответ на параметризация.</span><span class="sxs-lookup"><span data-stu-id="140c6-118">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="140c6-119">Например, изображение с высокой контрастностью</span><span class="sxs-lookup"><span data-stu-id="140c6-119">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="140c6-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="140c6-120">JSON Representation</span></span>

<span data-ttu-id="140c6-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="140c6-121">Here is a JSON representation of the resource</span></span>

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
