---
title: Тип перечисления teamsAsyncOperationStatus
description: Описывает текущее состояние teamsAsyncOperation.
author: nkramer
ms.openlocfilehash: 49b5b81999714627b1a1acd42df208594123b262
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332006"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="d8a8d-103">Тип перечисления teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="d8a8d-103">teamsAsyncOperationStatus enum type</span></span>

> <span data-ttu-id="d8a8d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d8a8d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8a8d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a8d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8a8d-106">Описывает текущее состояние [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="d8a8d-106">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="d8a8d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="d8a8d-107">Members</span></span>

| <span data-ttu-id="d8a8d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="d8a8d-108">Member</span></span> | <span data-ttu-id="d8a8d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d8a8d-109">Value</span></span>| <span data-ttu-id="d8a8d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d8a8d-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d8a8d-111">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="d8a8d-111">invalid</span></span>|<span data-ttu-id="d8a8d-112">0</span><span class="sxs-lookup"><span data-stu-id="d8a8d-112">0</span></span>|<span data-ttu-id="d8a8d-113">Недопустимое значение.</span><span class="sxs-lookup"><span data-stu-id="d8a8d-113">Invalid value.</span></span>|
|<span data-ttu-id="d8a8d-114">notStarted</span><span class="sxs-lookup"><span data-stu-id="d8a8d-114">notStarted</span></span>|<span data-ttu-id="d8a8d-115">1</span><span class="sxs-lookup"><span data-stu-id="d8a8d-115">1</span></span>|<span data-ttu-id="d8a8d-116">Эта операция не запущена.</span><span class="sxs-lookup"><span data-stu-id="d8a8d-116">The operation has not started.</span></span>|
|<span data-ttu-id="d8a8d-117">inProgress</span><span class="sxs-lookup"><span data-stu-id="d8a8d-117">inProgress</span></span>|<span data-ttu-id="d8a8d-118">2</span><span class="sxs-lookup"><span data-stu-id="d8a8d-118">2</span></span>|<span data-ttu-id="d8a8d-119">Выполнение операции.</span><span class="sxs-lookup"><span data-stu-id="d8a8d-119">The operation is running.</span></span>|
|<span data-ttu-id="d8a8d-120">succeeded</span><span class="sxs-lookup"><span data-stu-id="d8a8d-120">succeeded</span></span>|<span data-ttu-id="d8a8d-121">3</span><span class="sxs-lookup"><span data-stu-id="d8a8d-121">3</span></span>|<span data-ttu-id="d8a8d-122">Операция успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="d8a8d-122">The operation succeeded.</span></span>|
|<span data-ttu-id="d8a8d-123">failed</span><span class="sxs-lookup"><span data-stu-id="d8a8d-123">failed</span></span>|<span data-ttu-id="d8a8d-124">4</span><span class="sxs-lookup"><span data-stu-id="d8a8d-124">4</span></span>|<span data-ttu-id="d8a8d-125">Сбой операции.</span><span class="sxs-lookup"><span data-stu-id="d8a8d-125">The operation failed.</span></span>|