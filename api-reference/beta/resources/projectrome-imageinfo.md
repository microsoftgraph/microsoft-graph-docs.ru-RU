---
title: Тип ресурса imageInfo
description: Сложный тип для представления свойство **атрибуты** в части visualInfo объекта активности.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 112b1dc3d1db45f3fe470c1c21d483b09c00202c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514917"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="63cb6-103">Тип ресурса imageInfo</span><span class="sxs-lookup"><span data-stu-id="63cb6-103">imageInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63cb6-104">Сложный тип для представления свойство **атрибуты** в части [visualInfo](../resources/projectrome-visualinfo.md) объекта [активности](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="63cb6-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="63cb6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="63cb6-105">Properties</span></span>

|<span data-ttu-id="63cb6-106">Имя</span><span class="sxs-lookup"><span data-stu-id="63cb6-106">Name</span></span> | <span data-ttu-id="63cb6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="63cb6-107">Type</span></span> | <span data-ttu-id="63cb6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="63cb6-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="63cb6-109">IconUrl</span><span class="sxs-lookup"><span data-stu-id="63cb6-109">iconUrl</span></span> | <span data-ttu-id="63cb6-110">String</span><span class="sxs-lookup"><span data-stu-id="63cb6-110">String</span></span> | <span data-ttu-id="63cb6-111">Необязательный; URI, указывающий на значок, представляющий приложение, используемый для создания операции</span><span class="sxs-lookup"><span data-stu-id="63cb6-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="63cb6-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="63cb6-112">alternateText</span></span> | <span data-ttu-id="63cb6-113">String</span><span class="sxs-lookup"><span data-stu-id="63cb6-113">String</span></span> | <span data-ttu-id="63cb6-114">Необязательный; Замещающий текст доступного содержимого для образа</span><span class="sxs-lookup"><span data-stu-id="63cb6-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="63cb6-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="63cb6-115">addImageQuery</span></span> | <span data-ttu-id="63cb6-116">Логическое</span><span class="sxs-lookup"><span data-stu-id="63cb6-116">Boolean</span></span> | <span data-ttu-id="63cb6-117">Необязательный; параметр служит для указания сервера может отобразить изображение динамически в ответ на параметризации.</span><span class="sxs-lookup"><span data-stu-id="63cb6-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="63cb6-118">Для примера — изображение высокой контрастности</span><span class="sxs-lookup"><span data-stu-id="63cb6-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63cb6-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63cb6-119">JSON Representation</span></span>

<span data-ttu-id="63cb6-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63cb6-120">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-imageinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
