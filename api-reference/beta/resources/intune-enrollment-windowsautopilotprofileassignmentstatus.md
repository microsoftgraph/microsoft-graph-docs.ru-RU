---
title: Тип перечисления windowsAutopilotProfileAssignmentStatus
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1427ffeb45862312d92fdf02a00a242725894d36
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962634"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="5caae-103">Тип перечисления windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="5caae-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="5caae-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5caae-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5caae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5caae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5caae-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5caae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5caae-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5caae-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="5caae-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="5caae-108">Members</span></span>
|<span data-ttu-id="5caae-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="5caae-109">Member</span></span>|<span data-ttu-id="5caae-110">Значение</span><span class="sxs-lookup"><span data-stu-id="5caae-110">Value</span></span>|<span data-ttu-id="5caae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5caae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5caae-112">unknown</span><span class="sxs-lookup"><span data-stu-id="5caae-112">unknown</span></span>|<span data-ttu-id="5caae-113">0</span><span class="sxs-lookup"><span data-stu-id="5caae-113">0</span></span>|<span data-ttu-id="5caae-114">Состояние Unknown назначения</span><span class="sxs-lookup"><span data-stu-id="5caae-114">Unknown assignment status</span></span>|
|<span data-ttu-id="5caae-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="5caae-115">assignedInSync</span></span>|<span data-ttu-id="5caae-116">1</span><span class="sxs-lookup"><span data-stu-id="5caae-116">1</span></span>|<span data-ttu-id="5caae-117">Назначенный успешно в Intune и синхронизации с Windows автоматически Пилотная программа</span><span class="sxs-lookup"><span data-stu-id="5caae-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="5caae-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="5caae-118">assignedOutOfSync</span></span>|<span data-ttu-id="5caae-119">2</span><span class="sxs-lookup"><span data-stu-id="5caae-119">2</span></span>|<span data-ttu-id="5caae-120">Назначенный успешно в Intune и не синхронизированы с Пилотная программа автоматически Windows</span><span class="sxs-lookup"><span data-stu-id="5caae-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="5caae-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="5caae-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="5caae-122">3</span><span class="sxs-lookup"><span data-stu-id="5caae-122">3</span></span>|<span data-ttu-id="5caae-123">Назначенный успешно в Intune и либо в синхронизации или синхронизированы с Пилотная программа автоматически Windows</span><span class="sxs-lookup"><span data-stu-id="5caae-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="5caae-124">не назначено</span><span class="sxs-lookup"><span data-stu-id="5caae-124">notAssigned</span></span>|<span data-ttu-id="5caae-125">4</span><span class="sxs-lookup"><span data-stu-id="5caae-125">4</span></span>|<span data-ttu-id="5caae-126">Не назначен</span><span class="sxs-lookup"><span data-stu-id="5caae-126">Not assigned</span></span>|
|<span data-ttu-id="5caae-127">Ожидание</span><span class="sxs-lookup"><span data-stu-id="5caae-127">pending</span></span>|<span data-ttu-id="5caae-128">5</span><span class="sxs-lookup"><span data-stu-id="5caae-128">5</span></span>|<span data-ttu-id="5caae-129">Ожидающие назначения</span><span class="sxs-lookup"><span data-stu-id="5caae-129">Pending assignment</span></span>|
|<span data-ttu-id="5caae-130">failed</span><span class="sxs-lookup"><span data-stu-id="5caae-130">failed</span></span>|<span data-ttu-id="5caae-131">6</span><span class="sxs-lookup"><span data-stu-id="5caae-131">6</span></span>| <span data-ttu-id="5caae-132">Не удалось назначения</span><span class="sxs-lookup"><span data-stu-id="5caae-132">Assignment failed</span></span>|





