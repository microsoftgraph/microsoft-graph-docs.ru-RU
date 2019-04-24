---
title: тип перечисления Теамсасинкоператионстатус
description: Описывает текущее состояние Теамсасинкоператион.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b3ceaca73fe013b76f44cdf9290f3c0935e93b0a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462230"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="2b4fa-103">тип перечисления Теамсасинкоператионстатус</span><span class="sxs-lookup"><span data-stu-id="2b4fa-103">teamsAsyncOperationStatus enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b4fa-104">Описывает текущее состояние [теамсасинкоператион](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="2b4fa-104">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="2b4fa-105">Элементы</span><span class="sxs-lookup"><span data-stu-id="2b4fa-105">Members</span></span>

| <span data-ttu-id="2b4fa-106">Элемент</span><span class="sxs-lookup"><span data-stu-id="2b4fa-106">Member</span></span> | <span data-ttu-id="2b4fa-107">Значение</span><span class="sxs-lookup"><span data-stu-id="2b4fa-107">Value</span></span>| <span data-ttu-id="2b4fa-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2b4fa-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2b4fa-109">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="2b4fa-109">invalid</span></span>|<span data-ttu-id="2b4fa-110">нуль</span><span class="sxs-lookup"><span data-stu-id="2b4fa-110">0</span></span>|<span data-ttu-id="2b4fa-111">Недопустимое значение.</span><span class="sxs-lookup"><span data-stu-id="2b4fa-111">Invalid value.</span></span>|
|<span data-ttu-id="2b4fa-112">notStarted</span><span class="sxs-lookup"><span data-stu-id="2b4fa-112">notStarted</span></span>|<span data-ttu-id="2b4fa-113">1,1</span><span class="sxs-lookup"><span data-stu-id="2b4fa-113">1</span></span>|<span data-ttu-id="2b4fa-114">Операция не запущена.</span><span class="sxs-lookup"><span data-stu-id="2b4fa-114">The operation has not started.</span></span>|
|<span data-ttu-id="2b4fa-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="2b4fa-115">inProgress</span></span>|<span data-ttu-id="2b4fa-116">2</span><span class="sxs-lookup"><span data-stu-id="2b4fa-116">2</span></span>|<span data-ttu-id="2b4fa-117">Выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="2b4fa-117">The operation is running.</span></span>|
|<span data-ttu-id="2b4fa-118">закончил</span><span class="sxs-lookup"><span data-stu-id="2b4fa-118">succeeded</span></span>|<span data-ttu-id="2b4fa-119">4</span><span class="sxs-lookup"><span data-stu-id="2b4fa-119">3</span></span>|<span data-ttu-id="2b4fa-120">Операция выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="2b4fa-120">The operation succeeded.</span></span>|
|<span data-ttu-id="2b4fa-121">сбоев</span><span class="sxs-lookup"><span data-stu-id="2b4fa-121">failed</span></span>|<span data-ttu-id="2b4fa-122">SP4</span><span class="sxs-lookup"><span data-stu-id="2b4fa-122">4</span></span>|<span data-ttu-id="2b4fa-123">Сбой операции.</span><span class="sxs-lookup"><span data-stu-id="2b4fa-123">The operation failed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
