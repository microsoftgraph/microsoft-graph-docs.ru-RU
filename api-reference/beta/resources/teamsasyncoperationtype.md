---
title: тип перечисления объекта teamsasyncoperationtype
description: Типы Теамсасинкоператион. Элементы будут добавлены здесь, так как поддерживаются дополнительные асинхронные операции.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4de95db194bf41939521b53f06614b46b6afae99
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553640"
---
# <a name="teamsasyncoperationtype-enum-type"></a><span data-ttu-id="0a60d-104">тип перечисления объекта teamsasyncoperationtype</span><span class="sxs-lookup"><span data-stu-id="0a60d-104">teamsAsyncOperationType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a60d-105">Типы [теамсасинкоператион](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0a60d-105">Types of [teamsAsyncOperation](teamsasyncoperation.md).</span></span> <span data-ttu-id="0a60d-106">Элементы будут добавлены здесь, так как поддерживаются дополнительные асинхронные операции.</span><span class="sxs-lookup"><span data-stu-id="0a60d-106">Members will be added here as more async operations are supported.</span></span>

## <a name="members"></a><span data-ttu-id="0a60d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="0a60d-107">Members</span></span>

| <span data-ttu-id="0a60d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="0a60d-108">Member</span></span> | <span data-ttu-id="0a60d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="0a60d-109">Value</span></span>| <span data-ttu-id="0a60d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0a60d-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0a60d-111">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="0a60d-111">invalid</span></span>|<span data-ttu-id="0a60d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="0a60d-112">0</span></span>|<span data-ttu-id="0a60d-113">Недопустимое значение.</span><span class="sxs-lookup"><span data-stu-id="0a60d-113">Invalid value.</span></span>|
|<span data-ttu-id="0a60d-114">Клонетеам</span><span class="sxs-lookup"><span data-stu-id="0a60d-114">cloneTeam</span></span>|<span data-ttu-id="0a60d-115">1 </span><span class="sxs-lookup"><span data-stu-id="0a60d-115">1</span></span>|<span data-ttu-id="0a60d-116">Операция клонирования команды.</span><span class="sxs-lookup"><span data-stu-id="0a60d-116">Operation to clone a team.</span></span>|
|<span data-ttu-id="0a60d-117">Арчиветеам</span><span class="sxs-lookup"><span data-stu-id="0a60d-117">archiveTeam</span></span>|<span data-ttu-id="0a60d-118">2 </span><span class="sxs-lookup"><span data-stu-id="0a60d-118">2</span></span>|<span data-ttu-id="0a60d-119">Операция архивации команды.</span><span class="sxs-lookup"><span data-stu-id="0a60d-119">Operation to archive a team.</span></span>|
|<span data-ttu-id="0a60d-120">Унарчиветеам</span><span class="sxs-lookup"><span data-stu-id="0a60d-120">unarchiveTeam</span></span>|<span data-ttu-id="0a60d-121">3 </span><span class="sxs-lookup"><span data-stu-id="0a60d-121">3</span></span>|<span data-ttu-id="0a60d-122">Операция восстановления архивной команды.</span><span class="sxs-lookup"><span data-stu-id="0a60d-122">Operation to restore an archived team.</span></span>|
|<span data-ttu-id="0a60d-123">Креатетеам</span><span class="sxs-lookup"><span data-stu-id="0a60d-123">createTeam</span></span>|<span data-ttu-id="0a60d-124">3 </span><span class="sxs-lookup"><span data-stu-id="0a60d-124">3</span></span>|<span data-ttu-id="0a60d-125">Операция по созданию команды с нуля.</span><span class="sxs-lookup"><span data-stu-id="0a60d-125">Operation to create a team from scratch.</span></span>|

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
