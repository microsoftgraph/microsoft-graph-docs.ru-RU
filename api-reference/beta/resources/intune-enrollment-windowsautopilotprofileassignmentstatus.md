---
title: тип перечисления Виндовсаутопилотпрофилеассигнментстатус
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d241d93924de254af3cb76adfab27b49291b97f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941396"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="8f2b0-103">тип перечисления Виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="8f2b0-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="8f2b0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f2b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f2b0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f2b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f2b0-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8f2b0-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="8f2b0-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8f2b0-107">Members</span></span>
|<span data-ttu-id="8f2b0-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8f2b0-108">Member</span></span>|<span data-ttu-id="8f2b0-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8f2b0-109">Value</span></span>|<span data-ttu-id="8f2b0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8f2b0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f2b0-111">unknown</span><span class="sxs-lookup"><span data-stu-id="8f2b0-111">unknown</span></span>|<span data-ttu-id="8f2b0-112">нуль</span><span class="sxs-lookup"><span data-stu-id="8f2b0-112">0</span></span>|<span data-ttu-id="8f2b0-113">Состояние неизвестного назначения</span><span class="sxs-lookup"><span data-stu-id="8f2b0-113">Unknown assignment status</span></span>|
|<span data-ttu-id="8f2b0-114">Ассигнединсинк</span><span class="sxs-lookup"><span data-stu-id="8f2b0-114">assignedInSync</span></span>|<span data-ttu-id="8f2b0-115">1,1</span><span class="sxs-lookup"><span data-stu-id="8f2b0-115">1</span></span>|<span data-ttu-id="8f2b0-116">Успешное назначение в Intune и синхронизация с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="8f2b0-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="8f2b0-117">Ассигнедаутофсинк</span><span class="sxs-lookup"><span data-stu-id="8f2b0-117">assignedOutOfSync</span></span>|<span data-ttu-id="8f2b0-118">2</span><span class="sxs-lookup"><span data-stu-id="8f2b0-118">2</span></span>|<span data-ttu-id="8f2b0-119">Успешно назначено в Intune и не синхронизировано с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="8f2b0-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="8f2b0-120">Ассигнедунковнсинкстате</span><span class="sxs-lookup"><span data-stu-id="8f2b0-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="8f2b0-121">4</span><span class="sxs-lookup"><span data-stu-id="8f2b0-121">3</span></span>|<span data-ttu-id="8f2b0-122">Успешное назначение в Intune и синхронизация с помощью автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="8f2b0-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="8f2b0-123">Нотассигнед</span><span class="sxs-lookup"><span data-stu-id="8f2b0-123">notAssigned</span></span>|<span data-ttu-id="8f2b0-124">SP4</span><span class="sxs-lookup"><span data-stu-id="8f2b0-124">4</span></span>|<span data-ttu-id="8f2b0-125">Не назначено</span><span class="sxs-lookup"><span data-stu-id="8f2b0-125">Not assigned</span></span>|
|<span data-ttu-id="8f2b0-126">закончен</span><span class="sxs-lookup"><span data-stu-id="8f2b0-126">pending</span></span>|<span data-ttu-id="8f2b0-127">17:00</span><span class="sxs-lookup"><span data-stu-id="8f2b0-127">5</span></span>|<span data-ttu-id="8f2b0-128">Ожидание назначения</span><span class="sxs-lookup"><span data-stu-id="8f2b0-128">Pending assignment</span></span>|
|<span data-ttu-id="8f2b0-129">сбоев</span><span class="sxs-lookup"><span data-stu-id="8f2b0-129">failed</span></span>|<span data-ttu-id="8f2b0-130">6 </span><span class="sxs-lookup"><span data-stu-id="8f2b0-130">6</span></span>| <span data-ttu-id="8f2b0-131">Сбой назначения</span><span class="sxs-lookup"><span data-stu-id="8f2b0-131">Assignment failed</span></span>|




