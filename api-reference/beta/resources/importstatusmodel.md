---
title: Тип ресурса Импортстатусмодел
description: Ниже показано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: c3fe64245d0fbce98db3ba87c3c39694e998c7e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548539"
---
# <a name="importstatusmodel-resource-type"></a><span data-ttu-id="c91cd-103">Тип ресурса Импортстатусмодел</span><span class="sxs-lookup"><span data-stu-id="c91cd-103">importStatusModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="c91cd-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c91cd-104">JSON representation</span></span>

<span data-ttu-id="c91cd-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c91cd-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.importstatusmodel"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "string",
  "status": "string"
}

```
## <a name="properties"></a><span data-ttu-id="c91cd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c91cd-106">Properties</span></span>
| <span data-ttu-id="c91cd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c91cd-107">Property</span></span>     | <span data-ttu-id="c91cd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c91cd-108">Type</span></span>   |<span data-ttu-id="c91cd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c91cd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c91cd-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c91cd-110">createdDateTime</span></span>| <span data-ttu-id="c91cd-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c91cd-111">DateTimeOffset</span></span> ||
|<span data-ttu-id="c91cd-112">id</span><span class="sxs-lookup"><span data-stu-id="c91cd-112">id</span></span>|<span data-ttu-id="c91cd-113">string</span><span class="sxs-lookup"><span data-stu-id="c91cd-113">string</span></span>||
|<span data-ttu-id="c91cd-114">status</span><span class="sxs-lookup"><span data-stu-id="c91cd-114">status</span></span>|<span data-ttu-id="c91cd-115">string</span><span class="sxs-lookup"><span data-stu-id="c91cd-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "importStatusModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/importstatusmodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
