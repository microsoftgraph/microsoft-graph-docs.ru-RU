---
title: Тип ресурса imageInfo
description: Сложный тип для представления свойство **атрибуты** в части visualInfo объекта активности.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 347e07b70e8bad6dce8571dd1fbac5cd00d9abdd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978692"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="65e07-103">Тип ресурса imageInfo</span><span class="sxs-lookup"><span data-stu-id="65e07-103">imageInfo resource type</span></span>

> <span data-ttu-id="65e07-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="65e07-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65e07-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65e07-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65e07-106">Сложный тип для представления свойство **атрибуты** в части [visualInfo](../resources/projectrome-visualinfo.md) объекта [активности](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="65e07-106">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="65e07-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="65e07-107">Properties</span></span>

|<span data-ttu-id="65e07-108">Имя</span><span class="sxs-lookup"><span data-stu-id="65e07-108">Name</span></span> | <span data-ttu-id="65e07-109">Тип</span><span class="sxs-lookup"><span data-stu-id="65e07-109">Type</span></span> | <span data-ttu-id="65e07-110">Описание</span><span class="sxs-lookup"><span data-stu-id="65e07-110">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="65e07-111">iconUrl</span><span class="sxs-lookup"><span data-stu-id="65e07-111">iconUrl</span></span> | <span data-ttu-id="65e07-112">Строка</span><span class="sxs-lookup"><span data-stu-id="65e07-112">String</span></span> | <span data-ttu-id="65e07-113">Необязательный; URI, указывающий на значок, представляющий приложение, используемый для создания операции</span><span class="sxs-lookup"><span data-stu-id="65e07-113">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="65e07-114">alternateText</span><span class="sxs-lookup"><span data-stu-id="65e07-114">alternateText</span></span> | <span data-ttu-id="65e07-115">Строка</span><span class="sxs-lookup"><span data-stu-id="65e07-115">String</span></span> | <span data-ttu-id="65e07-116">Необязательный; Замещающий текст доступного содержимого для образа</span><span class="sxs-lookup"><span data-stu-id="65e07-116">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="65e07-117">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="65e07-117">addImageQuery</span></span> | <span data-ttu-id="65e07-118">Логический</span><span class="sxs-lookup"><span data-stu-id="65e07-118">Boolean</span></span> | <span data-ttu-id="65e07-119">Необязательный; параметр служит для указания сервера может отобразить изображение динамически в ответ на параметризации.</span><span class="sxs-lookup"><span data-stu-id="65e07-119">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="65e07-120">Для примера — изображение высокой контрастности</span><span class="sxs-lookup"><span data-stu-id="65e07-120">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65e07-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65e07-121">JSON Representation</span></span>

<span data-ttu-id="65e07-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65e07-122">Here is a JSON representation of the resource</span></span>

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
