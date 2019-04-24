---
title: Тип ресурса Митингкапабилити
description: Содержит возможности собрания
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e71d7c8c6489d5856e5f2441cd93c7fdea033bd4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457146"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="8098f-103">Тип ресурса Митингкапабилити</span><span class="sxs-lookup"><span data-stu-id="8098f-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8098f-104">Содержит возможности собрания</span><span class="sxs-lookup"><span data-stu-id="8098f-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="8098f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8098f-105">Properties</span></span>

| <span data-ttu-id="8098f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8098f-106">Property</span></span>                          | <span data-ttu-id="8098f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8098f-107">Type</span></span>    | <span data-ttu-id="8098f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8098f-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="8098f-109">Аллованонимаусусерстодиалаут</span><span class="sxs-lookup"><span data-stu-id="8098f-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="8098f-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="8098f-110">Boolean</span></span> | <span data-ttu-id="8098f-111">Указывает, разрешено ли исходящие вызовы анонимных пользователей на собрании.</span><span class="sxs-lookup"><span data-stu-id="8098f-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="8098f-112">Аллованонимаусусерстостартмитинг</span><span class="sxs-lookup"><span data-stu-id="8098f-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="8098f-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8098f-113">Boolean</span></span> | <span data-ttu-id="8098f-114">Указывает, разрешено ли анонимным пользователям начинать собрание.</span><span class="sxs-lookup"><span data-stu-id="8098f-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="8098f-115">Аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="8098f-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="8098f-116">String</span><span class="sxs-lookup"><span data-stu-id="8098f-116">String</span></span>  | <span data-ttu-id="8098f-117">Возможные значения: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="8098f-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="8098f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8098f-118">JSON representation</span></span>

<span data-ttu-id="8098f-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8098f-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "allowAnonymousUsersToStartMeeting": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingcapability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
