---
title: Тип ресурса диагностики
description: Сведения об ошибке или предупреждении для операции OneNote.
localization_priority: Normal
ms.openlocfilehash: ef495374f84e0df887198b38a5c8488987a59343
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535216"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="1d9a2-103">Тип ресурса диагностики</span><span class="sxs-lookup"><span data-stu-id="1d9a2-103">diagnostic resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d9a2-104">Сведения об ошибке или предупреждении для операции OneNote.</span><span class="sxs-lookup"><span data-stu-id="1d9a2-104">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d9a2-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d9a2-105">JSON representation</span></span>

<span data-ttu-id="1d9a2-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="1d9a2-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="1d9a2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d9a2-107">Properties</span></span>
| <span data-ttu-id="1d9a2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d9a2-108">Property</span></span>     | <span data-ttu-id="1d9a2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1d9a2-109">Type</span></span>   |<span data-ttu-id="1d9a2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1d9a2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d9a2-111">message</span><span class="sxs-lookup"><span data-stu-id="1d9a2-111">message</span></span>|<span data-ttu-id="1d9a2-112">String</span><span class="sxs-lookup"><span data-stu-id="1d9a2-112">String</span></span>|<span data-ttu-id="1d9a2-113">Сообщение с описанием условия, вызвавшего ошибку или предупреждение.</span><span class="sxs-lookup"><span data-stu-id="1d9a2-113">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="1d9a2-114">url</span><span class="sxs-lookup"><span data-stu-id="1d9a2-114">url</span></span>|<span data-ttu-id="1d9a2-115">String</span><span class="sxs-lookup"><span data-stu-id="1d9a2-115">String</span></span>|<span data-ttu-id="1d9a2-116">Ссылка на документацию по этой ошибке.</span><span class="sxs-lookup"><span data-stu-id="1d9a2-116">The link to the documentation for this issue.</span></span>|

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
