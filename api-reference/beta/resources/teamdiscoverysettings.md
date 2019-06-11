---
title: Тип ресурса Теамдисковерисеттингс
description: Параметры, позволяющие настроить обнаружение команды другими пользователями.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 56284b678dec74e00724eeb429958aa54444208d
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2019
ms.locfileid: "34818707"
---
# <a name="teamdiscoverysettings-resource-type"></a><span data-ttu-id="3593d-103">Тип ресурса Теамдисковерисеттингс</span><span class="sxs-lookup"><span data-stu-id="3593d-103">teamDiscoverySettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3593d-104">Предоставляет параметры, позволяющие другим пользователям настраивать обнаружение [команды](team.md) .</span><span class="sxs-lookup"><span data-stu-id="3593d-104">Provides settings to enable others to configure [team](team.md) discoverability.</span></span> <span data-ttu-id="3593d-105">Параметры обнаружения можно изменять только для частных Teams.</span><span class="sxs-lookup"><span data-stu-id="3593d-105">You can only modify discovery settings for private teams.</span></span>

## <a name="properties"></a><span data-ttu-id="3593d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3593d-106">Properties</span></span>
| <span data-ttu-id="3593d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3593d-107">Property</span></span>     | <span data-ttu-id="3593d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3593d-108">Type</span></span>   |<span data-ttu-id="3593d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3593d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3593d-110">Шовинтеамссеарчандсугжестионс</span><span class="sxs-lookup"><span data-stu-id="3593d-110">showInTeamsSearchAndSuggestions</span></span>|<span data-ttu-id="3593d-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="3593d-111">Boolean</span></span>|<span data-ttu-id="3593d-112">Если задано значение true, команда становится видимой через поиск и предложения от клиента Teams.</span><span class="sxs-lookup"><span data-stu-id="3593d-112">If set to true, the team is visible via search and suggestions from the Teams client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3593d-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3593d-113">JSON representation</span></span>

<span data-ttu-id="3593d-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3593d-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamDiscoverySettings"
}-->

```json
{
  "showInTeamsSearchAndSuggestions": true
}
```

<!-- uuid: f1d42106-0b3d-4930-9f19-d76f4e03b36b
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's discoverySettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamdiscoverysettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
