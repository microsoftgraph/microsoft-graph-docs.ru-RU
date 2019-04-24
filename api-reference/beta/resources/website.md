---
title: Тип ресурса веб-сайта
description: Представляет веб-сайт.
localization_priority: Normal
ms.openlocfilehash: 3f8aadaf0a6b6beb2394664f04195267062dc9ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454046"
---
# <a name="website-resource-type"></a><span data-ttu-id="cb011-103">Тип ресурса веб-сайта</span><span class="sxs-lookup"><span data-stu-id="cb011-103">website resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb011-104">Представляет веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="cb011-104">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="cb011-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb011-105">Properties</span></span>
| <span data-ttu-id="cb011-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb011-106">Property</span></span>     | <span data-ttu-id="cb011-107">Тип</span><span class="sxs-lookup"><span data-stu-id="cb011-107">Type</span></span>   |<span data-ttu-id="cb011-108">Описание</span><span class="sxs-lookup"><span data-stu-id="cb011-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb011-109">type</span><span class="sxs-lookup"><span data-stu-id="cb011-109">type</span></span>|<span data-ttu-id="cb011-110">Строка</span><span class="sxs-lookup"><span data-stu-id="cb011-110">String</span></span>| <span data-ttu-id="cb011-111">Возможные значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="cb011-111">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="cb011-112">address</span><span class="sxs-lookup"><span data-stu-id="cb011-112">address</span></span>|<span data-ttu-id="cb011-113">string</span><span class="sxs-lookup"><span data-stu-id="cb011-113">string</span></span>|<span data-ttu-id="cb011-114">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="cb011-114">The URL of the website.</span></span>|
|<span data-ttu-id="cb011-115">displayName</span><span class="sxs-lookup"><span data-stu-id="cb011-115">displayName</span></span>|<span data-ttu-id="cb011-116">string</span><span class="sxs-lookup"><span data-stu-id="cb011-116">string</span></span>|<span data-ttu-id="cb011-117">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="cb011-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb011-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb011-118">JSON representation</span></span>

<span data-ttu-id="cb011-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb011-119">Here is a JSON representation of the resource.</span></span>

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
