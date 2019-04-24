---
title: Members
description: 'Описывает видимость команды. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ea8868924681d3e8f8cd0b4f55ff947c085260e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456968"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="45dff-103">тип перечисления объекта teamvisibilitytype</span><span class="sxs-lookup"><span data-stu-id="45dff-103">teamVisibilityType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45dff-104">Описывает видимость [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="45dff-104">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="45dff-105">Элементы</span><span class="sxs-lookup"><span data-stu-id="45dff-105">Members</span></span>

| <span data-ttu-id="45dff-106">Элемент</span><span class="sxs-lookup"><span data-stu-id="45dff-106">Member</span></span> | <span data-ttu-id="45dff-107">Значение</span><span class="sxs-lookup"><span data-stu-id="45dff-107">Value</span></span>| <span data-ttu-id="45dff-108">Описание</span><span class="sxs-lookup"><span data-stu-id="45dff-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="45dff-109">закрытый</span><span class="sxs-lookup"><span data-stu-id="45dff-109">private</span></span>|<span data-ttu-id="45dff-110">нуль</span><span class="sxs-lookup"><span data-stu-id="45dff-110">0</span></span>|<span data-ttu-id="45dff-111">Любой пользователь может видеть команду, но только владелец может добавить в нее пользователя.</span><span class="sxs-lookup"><span data-stu-id="45dff-111">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="45dff-112">public</span><span class="sxs-lookup"><span data-stu-id="45dff-112">public</span></span>|<span data-ttu-id="45dff-113">1,1</span><span class="sxs-lookup"><span data-stu-id="45dff-113">1</span></span>|<span data-ttu-id="45dff-114">Любой пользователь может присоединиться к команде.</span><span class="sxs-lookup"><span data-stu-id="45dff-114">Anyone can join the team.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamvisibilitytype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
