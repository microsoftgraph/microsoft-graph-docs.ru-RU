---
title: тип перечисления Виндовсаутопилотпрофилеассигнментстатус
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3be930f3289891235a1462d0322323eb9b44bf60
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989751"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="75ba4-103">тип перечисления Виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="75ba4-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="75ba4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75ba4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75ba4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75ba4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75ba4-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="75ba4-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="75ba4-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="75ba4-107">Members</span></span>
|<span data-ttu-id="75ba4-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="75ba4-108">Member</span></span>|<span data-ttu-id="75ba4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="75ba4-109">Value</span></span>|<span data-ttu-id="75ba4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="75ba4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75ba4-111">unknown</span><span class="sxs-lookup"><span data-stu-id="75ba4-111">unknown</span></span>|<span data-ttu-id="75ba4-112">нуль</span><span class="sxs-lookup"><span data-stu-id="75ba4-112">0</span></span>|<span data-ttu-id="75ba4-113">Состояние неизвестного назначения</span><span class="sxs-lookup"><span data-stu-id="75ba4-113">Unknown assignment status</span></span>|
|<span data-ttu-id="75ba4-114">Ассигнединсинк</span><span class="sxs-lookup"><span data-stu-id="75ba4-114">assignedInSync</span></span>|<span data-ttu-id="75ba4-115">1,1</span><span class="sxs-lookup"><span data-stu-id="75ba4-115">1</span></span>|<span data-ttu-id="75ba4-116">Успешное назначение в Intune и синхронизация с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="75ba4-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="75ba4-117">Ассигнедаутофсинк</span><span class="sxs-lookup"><span data-stu-id="75ba4-117">assignedOutOfSync</span></span>|<span data-ttu-id="75ba4-118">2</span><span class="sxs-lookup"><span data-stu-id="75ba4-118">2</span></span>|<span data-ttu-id="75ba4-119">Успешно назначено в Intune и не синхронизировано с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="75ba4-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="75ba4-120">Ассигнедунковнсинкстате</span><span class="sxs-lookup"><span data-stu-id="75ba4-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="75ba4-121">4</span><span class="sxs-lookup"><span data-stu-id="75ba4-121">3</span></span>|<span data-ttu-id="75ba4-122">Успешное назначение в Intune и синхронизация с помощью автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="75ba4-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="75ba4-123">Нотассигнед</span><span class="sxs-lookup"><span data-stu-id="75ba4-123">notAssigned</span></span>|<span data-ttu-id="75ba4-124">SP4</span><span class="sxs-lookup"><span data-stu-id="75ba4-124">4</span></span>|<span data-ttu-id="75ba4-125">Не назначено</span><span class="sxs-lookup"><span data-stu-id="75ba4-125">Not assigned</span></span>|
|<span data-ttu-id="75ba4-126">закончен</span><span class="sxs-lookup"><span data-stu-id="75ba4-126">pending</span></span>|<span data-ttu-id="75ba4-127">17:00</span><span class="sxs-lookup"><span data-stu-id="75ba4-127">5</span></span>|<span data-ttu-id="75ba4-128">Ожидание назначения</span><span class="sxs-lookup"><span data-stu-id="75ba4-128">Pending assignment</span></span>|
|<span data-ttu-id="75ba4-129">сбоев</span><span class="sxs-lookup"><span data-stu-id="75ba4-129">failed</span></span>|<span data-ttu-id="75ba4-130">6 </span><span class="sxs-lookup"><span data-stu-id="75ba4-130">6</span></span>| <span data-ttu-id="75ba4-131">Сбой назначения</span><span class="sxs-lookup"><span data-stu-id="75ba4-131">Assignment failed</span></span>|





