---
title: тип перечисления Виндовсаутопилотпрофилеассигнментстатус
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7100e5881049900bb474e20060ac916ec1199a29
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783370"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="8b44e-103">тип перечисления Виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="8b44e-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="8b44e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b44e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b44e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b44e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b44e-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8b44e-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="8b44e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8b44e-107">Members</span></span>
|<span data-ttu-id="8b44e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8b44e-108">Member</span></span>|<span data-ttu-id="8b44e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8b44e-109">Value</span></span>|<span data-ttu-id="8b44e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8b44e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b44e-111">unknown</span><span class="sxs-lookup"><span data-stu-id="8b44e-111">unknown</span></span>|<span data-ttu-id="8b44e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="8b44e-112">0</span></span>|<span data-ttu-id="8b44e-113">Состояние неизвестного назначения</span><span class="sxs-lookup"><span data-stu-id="8b44e-113">Unknown assignment status</span></span>|
|<span data-ttu-id="8b44e-114">ассигнединсинк</span><span class="sxs-lookup"><span data-stu-id="8b44e-114">assignedInSync</span></span>|<span data-ttu-id="8b44e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="8b44e-115">1</span></span>|<span data-ttu-id="8b44e-116">Успешное назначение в Intune и синхронизация с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="8b44e-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="8b44e-117">ассигнедаутофсинк</span><span class="sxs-lookup"><span data-stu-id="8b44e-117">assignedOutOfSync</span></span>|<span data-ttu-id="8b44e-118">2</span><span class="sxs-lookup"><span data-stu-id="8b44e-118">2</span></span>|<span data-ttu-id="8b44e-119">Успешно назначено в Intune и не синхронизировано с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="8b44e-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="8b44e-120">ассигнедунковнсинкстате</span><span class="sxs-lookup"><span data-stu-id="8b44e-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="8b44e-121">4</span><span class="sxs-lookup"><span data-stu-id="8b44e-121">3</span></span>|<span data-ttu-id="8b44e-122">Успешное назначение в Intune и синхронизация с помощью автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="8b44e-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="8b44e-123">нотассигнед</span><span class="sxs-lookup"><span data-stu-id="8b44e-123">notAssigned</span></span>|<span data-ttu-id="8b44e-124">4 </span><span class="sxs-lookup"><span data-stu-id="8b44e-124">4</span></span>|<span data-ttu-id="8b44e-125">Не назначено</span><span class="sxs-lookup"><span data-stu-id="8b44e-125">Not assigned</span></span>|
|<span data-ttu-id="8b44e-126">закончен</span><span class="sxs-lookup"><span data-stu-id="8b44e-126">pending</span></span>|<span data-ttu-id="8b44e-127">5 </span><span class="sxs-lookup"><span data-stu-id="8b44e-127">5</span></span>|<span data-ttu-id="8b44e-128">Ожидание назначения</span><span class="sxs-lookup"><span data-stu-id="8b44e-128">Pending assignment</span></span>|
|<span data-ttu-id="8b44e-129">сбоев</span><span class="sxs-lookup"><span data-stu-id="8b44e-129">failed</span></span>|<span data-ttu-id="8b44e-130">6 </span><span class="sxs-lookup"><span data-stu-id="8b44e-130">6</span></span>| <span data-ttu-id="8b44e-131">Сбой назначения</span><span class="sxs-lookup"><span data-stu-id="8b44e-131">Assignment failed</span></span>|



