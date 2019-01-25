---
title: Тип ресурса meetingCapability
description: Содержит возможности собрания
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e71d7c8c6489d5856e5f2441cd93c7fdea033bd4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524291"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="9bd19-103">Тип ресурса meetingCapability</span><span class="sxs-lookup"><span data-stu-id="9bd19-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bd19-104">Содержит возможности собрания</span><span class="sxs-lookup"><span data-stu-id="9bd19-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="9bd19-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9bd19-105">Properties</span></span>

| <span data-ttu-id="9bd19-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bd19-106">Property</span></span>                          | <span data-ttu-id="9bd19-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9bd19-107">Type</span></span>    | <span data-ttu-id="9bd19-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9bd19-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="9bd19-109">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="9bd19-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="9bd19-110">Логическое</span><span class="sxs-lookup"><span data-stu-id="9bd19-110">Boolean</span></span> | <span data-ttu-id="9bd19-111">Указывает, может ли анонимные пользователи исходящие звонки на собрании.</span><span class="sxs-lookup"><span data-stu-id="9bd19-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="9bd19-112">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="9bd19-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="9bd19-113">Логическое</span><span class="sxs-lookup"><span data-stu-id="9bd19-113">Boolean</span></span> | <span data-ttu-id="9bd19-114">Указывает, разрешены ли анонимные пользователи начало собрания.</span><span class="sxs-lookup"><span data-stu-id="9bd19-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="9bd19-115">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="9bd19-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="9bd19-116">String</span><span class="sxs-lookup"><span data-stu-id="9bd19-116">String</span></span>  | <span data-ttu-id="9bd19-117">Возможные значения: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="9bd19-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="9bd19-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9bd19-118">JSON representation</span></span>

<span data-ttu-id="9bd19-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bd19-119">The following is a JSON representation of the resource.</span></span>

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
