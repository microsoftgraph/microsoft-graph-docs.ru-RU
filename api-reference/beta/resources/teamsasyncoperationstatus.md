---
title: тип перечисления Теамсасинкоператионстатус
description: Описывает текущее состояние Теамсасинкоператион.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e9138adcc646677955a12091a3fb15badfd39f13
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578865"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="4d62e-103">тип перечисления Теамсасинкоператионстатус</span><span class="sxs-lookup"><span data-stu-id="4d62e-103">teamsAsyncOperationStatus enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d62e-104">Описывает текущее состояние [теамсасинкоператион](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="4d62e-104">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="4d62e-105">Элементы</span><span class="sxs-lookup"><span data-stu-id="4d62e-105">Members</span></span>

| <span data-ttu-id="4d62e-106">Элемент</span><span class="sxs-lookup"><span data-stu-id="4d62e-106">Member</span></span> | <span data-ttu-id="4d62e-107">Значение</span><span class="sxs-lookup"><span data-stu-id="4d62e-107">Value</span></span>| <span data-ttu-id="4d62e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4d62e-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4d62e-109">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="4d62e-109">invalid</span></span>|<span data-ttu-id="4d62e-110">нуль</span><span class="sxs-lookup"><span data-stu-id="4d62e-110">0</span></span>|<span data-ttu-id="4d62e-111">Недопустимое значение.</span><span class="sxs-lookup"><span data-stu-id="4d62e-111">Invalid value.</span></span>|
|<span data-ttu-id="4d62e-112">notStarted</span><span class="sxs-lookup"><span data-stu-id="4d62e-112">notStarted</span></span>|<span data-ttu-id="4d62e-113">1 </span><span class="sxs-lookup"><span data-stu-id="4d62e-113">1</span></span>|<span data-ttu-id="4d62e-114">Операция не запущена.</span><span class="sxs-lookup"><span data-stu-id="4d62e-114">The operation has not started.</span></span>|
|<span data-ttu-id="4d62e-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="4d62e-115">inProgress</span></span>|<span data-ttu-id="4d62e-116">2 </span><span class="sxs-lookup"><span data-stu-id="4d62e-116">2</span></span>|<span data-ttu-id="4d62e-117">Выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="4d62e-117">The operation is running.</span></span>|
|<span data-ttu-id="4d62e-118">закончил</span><span class="sxs-lookup"><span data-stu-id="4d62e-118">succeeded</span></span>|<span data-ttu-id="4d62e-119">3 </span><span class="sxs-lookup"><span data-stu-id="4d62e-119">3</span></span>|<span data-ttu-id="4d62e-120">Операция выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="4d62e-120">The operation succeeded.</span></span>|
|<span data-ttu-id="4d62e-121">сбоев</span><span class="sxs-lookup"><span data-stu-id="4d62e-121">failed</span></span>|<span data-ttu-id="4d62e-122">4 </span><span class="sxs-lookup"><span data-stu-id="4d62e-122">4</span></span>|<span data-ttu-id="4d62e-123">Сбой операции.</span><span class="sxs-lookup"><span data-stu-id="4d62e-123">The operation failed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
