---
title: Тип перечисления teamsAsyncOperationStatus
description: Описывает текущее состояние teamsAsyncOperation.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e9138adcc646677955a12091a3fb15badfd39f13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511711"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="07da5-103">Тип перечисления teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="07da5-103">teamsAsyncOperationStatus enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07da5-104">Описывает текущее состояние [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="07da5-104">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="07da5-105">Элементы</span><span class="sxs-lookup"><span data-stu-id="07da5-105">Members</span></span>

| <span data-ttu-id="07da5-106">Элемент</span><span class="sxs-lookup"><span data-stu-id="07da5-106">Member</span></span> | <span data-ttu-id="07da5-107">Значение</span><span class="sxs-lookup"><span data-stu-id="07da5-107">Value</span></span>| <span data-ttu-id="07da5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="07da5-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="07da5-109">Invalid</span><span class="sxs-lookup"><span data-stu-id="07da5-109">invalid</span></span>|<span data-ttu-id="07da5-110">(0)</span><span class="sxs-lookup"><span data-stu-id="07da5-110">0</span></span>|<span data-ttu-id="07da5-111">Недопустимое значение</span><span class="sxs-lookup"><span data-stu-id="07da5-111">Invalid value.</span></span>|
|<span data-ttu-id="07da5-112">notStarted</span><span class="sxs-lookup"><span data-stu-id="07da5-112">notStarted</span></span>|<span data-ttu-id="07da5-113">$1</span><span class="sxs-lookup"><span data-stu-id="07da5-113">1</span></span>|<span data-ttu-id="07da5-114">Эта операция не запущена.</span><span class="sxs-lookup"><span data-stu-id="07da5-114">The operation has not started.</span></span>|
|<span data-ttu-id="07da5-115">InProgress</span><span class="sxs-lookup"><span data-stu-id="07da5-115">inProgress</span></span>|<span data-ttu-id="07da5-116">–2</span><span class="sxs-lookup"><span data-stu-id="07da5-116">2</span></span>|<span data-ttu-id="07da5-117">Выполнение операции.</span><span class="sxs-lookup"><span data-stu-id="07da5-117">The operation is running.</span></span>|
|<span data-ttu-id="07da5-118">succeeded</span><span class="sxs-lookup"><span data-stu-id="07da5-118">succeeded</span></span>|<span data-ttu-id="07da5-119">–3</span><span class="sxs-lookup"><span data-stu-id="07da5-119">3</span></span>|<span data-ttu-id="07da5-120">Операция успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="07da5-120">The operation succeeded.</span></span>|
|<span data-ttu-id="07da5-121">failed</span><span class="sxs-lookup"><span data-stu-id="07da5-121">failed</span></span>|<span data-ttu-id="07da5-122">4</span><span class="sxs-lookup"><span data-stu-id="07da5-122">4</span></span>|<span data-ttu-id="07da5-123">Сбой операции.</span><span class="sxs-lookup"><span data-stu-id="07da5-123">The operation failed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
