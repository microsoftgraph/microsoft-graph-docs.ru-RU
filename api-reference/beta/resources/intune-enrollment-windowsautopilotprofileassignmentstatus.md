---
title: тип перечисления Виндовсаутопилотпрофилеассигнментстатус
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d7f946f113288ac95c87053a06ffd737de3dddc4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999000"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="5d570-103">тип перечисления Виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="5d570-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="5d570-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d570-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d570-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d570-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d570-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5d570-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="5d570-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5d570-107">Members</span></span>
|<span data-ttu-id="5d570-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5d570-108">Member</span></span>|<span data-ttu-id="5d570-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5d570-109">Value</span></span>|<span data-ttu-id="5d570-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5d570-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d570-111">unknown</span><span class="sxs-lookup"><span data-stu-id="5d570-111">unknown</span></span>|<span data-ttu-id="5d570-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5d570-112">0</span></span>|<span data-ttu-id="5d570-113">Состояние неизвестного назначения</span><span class="sxs-lookup"><span data-stu-id="5d570-113">Unknown assignment status</span></span>|
|<span data-ttu-id="5d570-114">Ассигнединсинк</span><span class="sxs-lookup"><span data-stu-id="5d570-114">assignedInSync</span></span>|<span data-ttu-id="5d570-115">1,1</span><span class="sxs-lookup"><span data-stu-id="5d570-115">1</span></span>|<span data-ttu-id="5d570-116">Успешное назначение в Intune и синхронизация с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="5d570-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="5d570-117">Ассигнедаутофсинк</span><span class="sxs-lookup"><span data-stu-id="5d570-117">assignedOutOfSync</span></span>|<span data-ttu-id="5d570-118">2</span><span class="sxs-lookup"><span data-stu-id="5d570-118">2</span></span>|<span data-ttu-id="5d570-119">Успешно назначено в Intune и не синхронизировано с программой автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="5d570-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="5d570-120">Ассигнедунковнсинкстате</span><span class="sxs-lookup"><span data-stu-id="5d570-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="5d570-121">4</span><span class="sxs-lookup"><span data-stu-id="5d570-121">3</span></span>|<span data-ttu-id="5d570-122">Успешное назначение в Intune и синхронизация с помощью автоматической пилотной программы Windows</span><span class="sxs-lookup"><span data-stu-id="5d570-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="5d570-123">Нотассигнед</span><span class="sxs-lookup"><span data-stu-id="5d570-123">notAssigned</span></span>|<span data-ttu-id="5d570-124">SP4</span><span class="sxs-lookup"><span data-stu-id="5d570-124">4</span></span>|<span data-ttu-id="5d570-125">Не назначено</span><span class="sxs-lookup"><span data-stu-id="5d570-125">Not assigned</span></span>|
|<span data-ttu-id="5d570-126">закончен</span><span class="sxs-lookup"><span data-stu-id="5d570-126">pending</span></span>|<span data-ttu-id="5d570-127">17:00</span><span class="sxs-lookup"><span data-stu-id="5d570-127">5</span></span>|<span data-ttu-id="5d570-128">Ожидание назначения</span><span class="sxs-lookup"><span data-stu-id="5d570-128">Pending assignment</span></span>|
|<span data-ttu-id="5d570-129">сбоев</span><span class="sxs-lookup"><span data-stu-id="5d570-129">failed</span></span>|<span data-ttu-id="5d570-130">6 </span><span class="sxs-lookup"><span data-stu-id="5d570-130">6</span></span>| <span data-ttu-id="5d570-131">Сбой назначения</span><span class="sxs-lookup"><span data-stu-id="5d570-131">Assignment failed</span></span>|





