---
title: Тип ресурса addIn
description: Ниже показано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: d2a63d4428cbb3bcc7cc169711eb6cc6b9e00a6f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535797"
---
# <a name="addin-resource-type"></a><span data-ttu-id="11608-103">Тип ресурса addIn</span><span class="sxs-lookup"><span data-stu-id="11608-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="11608-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="11608-104">JSON representation</span></span>

<span data-ttu-id="11608-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11608-105">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="11608-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="11608-106">Properties</span></span>
| <span data-ttu-id="11608-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="11608-107">Property</span></span>     | <span data-ttu-id="11608-108">Тип</span><span class="sxs-lookup"><span data-stu-id="11608-108">Type</span></span>   |<span data-ttu-id="11608-109">Описание</span><span class="sxs-lookup"><span data-stu-id="11608-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11608-110">id</span><span class="sxs-lookup"><span data-stu-id="11608-110">id</span></span>|<span data-ttu-id="11608-111">кодом</span><span class="sxs-lookup"><span data-stu-id="11608-111">guid</span></span>||
|<span data-ttu-id="11608-112">properties</span><span class="sxs-lookup"><span data-stu-id="11608-112">properties</span></span>|<span data-ttu-id="11608-113">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="11608-113">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="11608-114">type</span><span class="sxs-lookup"><span data-stu-id="11608-114">type</span></span>|<span data-ttu-id="11608-115">string</span><span class="sxs-lookup"><span data-stu-id="11608-115">string</span></span>||

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
