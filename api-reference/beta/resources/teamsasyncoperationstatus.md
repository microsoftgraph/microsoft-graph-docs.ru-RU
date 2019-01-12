---
title: Тип перечисления teamsAsyncOperationStatus
description: Описывает текущее состояние teamsAsyncOperation.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e136d043cf58480d93888374558a1be06ca9053d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914823"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="a0a43-103">Тип перечисления teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="a0a43-103">teamsAsyncOperationStatus enum type</span></span>

> <span data-ttu-id="a0a43-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a0a43-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0a43-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0a43-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0a43-106">Описывает текущее состояние [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="a0a43-106">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="a0a43-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="a0a43-107">Members</span></span>

| <span data-ttu-id="a0a43-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="a0a43-108">Member</span></span> | <span data-ttu-id="a0a43-109">Значение</span><span class="sxs-lookup"><span data-stu-id="a0a43-109">Value</span></span>| <span data-ttu-id="a0a43-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a0a43-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a0a43-111">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="a0a43-111">invalid</span></span>|<span data-ttu-id="a0a43-112">0</span><span class="sxs-lookup"><span data-stu-id="a0a43-112">0</span></span>|<span data-ttu-id="a0a43-113">Недопустимое значение.</span><span class="sxs-lookup"><span data-stu-id="a0a43-113">Invalid value.</span></span>|
|<span data-ttu-id="a0a43-114">notStarted</span><span class="sxs-lookup"><span data-stu-id="a0a43-114">notStarted</span></span>|<span data-ttu-id="a0a43-115">1</span><span class="sxs-lookup"><span data-stu-id="a0a43-115">1</span></span>|<span data-ttu-id="a0a43-116">Эта операция не запущена.</span><span class="sxs-lookup"><span data-stu-id="a0a43-116">The operation has not started.</span></span>|
|<span data-ttu-id="a0a43-117">inProgress</span><span class="sxs-lookup"><span data-stu-id="a0a43-117">inProgress</span></span>|<span data-ttu-id="a0a43-118">2</span><span class="sxs-lookup"><span data-stu-id="a0a43-118">2</span></span>|<span data-ttu-id="a0a43-119">Выполнение операции.</span><span class="sxs-lookup"><span data-stu-id="a0a43-119">The operation is running.</span></span>|
|<span data-ttu-id="a0a43-120">succeeded</span><span class="sxs-lookup"><span data-stu-id="a0a43-120">succeeded</span></span>|<span data-ttu-id="a0a43-121">3</span><span class="sxs-lookup"><span data-stu-id="a0a43-121">3</span></span>|<span data-ttu-id="a0a43-122">Операция успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="a0a43-122">The operation succeeded.</span></span>|
|<span data-ttu-id="a0a43-123">failed</span><span class="sxs-lookup"><span data-stu-id="a0a43-123">failed</span></span>|<span data-ttu-id="a0a43-124">4</span><span class="sxs-lookup"><span data-stu-id="a0a43-124">4</span></span>|<span data-ttu-id="a0a43-125">Сбой операции.</span><span class="sxs-lookup"><span data-stu-id="a0a43-125">The operation failed.</span></span>|
