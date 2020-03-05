---
title: тип перечисления Емаилсинксчедуле
description: Возможные значения для расписания синхронизации электронной почты.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c77a56b5dea371b4d91deb2258dad265b4d0433c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526467"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="e93d9-103">тип перечисления Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="e93d9-103">emailSyncSchedule enum type</span></span>

<span data-ttu-id="e93d9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e93d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e93d9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e93d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e93d9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e93d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e93d9-107">Возможные значения для расписания синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e93d9-107">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="e93d9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e93d9-108">Members</span></span>
|<span data-ttu-id="e93d9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e93d9-109">Member</span></span>|<span data-ttu-id="e93d9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e93d9-110">Value</span></span>|<span data-ttu-id="e93d9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e93d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e93d9-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="e93d9-112">userDefined</span></span>|<span data-ttu-id="e93d9-113">нуль</span><span class="sxs-lookup"><span data-stu-id="e93d9-113">0</span></span>|<span data-ttu-id="e93d9-114">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="e93d9-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e93d9-115">асмессажесарриве</span><span class="sxs-lookup"><span data-stu-id="e93d9-115">asMessagesArrive</span></span>|<span data-ttu-id="e93d9-116">1 </span><span class="sxs-lookup"><span data-stu-id="e93d9-116">1</span></span>|<span data-ttu-id="e93d9-117">Синхронизация по мере поступления сообщений.</span><span class="sxs-lookup"><span data-stu-id="e93d9-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="e93d9-118">Вручную</span><span class="sxs-lookup"><span data-stu-id="e93d9-118">manual</span></span>|<span data-ttu-id="e93d9-119">2 </span><span class="sxs-lookup"><span data-stu-id="e93d9-119">2</span></span>|<span data-ttu-id="e93d9-120">Синхронизация вручную.</span><span class="sxs-lookup"><span data-stu-id="e93d9-120">Sync manually.</span></span>|
|<span data-ttu-id="e93d9-121">фифтинминутес</span><span class="sxs-lookup"><span data-stu-id="e93d9-121">fifteenMinutes</span></span>|<span data-ttu-id="e93d9-122">3 </span><span class="sxs-lookup"><span data-stu-id="e93d9-122">3</span></span>|<span data-ttu-id="e93d9-123">Синхронизация каждые пятнадцать минут.</span><span class="sxs-lookup"><span data-stu-id="e93d9-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="e93d9-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="e93d9-124">thirtyMinutes</span></span>|<span data-ttu-id="e93d9-125">4 </span><span class="sxs-lookup"><span data-stu-id="e93d9-125">4</span></span>|<span data-ttu-id="e93d9-126">Синхронизация каждые 30 минут.</span><span class="sxs-lookup"><span data-stu-id="e93d9-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="e93d9-127">сикстиминутес</span><span class="sxs-lookup"><span data-stu-id="e93d9-127">sixtyMinutes</span></span>|<span data-ttu-id="e93d9-128">5 </span><span class="sxs-lookup"><span data-stu-id="e93d9-128">5</span></span>|<span data-ttu-id="e93d9-129">Синхронизация каждые 60 минут.</span><span class="sxs-lookup"><span data-stu-id="e93d9-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="e93d9-130">баседонмюсаже</span><span class="sxs-lookup"><span data-stu-id="e93d9-130">basedOnMyUsage</span></span>|<span data-ttu-id="e93d9-131">6 </span><span class="sxs-lookup"><span data-stu-id="e93d9-131">6</span></span>|<span data-ttu-id="e93d9-132">Синхронизация с учетом использования.</span><span class="sxs-lookup"><span data-stu-id="e93d9-132">Sync based on my usage.</span></span>|



