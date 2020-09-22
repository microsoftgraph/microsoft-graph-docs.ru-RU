---
title: Тип ресурса Теамдисковерисеттингс
description: Параметры для настройки возможности обнаружения команды другими пользователями.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f26c47b2e1863c3108bc23f7c388179bd8006156
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046666"
---
# <a name="teamdiscoverysettings-resource-type"></a><span data-ttu-id="5f0e6-103">Тип ресурса Теамдисковерисеттингс</span><span class="sxs-lookup"><span data-stu-id="5f0e6-103">teamDiscoverySettings resource type</span></span>

<span data-ttu-id="5f0e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f0e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f0e6-105">Предоставляет параметры, позволяющие другим пользователям настраивать обнаружение [команды](team.md) .</span><span class="sxs-lookup"><span data-stu-id="5f0e6-105">Provides settings to enable others to configure [team](team.md) discoverability.</span></span> <span data-ttu-id="5f0e6-106">Параметры обнаружения можно изменять только для частных Teams.</span><span class="sxs-lookup"><span data-stu-id="5f0e6-106">You can only modify discovery settings for private teams.</span></span>

## <a name="properties"></a><span data-ttu-id="5f0e6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f0e6-107">Properties</span></span>
| <span data-ttu-id="5f0e6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f0e6-108">Property</span></span>     | <span data-ttu-id="5f0e6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5f0e6-109">Type</span></span>   |<span data-ttu-id="5f0e6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5f0e6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f0e6-111">шовинтеамссеарчандсугжестионс</span><span class="sxs-lookup"><span data-stu-id="5f0e6-111">showInTeamsSearchAndSuggestions</span></span>|<span data-ttu-id="5f0e6-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f0e6-112">Boolean</span></span>|<span data-ttu-id="5f0e6-113">Если задано значение true, команда становится видимой через поиск и предложения от клиента Teams.</span><span class="sxs-lookup"><span data-stu-id="5f0e6-113">If set to true, the team is visible via search and suggestions from the Teams client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f0e6-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f0e6-114">JSON representation</span></span>

<span data-ttu-id="5f0e6-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f0e6-115">The following is a JSON representation of the resource.</span></span>

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


