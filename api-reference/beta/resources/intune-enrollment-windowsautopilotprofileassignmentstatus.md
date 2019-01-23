---
title: Тип перечисления windowsAutopilotProfileAssignmentStatus
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 68612e2f4ccee46612c82237630efafda484b7e9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419123"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="d223f-103">Тип перечисления windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="d223f-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="d223f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d223f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d223f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d223f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d223f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d223f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d223f-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d223f-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="d223f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d223f-108">Members</span></span>
|<span data-ttu-id="d223f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d223f-109">Member</span></span>|<span data-ttu-id="d223f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d223f-110">Value</span></span>|<span data-ttu-id="d223f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d223f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d223f-112">unknown</span><span class="sxs-lookup"><span data-stu-id="d223f-112">unknown</span></span>|<span data-ttu-id="d223f-113">0</span><span class="sxs-lookup"><span data-stu-id="d223f-113">0</span></span>|<span data-ttu-id="d223f-114">Состояние Unknown назначения</span><span class="sxs-lookup"><span data-stu-id="d223f-114">Unknown assignment status</span></span>|
|<span data-ttu-id="d223f-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="d223f-115">assignedInSync</span></span>|<span data-ttu-id="d223f-116">1</span><span class="sxs-lookup"><span data-stu-id="d223f-116">1</span></span>|<span data-ttu-id="d223f-117">Назначенный успешно в Intune и синхронизации с Windows автоматически Пилотная программа</span><span class="sxs-lookup"><span data-stu-id="d223f-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="d223f-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="d223f-118">assignedOutOfSync</span></span>|<span data-ttu-id="d223f-119">2</span><span class="sxs-lookup"><span data-stu-id="d223f-119">2</span></span>|<span data-ttu-id="d223f-120">Назначенный успешно в Intune и не синхронизированы с Пилотная программа автоматически Windows</span><span class="sxs-lookup"><span data-stu-id="d223f-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="d223f-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="d223f-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="d223f-122">3</span><span class="sxs-lookup"><span data-stu-id="d223f-122">3</span></span>|<span data-ttu-id="d223f-123">Назначенный успешно в Intune и либо в синхронизации или синхронизированы с Пилотная программа автоматически Windows</span><span class="sxs-lookup"><span data-stu-id="d223f-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="d223f-124">не назначено</span><span class="sxs-lookup"><span data-stu-id="d223f-124">notAssigned</span></span>|<span data-ttu-id="d223f-125">4</span><span class="sxs-lookup"><span data-stu-id="d223f-125">4</span></span>|<span data-ttu-id="d223f-126">Не назначен</span><span class="sxs-lookup"><span data-stu-id="d223f-126">Not assigned</span></span>|
|<span data-ttu-id="d223f-127">Ожидание</span><span class="sxs-lookup"><span data-stu-id="d223f-127">pending</span></span>|<span data-ttu-id="d223f-128">5</span><span class="sxs-lookup"><span data-stu-id="d223f-128">5</span></span>|<span data-ttu-id="d223f-129">Ожидающие назначения</span><span class="sxs-lookup"><span data-stu-id="d223f-129">Pending assignment</span></span>|
|<span data-ttu-id="d223f-130">failed</span><span class="sxs-lookup"><span data-stu-id="d223f-130">failed</span></span>|<span data-ttu-id="d223f-131">6</span><span class="sxs-lookup"><span data-stu-id="d223f-131">6</span></span>| <span data-ttu-id="d223f-132">Не удалось назначения</span><span class="sxs-lookup"><span data-stu-id="d223f-132">Assignment failed</span></span>|




