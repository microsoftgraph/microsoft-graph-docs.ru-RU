---
title: Тип перечисления teamsAsyncOperationStatus
description: Описывает текущее состояние teamsAsyncOperation.
ms.openlocfilehash: f553242ace983651b8d4fda77370de712f9d08b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075765"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="f5044-103">Тип перечисления teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="f5044-103">teamsAsyncOperationStatus enum type</span></span>

> <span data-ttu-id="f5044-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f5044-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5044-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5044-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5044-106">Описывает текущее состояние [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="f5044-106">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="f5044-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f5044-107">Members</span></span>

| <span data-ttu-id="f5044-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f5044-108">Member</span></span> | <span data-ttu-id="f5044-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f5044-109">Value</span></span>| <span data-ttu-id="f5044-110">Description</span><span class="sxs-lookup"><span data-stu-id="f5044-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f5044-111">Недопустимый</span><span class="sxs-lookup"><span data-stu-id="f5044-111">invalid</span></span>|<span data-ttu-id="f5044-112">0</span><span class="sxs-lookup"><span data-stu-id="f5044-112">0</span></span>|<span data-ttu-id="f5044-113">Недопустимое значение.</span><span class="sxs-lookup"><span data-stu-id="f5044-113">Invalid value.</span></span>|
|<span data-ttu-id="f5044-114">notStarted</span><span class="sxs-lookup"><span data-stu-id="f5044-114">notStarted</span></span>|<span data-ttu-id="f5044-115">1</span><span class="sxs-lookup"><span data-stu-id="f5044-115">1</span></span>|<span data-ttu-id="f5044-116">Эта операция не запущена.</span><span class="sxs-lookup"><span data-stu-id="f5044-116">The operation has not started.</span></span>|
|<span data-ttu-id="f5044-117">inProgress</span><span class="sxs-lookup"><span data-stu-id="f5044-117">inProgress</span></span>|<span data-ttu-id="f5044-118">2</span><span class="sxs-lookup"><span data-stu-id="f5044-118">2</span></span>|<span data-ttu-id="f5044-119">Выполнение операции.</span><span class="sxs-lookup"><span data-stu-id="f5044-119">The operation is running.</span></span>|
|<span data-ttu-id="f5044-120">succeeded</span><span class="sxs-lookup"><span data-stu-id="f5044-120">succeeded</span></span>|<span data-ttu-id="f5044-121">3</span><span class="sxs-lookup"><span data-stu-id="f5044-121">3</span></span>|<span data-ttu-id="f5044-122">Операция успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="f5044-122">The operation succeeded.</span></span>|
|<span data-ttu-id="f5044-123">failed</span><span class="sxs-lookup"><span data-stu-id="f5044-123">failed</span></span>|<span data-ttu-id="f5044-124">4</span><span class="sxs-lookup"><span data-stu-id="f5044-124">4</span></span>|<span data-ttu-id="f5044-125">Сбой операции.</span><span class="sxs-lookup"><span data-stu-id="f5044-125">The operation failed.</span></span>|