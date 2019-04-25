---
title: Тип ресурса Едукатионлинкресаурце
description: Подкласс объекта Едукатионресаурце. Этот ресурс является ссылкой и не имеет дополнительных данных, связанных с ней.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 09e7c7c5070d6f8f288dbf18d6fb9ce81b456092
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542884"
---
# <a name="educationlinkresource-resource-type"></a><span data-ttu-id="4efba-104">Тип ресурса Едукатионлинкресаурце</span><span class="sxs-lookup"><span data-stu-id="4efba-104">educationLinkResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4efba-105">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="4efba-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="4efba-106">Этот ресурс является ссылкой и не имеет дополнительных данных, связанных с ней.</span><span class="sxs-lookup"><span data-stu-id="4efba-106">This resource is a link and does not have any additional data associated with it.</span></span>


## <a name="properties"></a><span data-ttu-id="4efba-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4efba-107">Properties</span></span>
| <span data-ttu-id="4efba-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4efba-108">Property</span></span>     | <span data-ttu-id="4efba-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4efba-109">Type</span></span>   |<span data-ttu-id="4efba-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4efba-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4efba-111">ссылка</span><span class="sxs-lookup"><span data-stu-id="4efba-111">link</span></span>|<span data-ttu-id="4efba-112">String</span><span class="sxs-lookup"><span data-stu-id="4efba-112">String</span></span>|<span data-ttu-id="4efba-113">URL-адрес ресурса.</span><span class="sxs-lookup"><span data-stu-id="4efba-113">URL to the resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4efba-114">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4efba-114">JSON representation</span></span>

<span data-ttu-id="4efba-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4efba-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationlinkresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
