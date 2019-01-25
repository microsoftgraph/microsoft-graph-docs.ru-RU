---
title: Тип перечисления teamsAsyncOperationType
description: Типы teamsAsyncOperation. Участники будут добавляться здесь дополнительных async поддерживают операции.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4de95db194bf41939521b53f06614b46b6afae99
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516569"
---
# <a name="teamsasyncoperationtype-enum-type"></a><span data-ttu-id="397f7-104">Тип перечисления teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="397f7-104">teamsAsyncOperationType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="397f7-105">Типы [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="397f7-105">Types of [teamsAsyncOperation](teamsasyncoperation.md).</span></span> <span data-ttu-id="397f7-106">Участники будут добавляться здесь дополнительных async поддерживают операции.</span><span class="sxs-lookup"><span data-stu-id="397f7-106">Members will be added here as more async operations are supported.</span></span>

## <a name="members"></a><span data-ttu-id="397f7-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="397f7-107">Members</span></span>

| <span data-ttu-id="397f7-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="397f7-108">Member</span></span> | <span data-ttu-id="397f7-109">Значение</span><span class="sxs-lookup"><span data-stu-id="397f7-109">Value</span></span>| <span data-ttu-id="397f7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="397f7-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="397f7-111">Invalid</span><span class="sxs-lookup"><span data-stu-id="397f7-111">invalid</span></span>|<span data-ttu-id="397f7-112">(0)</span><span class="sxs-lookup"><span data-stu-id="397f7-112">0</span></span>|<span data-ttu-id="397f7-113">Недопустимое значение</span><span class="sxs-lookup"><span data-stu-id="397f7-113">Invalid value.</span></span>|
|<span data-ttu-id="397f7-114">cloneTeam</span><span class="sxs-lookup"><span data-stu-id="397f7-114">cloneTeam</span></span>|<span data-ttu-id="397f7-115">$1</span><span class="sxs-lookup"><span data-stu-id="397f7-115">1</span></span>|<span data-ttu-id="397f7-116">Операция следует скопировать группы.</span><span class="sxs-lookup"><span data-stu-id="397f7-116">Operation to clone a team.</span></span>|
|<span data-ttu-id="397f7-117">archiveTeam</span><span class="sxs-lookup"><span data-stu-id="397f7-117">archiveTeam</span></span>|<span data-ttu-id="397f7-118">–2</span><span class="sxs-lookup"><span data-stu-id="397f7-118">2</span></span>|<span data-ttu-id="397f7-119">Операции в архив группы.</span><span class="sxs-lookup"><span data-stu-id="397f7-119">Operation to archive a team.</span></span>|
|<span data-ttu-id="397f7-120">unarchiveTeam</span><span class="sxs-lookup"><span data-stu-id="397f7-120">unarchiveTeam</span></span>|<span data-ttu-id="397f7-121">–3</span><span class="sxs-lookup"><span data-stu-id="397f7-121">3</span></span>|<span data-ttu-id="397f7-122">Операция восстановление архивированных группы.</span><span class="sxs-lookup"><span data-stu-id="397f7-122">Operation to restore an archived team.</span></span>|
|<span data-ttu-id="397f7-123">createTeam</span><span class="sxs-lookup"><span data-stu-id="397f7-123">createTeam</span></span>|<span data-ttu-id="397f7-124">–3</span><span class="sxs-lookup"><span data-stu-id="397f7-124">3</span></span>|<span data-ttu-id="397f7-125">Операция создать группу «с нуля».</span><span class="sxs-lookup"><span data-stu-id="397f7-125">Operation to create a team from scratch.</span></span>|

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
