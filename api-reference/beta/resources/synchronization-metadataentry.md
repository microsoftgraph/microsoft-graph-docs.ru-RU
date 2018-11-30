---
title: Тип ресурса metadataEntry
description: Метаданные для данного объекта.
ms.openlocfilehash: 8fed980c5310b0a9f13a6f3269dde90fad083751
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075595"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="dbef6-103">Тип ресурса metadataEntry</span><span class="sxs-lookup"><span data-stu-id="dbef6-103">metadataEntry resource type</span></span>

> <span data-ttu-id="dbef6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dbef6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbef6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbef6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbef6-106">Метаданные для данного объекта.</span><span class="sxs-lookup"><span data-stu-id="dbef6-106">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="dbef6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbef6-107">Properties</span></span>
| <span data-ttu-id="dbef6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbef6-108">Property</span></span>     | <span data-ttu-id="dbef6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dbef6-109">Type</span></span>   |<span data-ttu-id="dbef6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dbef6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbef6-111">key</span><span class="sxs-lookup"><span data-stu-id="dbef6-111">key</span></span>|<span data-ttu-id="dbef6-112">String</span><span class="sxs-lookup"><span data-stu-id="dbef6-112">String</span></span>|<span data-ttu-id="dbef6-113">Имя свойства метаданных.</span><span class="sxs-lookup"><span data-stu-id="dbef6-113">Name of the metadata property.</span></span>|
|<span data-ttu-id="dbef6-114">value</span><span class="sxs-lookup"><span data-stu-id="dbef6-114">value</span></span>|<span data-ttu-id="dbef6-115">String</span><span class="sxs-lookup"><span data-stu-id="dbef6-115">String</span></span>|<span data-ttu-id="dbef6-116">Значение свойства метаданных.</span><span class="sxs-lookup"><span data-stu-id="dbef6-116">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbef6-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dbef6-117">JSON representation</span></span>

<span data-ttu-id="dbef6-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dbef6-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->