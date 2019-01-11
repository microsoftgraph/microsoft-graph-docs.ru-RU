---
title: Тип ресурса metadataEntry
description: Метаданные для данного объекта.
localization_priority: Normal
ms.openlocfilehash: ffdb2dd3b6729320b5991b1158e10d145e339968
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819483"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="785c2-103">Тип ресурса metadataEntry</span><span class="sxs-lookup"><span data-stu-id="785c2-103">metadataEntry resource type</span></span>

> <span data-ttu-id="785c2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="785c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="785c2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="785c2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="785c2-106">Метаданные для данного объекта.</span><span class="sxs-lookup"><span data-stu-id="785c2-106">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="785c2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="785c2-107">Properties</span></span>
| <span data-ttu-id="785c2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="785c2-108">Property</span></span>     | <span data-ttu-id="785c2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="785c2-109">Type</span></span>   |<span data-ttu-id="785c2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="785c2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="785c2-111">key</span><span class="sxs-lookup"><span data-stu-id="785c2-111">key</span></span>|<span data-ttu-id="785c2-112">Строка</span><span class="sxs-lookup"><span data-stu-id="785c2-112">String</span></span>|<span data-ttu-id="785c2-113">Имя свойства метаданных.</span><span class="sxs-lookup"><span data-stu-id="785c2-113">Name of the metadata property.</span></span>|
|<span data-ttu-id="785c2-114">value</span><span class="sxs-lookup"><span data-stu-id="785c2-114">value</span></span>|<span data-ttu-id="785c2-115">Строка</span><span class="sxs-lookup"><span data-stu-id="785c2-115">String</span></span>|<span data-ttu-id="785c2-116">Значение свойства метаданных.</span><span class="sxs-lookup"><span data-stu-id="785c2-116">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="785c2-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="785c2-117">JSON representation</span></span>

<span data-ttu-id="785c2-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="785c2-118">The following is a JSON representation of the resource.</span></span>

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
