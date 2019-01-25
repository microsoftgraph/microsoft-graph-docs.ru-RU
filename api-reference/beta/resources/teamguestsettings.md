---
title: Тип ресурса teamGuestSettings
description: Параметры для настройки ли гости могут создать, обновить или удалить каналы рабочих групп.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 4d76ffcbc5ec675ee670394854183c07721c0af9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522310"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="9b269-103">Тип ресурса teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="9b269-103">teamGuestSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b269-104">Параметры для настройки ли гости могут создать, обновить или удалить каналы в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="9b269-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9b269-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b269-105">Properties</span></span>
| <span data-ttu-id="9b269-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b269-106">Property</span></span>     | <span data-ttu-id="9b269-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9b269-107">Type</span></span>   |<span data-ttu-id="9b269-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9b269-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b269-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="9b269-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="9b269-110">Логическое</span><span class="sxs-lookup"><span data-stu-id="9b269-110">Boolean</span></span>|<span data-ttu-id="9b269-111">Если параметр имеет значение true, Гости можно добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="9b269-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="9b269-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="9b269-112">allowDeleteChannels</span></span>|<span data-ttu-id="9b269-113">Логическое</span><span class="sxs-lookup"><span data-stu-id="9b269-113">Boolean</span></span>|<span data-ttu-id="9b269-114">Если параметр имеет значение true, гости могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="9b269-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b269-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b269-115">JSON representation</span></span>

<span data-ttu-id="9b269-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b269-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamguestsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
