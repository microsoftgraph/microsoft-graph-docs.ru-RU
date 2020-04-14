---
title: тип перечисления Виндовсаутопилотпрофилеассигнментстатус
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bb330cfd32c4c32b3f4da26755a5060447d21316
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43358567"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="38224-103">тип перечисления Виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="38224-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

<span data-ttu-id="38224-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38224-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38224-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38224-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38224-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38224-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38224-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="38224-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="38224-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="38224-108">Members</span></span>
|<span data-ttu-id="38224-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="38224-109">Member</span></span>|<span data-ttu-id="38224-110">Значение</span><span class="sxs-lookup"><span data-stu-id="38224-110">Value</span></span>|<span data-ttu-id="38224-111">Описание</span><span class="sxs-lookup"><span data-stu-id="38224-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38224-112">unknown</span><span class="sxs-lookup"><span data-stu-id="38224-112">unknown</span></span>|<span data-ttu-id="38224-113">нуль</span><span class="sxs-lookup"><span data-stu-id="38224-113">0</span></span>|<span data-ttu-id="38224-114">Состояние неизвестного назначения</span><span class="sxs-lookup"><span data-stu-id="38224-114">Unknown assignment status</span></span>|
|<span data-ttu-id="38224-115">ассигнединсинк</span><span class="sxs-lookup"><span data-stu-id="38224-115">assignedInSync</span></span>|<span data-ttu-id="38224-116">1,1</span><span class="sxs-lookup"><span data-stu-id="38224-116">1</span></span>|<span data-ttu-id="38224-117">Успешное назначение в Intune и синхронизация с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="38224-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="38224-118">ассигнедаутофсинк</span><span class="sxs-lookup"><span data-stu-id="38224-118">assignedOutOfSync</span></span>|<span data-ttu-id="38224-119">2</span><span class="sxs-lookup"><span data-stu-id="38224-119">2</span></span>|<span data-ttu-id="38224-120">Успешно назначено в Intune и не синхронизировано с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="38224-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="38224-121">ассигнедунковнсинкстате</span><span class="sxs-lookup"><span data-stu-id="38224-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="38224-122">4</span><span class="sxs-lookup"><span data-stu-id="38224-122">3</span></span>|<span data-ttu-id="38224-123">Успешное назначение в Intune и синхронизация с помощью автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="38224-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="38224-124">нотассигнед</span><span class="sxs-lookup"><span data-stu-id="38224-124">notAssigned</span></span>|<span data-ttu-id="38224-125">4 </span><span class="sxs-lookup"><span data-stu-id="38224-125">4</span></span>|<span data-ttu-id="38224-126">Не назначено</span><span class="sxs-lookup"><span data-stu-id="38224-126">Not assigned</span></span>|
|<span data-ttu-id="38224-127">закончен</span><span class="sxs-lookup"><span data-stu-id="38224-127">pending</span></span>|<span data-ttu-id="38224-128">5 </span><span class="sxs-lookup"><span data-stu-id="38224-128">5</span></span>|<span data-ttu-id="38224-129">Ожидание назначения</span><span class="sxs-lookup"><span data-stu-id="38224-129">Pending assignment</span></span>|
|<span data-ttu-id="38224-130">сбоев</span><span class="sxs-lookup"><span data-stu-id="38224-130">failed</span></span>|<span data-ttu-id="38224-131">6 </span><span class="sxs-lookup"><span data-stu-id="38224-131">6</span></span>| <span data-ttu-id="38224-132">Сбой назначения</span><span class="sxs-lookup"><span data-stu-id="38224-132">Assignment failed</span></span>|



