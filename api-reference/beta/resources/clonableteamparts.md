---
title: Тип перечисления clonableTeamParts
description: 'Описывается, какие часть команды должны клонируется. '
localization_priority: Normal
ms.openlocfilehash: 3169d6e367484248e581c12c38887e07cf5c95af
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511466"
---
# <a name="clonableteamparts-enum-type"></a><span data-ttu-id="a81dc-103">Тип перечисления clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="a81dc-103">clonableTeamParts enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a81dc-104">Описывается, какие части [группы](../resources/team.md) должны клонировании.</span><span class="sxs-lookup"><span data-stu-id="a81dc-104">Describes which part of a [team](../resources/team.md) should be cloned.</span></span> 

## <a name="members"></a><span data-ttu-id="a81dc-105">Элементы</span><span class="sxs-lookup"><span data-stu-id="a81dc-105">Members</span></span>

| <span data-ttu-id="a81dc-106">Элемент</span><span class="sxs-lookup"><span data-stu-id="a81dc-106">Member</span></span> | <span data-ttu-id="a81dc-107">Значение</span><span class="sxs-lookup"><span data-stu-id="a81dc-107">Value</span></span>| <span data-ttu-id="a81dc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a81dc-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a81dc-109">apps</span><span class="sxs-lookup"><span data-stu-id="a81dc-109">apps</span></span>|<span data-ttu-id="a81dc-110">$1</span><span class="sxs-lookup"><span data-stu-id="a81dc-110">1</span></span>|<span data-ttu-id="a81dc-111">Скопируйте список установленных приложениях.</span><span class="sxs-lookup"><span data-stu-id="a81dc-111">Copy the list of installed apps.</span></span>|
|<span data-ttu-id="a81dc-112">Tabs</span><span class="sxs-lookup"><span data-stu-id="a81dc-112">tabs</span></span>|<span data-ttu-id="a81dc-113">–2</span><span class="sxs-lookup"><span data-stu-id="a81dc-113">2</span></span>|<span data-ttu-id="a81dc-114">Копирует вкладок между каналами.</span><span class="sxs-lookup"><span data-stu-id="a81dc-114">copies the tabs within channels.</span></span>|
|<span data-ttu-id="a81dc-115">settings</span><span class="sxs-lookup"><span data-stu-id="a81dc-115">settings</span></span>|<span data-ttu-id="a81dc-116">4</span><span class="sxs-lookup"><span data-stu-id="a81dc-116">4</span></span>|<span data-ttu-id="a81dc-117">Копирует все параметры в рамках рабочей группы, а также параметры ключа группы.</span><span class="sxs-lookup"><span data-stu-id="a81dc-117">Copies all settings within the team, along with key group settings.</span></span>|
|<span data-ttu-id="a81dc-118">каналы</span><span class="sxs-lookup"><span data-stu-id="a81dc-118">channels</span></span>|<span data-ttu-id="a81dc-119">: = 8</span><span class="sxs-lookup"><span data-stu-id="a81dc-119">8</span></span>|<span data-ttu-id="a81dc-120">Копирует структуру канала (но не сообщения в канале).</span><span class="sxs-lookup"><span data-stu-id="a81dc-120">copies the channel structure (but not the messages in the channel).</span></span>|
|<span data-ttu-id="a81dc-121">members</span><span class="sxs-lookup"><span data-stu-id="a81dc-121">members</span></span>|<span data-ttu-id="a81dc-122">1.6</span><span class="sxs-lookup"><span data-stu-id="a81dc-122">16</span></span>|<span data-ttu-id="a81dc-123">Копирует участников и владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="a81dc-123">copies the members and owners of the team.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/clonableteamparts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
