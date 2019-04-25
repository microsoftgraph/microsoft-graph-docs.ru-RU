---
title: тип перечисления Виндовсаутопилотпрофилеассигнментстатус
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f4c6fbfcbefd88af31f2875cf33755b3be21e06
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525280"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="ec114-103">тип перечисления Виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="ec114-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="ec114-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec114-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec114-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec114-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec114-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ec114-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="ec114-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ec114-107">Members</span></span>
|<span data-ttu-id="ec114-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ec114-108">Member</span></span>|<span data-ttu-id="ec114-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ec114-109">Value</span></span>|<span data-ttu-id="ec114-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ec114-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec114-111">unknown</span><span class="sxs-lookup"><span data-stu-id="ec114-111">unknown</span></span>|<span data-ttu-id="ec114-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ec114-112">0</span></span>|<span data-ttu-id="ec114-113">Состояние неИзвестного назначения</span><span class="sxs-lookup"><span data-stu-id="ec114-113">Unknown assignment status</span></span>|
|<span data-ttu-id="ec114-114">Ассигнединсинк</span><span class="sxs-lookup"><span data-stu-id="ec114-114">assignedInSync</span></span>|<span data-ttu-id="ec114-115">1 </span><span class="sxs-lookup"><span data-stu-id="ec114-115">1</span></span>|<span data-ttu-id="ec114-116">Успешное назначение в Intune и синхронизация с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="ec114-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="ec114-117">Ассигнедаутофсинк</span><span class="sxs-lookup"><span data-stu-id="ec114-117">assignedOutOfSync</span></span>|<span data-ttu-id="ec114-118">2 </span><span class="sxs-lookup"><span data-stu-id="ec114-118">2</span></span>|<span data-ttu-id="ec114-119">Успешно назначено в Intune и не синхронизировано с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="ec114-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="ec114-120">Ассигнедунковнсинкстате</span><span class="sxs-lookup"><span data-stu-id="ec114-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="ec114-121">3 </span><span class="sxs-lookup"><span data-stu-id="ec114-121">3</span></span>|<span data-ttu-id="ec114-122">Успешное назначение в Intune и синхронизация с помощью автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="ec114-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="ec114-123">Нотассигнед</span><span class="sxs-lookup"><span data-stu-id="ec114-123">notAssigned</span></span>|<span data-ttu-id="ec114-124">4 </span><span class="sxs-lookup"><span data-stu-id="ec114-124">4</span></span>|<span data-ttu-id="ec114-125">Не назначено</span><span class="sxs-lookup"><span data-stu-id="ec114-125">Not assigned</span></span>|
|<span data-ttu-id="ec114-126">закончен</span><span class="sxs-lookup"><span data-stu-id="ec114-126">pending</span></span>|<span data-ttu-id="ec114-127">5 </span><span class="sxs-lookup"><span data-stu-id="ec114-127">5</span></span>|<span data-ttu-id="ec114-128">Ожидание назначения</span><span class="sxs-lookup"><span data-stu-id="ec114-128">Pending assignment</span></span>|
|<span data-ttu-id="ec114-129">сбоев</span><span class="sxs-lookup"><span data-stu-id="ec114-129">failed</span></span>|<span data-ttu-id="ec114-130">6 </span><span class="sxs-lookup"><span data-stu-id="ec114-130">6</span></span>| <span data-ttu-id="ec114-131">Сбой назначения</span><span class="sxs-lookup"><span data-stu-id="ec114-131">Assignment failed</span></span>|





