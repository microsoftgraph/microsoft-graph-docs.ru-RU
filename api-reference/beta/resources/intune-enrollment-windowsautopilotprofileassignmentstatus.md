---
title: тип перечисления Виндовсаутопилотпрофилеассигнментстатус
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f4c6fbfcbefd88af31f2875cf33755b3be21e06
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773191"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="9b567-103">тип перечисления Виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="9b567-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="9b567-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b567-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b567-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b567-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b567-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9b567-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="9b567-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9b567-107">Members</span></span>
|<span data-ttu-id="9b567-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9b567-108">Member</span></span>|<span data-ttu-id="9b567-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9b567-109">Value</span></span>|<span data-ttu-id="9b567-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9b567-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b567-111">unknown</span><span class="sxs-lookup"><span data-stu-id="9b567-111">unknown</span></span>|<span data-ttu-id="9b567-112">нуль</span><span class="sxs-lookup"><span data-stu-id="9b567-112">0</span></span>|<span data-ttu-id="9b567-113">Состояние неИзвестного назначения</span><span class="sxs-lookup"><span data-stu-id="9b567-113">Unknown assignment status</span></span>|
|<span data-ttu-id="9b567-114">Ассигнединсинк</span><span class="sxs-lookup"><span data-stu-id="9b567-114">assignedInSync</span></span>|<span data-ttu-id="9b567-115">1,1</span><span class="sxs-lookup"><span data-stu-id="9b567-115">1</span></span>|<span data-ttu-id="9b567-116">Успешное назначение в Intune и синхронизация с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="9b567-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="9b567-117">Ассигнедаутофсинк</span><span class="sxs-lookup"><span data-stu-id="9b567-117">assignedOutOfSync</span></span>|<span data-ttu-id="9b567-118">2</span><span class="sxs-lookup"><span data-stu-id="9b567-118">2</span></span>|<span data-ttu-id="9b567-119">Успешно назначено в Intune и не синхронизировано с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="9b567-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="9b567-120">Ассигнедунковнсинкстате</span><span class="sxs-lookup"><span data-stu-id="9b567-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="9b567-121">4</span><span class="sxs-lookup"><span data-stu-id="9b567-121">3</span></span>|<span data-ttu-id="9b567-122">Успешное назначение в Intune и синхронизация с помощью автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="9b567-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="9b567-123">Нотассигнед</span><span class="sxs-lookup"><span data-stu-id="9b567-123">notAssigned</span></span>|<span data-ttu-id="9b567-124">SP4</span><span class="sxs-lookup"><span data-stu-id="9b567-124">4</span></span>|<span data-ttu-id="9b567-125">Не назначено</span><span class="sxs-lookup"><span data-stu-id="9b567-125">Not assigned</span></span>|
|<span data-ttu-id="9b567-126">закончен</span><span class="sxs-lookup"><span data-stu-id="9b567-126">pending</span></span>|<span data-ttu-id="9b567-127">17:00</span><span class="sxs-lookup"><span data-stu-id="9b567-127">5</span></span>|<span data-ttu-id="9b567-128">Ожидание назначения</span><span class="sxs-lookup"><span data-stu-id="9b567-128">Pending assignment</span></span>|
|<span data-ttu-id="9b567-129">сбоев</span><span class="sxs-lookup"><span data-stu-id="9b567-129">failed</span></span>|<span data-ttu-id="9b567-130">ICMPv6</span><span class="sxs-lookup"><span data-stu-id="9b567-130">6</span></span>| <span data-ttu-id="9b567-131">Сбой назначения</span><span class="sxs-lookup"><span data-stu-id="9b567-131">Assignment failed</span></span>|





