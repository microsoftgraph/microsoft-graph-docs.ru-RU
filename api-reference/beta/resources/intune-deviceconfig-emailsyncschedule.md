---
title: тип перечисления Емаилсинксчедуле
description: Возможные значения для расписания синхронизации электронной почты.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 63e0c1ffaed029ca5ba010181c70ab0588135a36
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49198876"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="22d97-103">тип перечисления Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="22d97-103">emailSyncSchedule enum type</span></span>

<span data-ttu-id="22d97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22d97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22d97-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22d97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22d97-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22d97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22d97-107">Возможные значения для расписания синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="22d97-107">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="22d97-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="22d97-108">Members</span></span>
|<span data-ttu-id="22d97-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="22d97-109">Member</span></span>|<span data-ttu-id="22d97-110">Значение</span><span class="sxs-lookup"><span data-stu-id="22d97-110">Value</span></span>|<span data-ttu-id="22d97-111">Описание</span><span class="sxs-lookup"><span data-stu-id="22d97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22d97-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="22d97-112">userDefined</span></span>|<span data-ttu-id="22d97-113">нуль</span><span class="sxs-lookup"><span data-stu-id="22d97-113">0</span></span>|<span data-ttu-id="22d97-114">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="22d97-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="22d97-115">асмессажесарриве</span><span class="sxs-lookup"><span data-stu-id="22d97-115">asMessagesArrive</span></span>|<span data-ttu-id="22d97-116">1,1</span><span class="sxs-lookup"><span data-stu-id="22d97-116">1</span></span>|<span data-ttu-id="22d97-117">Синхронизация по мере поступления сообщений.</span><span class="sxs-lookup"><span data-stu-id="22d97-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="22d97-118">Вручную</span><span class="sxs-lookup"><span data-stu-id="22d97-118">manual</span></span>|<span data-ttu-id="22d97-119">2</span><span class="sxs-lookup"><span data-stu-id="22d97-119">2</span></span>|<span data-ttu-id="22d97-120">Синхронизация вручную.</span><span class="sxs-lookup"><span data-stu-id="22d97-120">Sync manually.</span></span>|
|<span data-ttu-id="22d97-121">фифтинминутес</span><span class="sxs-lookup"><span data-stu-id="22d97-121">fifteenMinutes</span></span>|<span data-ttu-id="22d97-122">4</span><span class="sxs-lookup"><span data-stu-id="22d97-122">3</span></span>|<span data-ttu-id="22d97-123">Синхронизация каждые пятнадцать минут.</span><span class="sxs-lookup"><span data-stu-id="22d97-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="22d97-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="22d97-124">thirtyMinutes</span></span>|<span data-ttu-id="22d97-125">4 </span><span class="sxs-lookup"><span data-stu-id="22d97-125">4</span></span>|<span data-ttu-id="22d97-126">Синхронизация каждые 30 минут.</span><span class="sxs-lookup"><span data-stu-id="22d97-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="22d97-127">сикстиминутес</span><span class="sxs-lookup"><span data-stu-id="22d97-127">sixtyMinutes</span></span>|<span data-ttu-id="22d97-128">5 </span><span class="sxs-lookup"><span data-stu-id="22d97-128">5</span></span>|<span data-ttu-id="22d97-129">Синхронизация каждые 60 минут.</span><span class="sxs-lookup"><span data-stu-id="22d97-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="22d97-130">баседонмюсаже</span><span class="sxs-lookup"><span data-stu-id="22d97-130">basedOnMyUsage</span></span>|<span data-ttu-id="22d97-131">6 </span><span class="sxs-lookup"><span data-stu-id="22d97-131">6</span></span>|<span data-ttu-id="22d97-132">Синхронизация с учетом использования.</span><span class="sxs-lookup"><span data-stu-id="22d97-132">Sync based on my usage.</span></span>|




