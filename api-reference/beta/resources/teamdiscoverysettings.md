---
title: Тип ресурса Теамдисковерисеттингс
description: Параметры для настройки возможности обнаружения команды другими пользователями.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9a668c9d3b234fede0ad5c151e1dbbc95fc93516
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519962"
---
# <a name="teamdiscoverysettings-resource-type"></a><span data-ttu-id="b7405-103">Тип ресурса Теамдисковерисеттингс</span><span class="sxs-lookup"><span data-stu-id="b7405-103">teamDiscoverySettings resource type</span></span>

<span data-ttu-id="b7405-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b7405-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7405-105">Предоставляет параметры, позволяющие другим пользователям настраивать обнаружение [команды](team.md) .</span><span class="sxs-lookup"><span data-stu-id="b7405-105">Provides settings to enable others to configure [team](team.md) discoverability.</span></span> <span data-ttu-id="b7405-106">Параметры обнаружения можно изменять только для частных Teams.</span><span class="sxs-lookup"><span data-stu-id="b7405-106">You can only modify discovery settings for private teams.</span></span>

## <a name="properties"></a><span data-ttu-id="b7405-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7405-107">Properties</span></span>
| <span data-ttu-id="b7405-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7405-108">Property</span></span>     | <span data-ttu-id="b7405-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b7405-109">Type</span></span>   |<span data-ttu-id="b7405-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b7405-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7405-111">шовинтеамссеарчандсугжестионс</span><span class="sxs-lookup"><span data-stu-id="b7405-111">showInTeamsSearchAndSuggestions</span></span>|<span data-ttu-id="b7405-112">Логический</span><span class="sxs-lookup"><span data-stu-id="b7405-112">Boolean</span></span>|<span data-ttu-id="b7405-113">Если задано значение true, команда становится видимой через поиск и предложения от клиента Teams.</span><span class="sxs-lookup"><span data-stu-id="b7405-113">If set to true, the team is visible via search and suggestions from the Teams client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7405-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7405-114">JSON representation</span></span>

<span data-ttu-id="b7405-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7405-115">The following is a JSON representation of the resource.</span></span>

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
