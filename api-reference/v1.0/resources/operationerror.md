---
title: Тип ресурса Оператионеррор
description: Описание ошибок в Теамсасинкоператион.
localization_priority: Normal
ms.openlocfilehash: 22590d7d955cf01385292d2796ad960b1c0ced41
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462608"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="aed84-103">Тип ресурса Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="aed84-103">operationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aed84-104">Описание ошибок в [теамсасинкоператион](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="aed84-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="aed84-105">Свойства Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="aed84-105">operationError Properties</span></span>
| <span data-ttu-id="aed84-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="aed84-106">Property</span></span>     | <span data-ttu-id="aed84-107">Тип</span><span class="sxs-lookup"><span data-stu-id="aed84-107">Type</span></span>   |<span data-ttu-id="aed84-108">Описание</span><span class="sxs-lookup"><span data-stu-id="aed84-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aed84-109">code</span><span class="sxs-lookup"><span data-stu-id="aed84-109">code</span></span>|<span data-ttu-id="aed84-110">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="aed84-110">string (readonly)</span></span>|<span data-ttu-id="aed84-111">Код ошибки операции.</span><span class="sxs-lookup"><span data-stu-id="aed84-111">Operation error code.</span></span>|
|<span data-ttu-id="aed84-112">message</span><span class="sxs-lookup"><span data-stu-id="aed84-112">message</span></span>|<span data-ttu-id="aed84-113">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="aed84-113">string (readonly)</span></span>|<span data-ttu-id="aed84-114">Сообщение об ошибке операции.</span><span class="sxs-lookup"><span data-stu-id="aed84-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aed84-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aed84-115">JSON representation</span></span>

<span data-ttu-id="aed84-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aed84-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/operationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
