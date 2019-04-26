---
title: Тип ресурса Митингкапабилити
description: Содержит возможности собрания
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 55a577490ee4c40bbd4adcc63a7e4aa7f38c8dd1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342600"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="e1ac8-103">Тип ресурса Митингкапабилити</span><span class="sxs-lookup"><span data-stu-id="e1ac8-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1ac8-104">Содержит возможности собрания</span><span class="sxs-lookup"><span data-stu-id="e1ac8-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="e1ac8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1ac8-105">Properties</span></span>

| <span data-ttu-id="e1ac8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1ac8-106">Property</span></span>                          | <span data-ttu-id="e1ac8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e1ac8-107">Type</span></span>    | <span data-ttu-id="e1ac8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e1ac8-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="e1ac8-109">Аллованонимаусусерстодиалаут</span><span class="sxs-lookup"><span data-stu-id="e1ac8-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="e1ac8-110">Логический</span><span class="sxs-lookup"><span data-stu-id="e1ac8-110">Boolean</span></span> | <span data-ttu-id="e1ac8-111">Указывает, разрешено ли исходящие вызовы анонимных пользователей на собрании.</span><span class="sxs-lookup"><span data-stu-id="e1ac8-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="e1ac8-112">Аллованонимаусусерстостартмитинг</span><span class="sxs-lookup"><span data-stu-id="e1ac8-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="e1ac8-113">Логический</span><span class="sxs-lookup"><span data-stu-id="e1ac8-113">Boolean</span></span> | <span data-ttu-id="e1ac8-114">Указывает, разрешено ли анонимным пользователям начинать собрание.</span><span class="sxs-lookup"><span data-stu-id="e1ac8-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="e1ac8-115">Аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="e1ac8-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="e1ac8-116">String</span><span class="sxs-lookup"><span data-stu-id="e1ac8-116">String</span></span>  | <span data-ttu-id="e1ac8-117">Возможные значения: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="e1ac8-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="e1ac8-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1ac8-118">JSON representation</span></span>

<span data-ttu-id="e1ac8-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1ac8-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
