---
title: Тип ресурса addIn
description: Ниже показано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: d2a63d4428cbb3bcc7cc169711eb6cc6b9e00a6f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522331"
---
# <a name="addin-resource-type"></a><span data-ttu-id="0b757-103">Тип ресурса addIn</span><span class="sxs-lookup"><span data-stu-id="0b757-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="0b757-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b757-104">JSON representation</span></span>

<span data-ttu-id="0b757-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b757-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyvalue"}],
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="0b757-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b757-106">Properties</span></span>
| <span data-ttu-id="0b757-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b757-107">Property</span></span>     | <span data-ttu-id="0b757-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0b757-108">Type</span></span>   |<span data-ttu-id="0b757-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0b757-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b757-110">id</span><span class="sxs-lookup"><span data-stu-id="0b757-110">id</span></span>|<span data-ttu-id="0b757-111">Guid</span><span class="sxs-lookup"><span data-stu-id="0b757-111">guid</span></span>||
|<span data-ttu-id="0b757-112">properties</span><span class="sxs-lookup"><span data-stu-id="0b757-112">properties</span></span>|<span data-ttu-id="0b757-113">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0b757-113">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="0b757-114">type</span><span class="sxs-lookup"><span data-stu-id="0b757-114">type</span></span>|<span data-ttu-id="0b757-115">строка</span><span class="sxs-lookup"><span data-stu-id="0b757-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/addin.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
