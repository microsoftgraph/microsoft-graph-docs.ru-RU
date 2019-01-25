---
title: Тип ресурса диагностики
description: Сведения об ошибке или предупреждение для выполнения операции OneNote.
localization_priority: Normal
ms.openlocfilehash: ef495374f84e0df887198b38a5c8488987a59343
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509506"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="c5c00-103">Тип ресурса диагностики</span><span class="sxs-lookup"><span data-stu-id="c5c00-103">diagnostic resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5c00-104">Сведения об ошибке или предупреждение для выполнения операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="c5c00-104">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5c00-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5c00-105">JSON representation</span></span>

<span data-ttu-id="c5c00-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c5c00-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a><span data-ttu-id="c5c00-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5c00-107">Properties</span></span>
| <span data-ttu-id="c5c00-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5c00-108">Property</span></span>     | <span data-ttu-id="c5c00-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c5c00-109">Type</span></span>   |<span data-ttu-id="c5c00-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c5c00-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5c00-111">message</span><span class="sxs-lookup"><span data-stu-id="c5c00-111">message</span></span>|<span data-ttu-id="c5c00-112">String</span><span class="sxs-lookup"><span data-stu-id="c5c00-112">String</span></span>|<span data-ttu-id="c5c00-113">Сообщение, описывающее условие, инициирующую сообщение об ошибке или предупреждение.</span><span class="sxs-lookup"><span data-stu-id="c5c00-113">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="c5c00-114">url</span><span class="sxs-lookup"><span data-stu-id="c5c00-114">url</span></span>|<span data-ttu-id="c5c00-115">String</span><span class="sxs-lookup"><span data-stu-id="c5c00-115">String</span></span>|<span data-ttu-id="c5c00-116">Ссылка на документацию для этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="c5c00-116">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/diagnostic.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
