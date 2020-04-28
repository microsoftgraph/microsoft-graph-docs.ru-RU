---
title: тип перечисления Теамсасинкоператионстатус
description: Описывает текущее состояние Теамсасинкоператион.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2c82065c789847d3e2a11947dcf921b12c55530e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519899"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="9f452-103">тип перечисления Теамсасинкоператионстатус</span><span class="sxs-lookup"><span data-stu-id="9f452-103">teamsAsyncOperationStatus enum type</span></span>

<span data-ttu-id="9f452-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f452-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f452-105">Описывает текущее состояние [теамсасинкоператион](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9f452-105">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="9f452-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="9f452-106">Members</span></span>

| <span data-ttu-id="9f452-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="9f452-107">Member</span></span> | <span data-ttu-id="9f452-108">Значение</span><span class="sxs-lookup"><span data-stu-id="9f452-108">Value</span></span>| <span data-ttu-id="9f452-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9f452-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9f452-110">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="9f452-110">invalid</span></span>|<span data-ttu-id="9f452-111">нуль</span><span class="sxs-lookup"><span data-stu-id="9f452-111">0</span></span>|<span data-ttu-id="9f452-112">Недопустимое значение.</span><span class="sxs-lookup"><span data-stu-id="9f452-112">Invalid value.</span></span>|
|<span data-ttu-id="9f452-113">notStarted</span><span class="sxs-lookup"><span data-stu-id="9f452-113">notStarted</span></span>|<span data-ttu-id="9f452-114">1,1</span><span class="sxs-lookup"><span data-stu-id="9f452-114">1</span></span>|<span data-ttu-id="9f452-115">Операция не запущена.</span><span class="sxs-lookup"><span data-stu-id="9f452-115">The operation has not started.</span></span>|
|<span data-ttu-id="9f452-116">inProgress</span><span class="sxs-lookup"><span data-stu-id="9f452-116">inProgress</span></span>|<span data-ttu-id="9f452-117">2</span><span class="sxs-lookup"><span data-stu-id="9f452-117">2</span></span>|<span data-ttu-id="9f452-118">Выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="9f452-118">The operation is running.</span></span>|
|<span data-ttu-id="9f452-119">закончил</span><span class="sxs-lookup"><span data-stu-id="9f452-119">succeeded</span></span>|<span data-ttu-id="9f452-120">4</span><span class="sxs-lookup"><span data-stu-id="9f452-120">3</span></span>|<span data-ttu-id="9f452-121">Операция выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="9f452-121">The operation succeeded.</span></span>|
|<span data-ttu-id="9f452-122">сбоев</span><span class="sxs-lookup"><span data-stu-id="9f452-122">failed</span></span>|<span data-ttu-id="9f452-123">4 </span><span class="sxs-lookup"><span data-stu-id="9f452-123">4</span></span>|<span data-ttu-id="9f452-124">Сбой операции.</span><span class="sxs-lookup"><span data-stu-id="9f452-124">The operation failed.</span></span>|
