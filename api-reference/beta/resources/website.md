---
title: тип ресурса website
description: Представляет веб-сайта.
localization_priority: Normal
ms.openlocfilehash: 3f8aadaf0a6b6beb2394664f04195267062dc9ae
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641248"
---
# <a name="website-resource-type"></a><span data-ttu-id="4b071-103">тип ресурса website</span><span class="sxs-lookup"><span data-stu-id="4b071-103">website resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b071-104">Представляет веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="4b071-104">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="4b071-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b071-105">Properties</span></span>
| <span data-ttu-id="4b071-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b071-106">Property</span></span>     | <span data-ttu-id="4b071-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4b071-107">Type</span></span>   |<span data-ttu-id="4b071-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4b071-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b071-109">type</span><span class="sxs-lookup"><span data-stu-id="4b071-109">type</span></span>|<span data-ttu-id="4b071-110">String</span><span class="sxs-lookup"><span data-stu-id="4b071-110">String</span></span>| <span data-ttu-id="4b071-111">Возможные значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="4b071-111">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="4b071-112">address</span><span class="sxs-lookup"><span data-stu-id="4b071-112">address</span></span>|<span data-ttu-id="4b071-113">строка</span><span class="sxs-lookup"><span data-stu-id="4b071-113">string</span></span>|<span data-ttu-id="4b071-114">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="4b071-114">The URL of the website.</span></span>|
|<span data-ttu-id="4b071-115">displayName</span><span class="sxs-lookup"><span data-stu-id="4b071-115">displayName</span></span>|<span data-ttu-id="4b071-116">строка</span><span class="sxs-lookup"><span data-stu-id="4b071-116">string</span></span>|<span data-ttu-id="4b071-117">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="4b071-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b071-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4b071-118">JSON representation</span></span>

<span data-ttu-id="4b071-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b071-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/website.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
