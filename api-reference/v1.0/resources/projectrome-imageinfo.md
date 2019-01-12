---
title: Тип ресурса imageInfo
description: Сложный тип для представления свойство **атрибуты** в части visualInfo объекта активности.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: a17fe40f53308a0b1b1f587425d2afb019f84bb5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982367"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="1fc9a-103">Тип ресурса imageInfo</span><span class="sxs-lookup"><span data-stu-id="1fc9a-103">imageInfo resource type</span></span>

<span data-ttu-id="1fc9a-104">Сложный тип для представления свойство **атрибуты** в части [visualInfo](../resources/projectrome-visualinfo.md) объекта [активности](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="1fc9a-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="1fc9a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1fc9a-105">Properties</span></span>

|<span data-ttu-id="1fc9a-106">Имя</span><span class="sxs-lookup"><span data-stu-id="1fc9a-106">Name</span></span> | <span data-ttu-id="1fc9a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1fc9a-107">Type</span></span> | <span data-ttu-id="1fc9a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1fc9a-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="1fc9a-109">iconUrl</span><span class="sxs-lookup"><span data-stu-id="1fc9a-109">iconUrl</span></span> | <span data-ttu-id="1fc9a-110">Строка</span><span class="sxs-lookup"><span data-stu-id="1fc9a-110">String</span></span> | <span data-ttu-id="1fc9a-111">Необязательный; URI, указывающий на значок, представляющий приложение, используемый для создания операции</span><span class="sxs-lookup"><span data-stu-id="1fc9a-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="1fc9a-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="1fc9a-112">alternateText</span></span> | <span data-ttu-id="1fc9a-113">Строка</span><span class="sxs-lookup"><span data-stu-id="1fc9a-113">String</span></span> | <span data-ttu-id="1fc9a-114">Необязательный; Замещающий текст доступного содержимого для образа</span><span class="sxs-lookup"><span data-stu-id="1fc9a-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="1fc9a-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="1fc9a-115">addImageQuery</span></span> | <span data-ttu-id="1fc9a-116">Логический</span><span class="sxs-lookup"><span data-stu-id="1fc9a-116">Boolean</span></span> | <span data-ttu-id="1fc9a-117">Необязательный; параметр служит для указания сервера может отобразить изображение динамически в ответ на параметризации.</span><span class="sxs-lookup"><span data-stu-id="1fc9a-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="1fc9a-118">Для примера — изображение высокой контрастности</span><span class="sxs-lookup"><span data-stu-id="1fc9a-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fc9a-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1fc9a-119">JSON Representation</span></span>

<span data-ttu-id="1fc9a-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1fc9a-120">Here is a JSON representation of the resource</span></span>

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
