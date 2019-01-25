---
title: Members
description: 'Описывает видимость группы. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7e77fbd2667f8656a4c2f66046636ff73ac8891d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521350"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="d0a10-103">Тип перечисления teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="d0a10-103">teamVisibilityType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0a10-104">Описывает видимость [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d0a10-104">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="d0a10-105">Элементы</span><span class="sxs-lookup"><span data-stu-id="d0a10-105">Members</span></span>

| <span data-ttu-id="d0a10-106">Элемент</span><span class="sxs-lookup"><span data-stu-id="d0a10-106">Member</span></span> | <span data-ttu-id="d0a10-107">Значение</span><span class="sxs-lookup"><span data-stu-id="d0a10-107">Value</span></span>| <span data-ttu-id="d0a10-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d0a10-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d0a10-109">Private</span><span class="sxs-lookup"><span data-stu-id="d0a10-109">private</span></span>|<span data-ttu-id="d0a10-110">(0)</span><span class="sxs-lookup"><span data-stu-id="d0a10-110">0</span></span>|<span data-ttu-id="d0a10-111">Любой пользователь может просматривать группы, но только владелец можно добавить пользователя в группу.</span><span class="sxs-lookup"><span data-stu-id="d0a10-111">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="d0a10-112">public</span><span class="sxs-lookup"><span data-stu-id="d0a10-112">public</span></span>|<span data-ttu-id="d0a10-113">$1</span><span class="sxs-lookup"><span data-stu-id="d0a10-113">1</span></span>|<span data-ttu-id="d0a10-114">Для присоединения к группе.</span><span class="sxs-lookup"><span data-stu-id="d0a10-114">Anyone can join the team.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamvisibilitytype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
