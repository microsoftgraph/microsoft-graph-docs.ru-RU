---
title: Тип ресурса teamDiscoverySettings
description: Параметры для настройки возможности обнаружения команды другими пользователями.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: edc3c6cc446e35f2f5a97212d3c0b6f69b81ce30
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292915"
---
# <a name="teamdiscoverysettings-resource-type"></a><span data-ttu-id="a8695-103">Тип ресурса teamDiscoverySettings</span><span class="sxs-lookup"><span data-stu-id="a8695-103">teamDiscoverySettings resource type</span></span>

<span data-ttu-id="a8695-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8695-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8695-105">Предоставляет параметры, позволяющие другим пользователям настраивать [возможность](team.md) обнаружения команд.</span><span class="sxs-lookup"><span data-stu-id="a8695-105">Provides settings to enable others to configure [team](team.md) discoverability.</span></span> <span data-ttu-id="a8695-106">Изменить параметры обнаружения можно только для закрытых команд.</span><span class="sxs-lookup"><span data-stu-id="a8695-106">You can only modify discovery settings for private teams.</span></span>

## <a name="properties"></a><span data-ttu-id="a8695-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8695-107">Properties</span></span>
| <span data-ttu-id="a8695-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8695-108">Property</span></span>     | <span data-ttu-id="a8695-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a8695-109">Type</span></span>   |<span data-ttu-id="a8695-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a8695-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8695-111">showInTeamsSearchAndSuggestions</span><span class="sxs-lookup"><span data-stu-id="a8695-111">showInTeamsSearchAndSuggestions</span></span>|<span data-ttu-id="a8695-112">Логический</span><span class="sxs-lookup"><span data-stu-id="a8695-112">Boolean</span></span>|<span data-ttu-id="a8695-113">Если за установлено true, команда будет видна с помощью поиска и предложений из клиента Teams.</span><span class="sxs-lookup"><span data-stu-id="a8695-113">If set to true, the team is visible via search and suggestions from the Teams client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8695-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8695-114">JSON representation</span></span>

<span data-ttu-id="a8695-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8695-115">The following is a JSON representation of the resource.</span></span>

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
  ]
}-->


