---
title: тип перечисления Емаилсинксчедуле
description: Возможные значения для расписания синхронизации электронной почты.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f2d7d9d4918946b3683bce5f118fa9a04edf7afe
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791802"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="972b9-103">тип перечисления Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="972b9-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="972b9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="972b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="972b9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="972b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="972b9-106">Возможные значения для расписания синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="972b9-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="972b9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="972b9-107">Members</span></span>
|<span data-ttu-id="972b9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="972b9-108">Member</span></span>|<span data-ttu-id="972b9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="972b9-109">Value</span></span>|<span data-ttu-id="972b9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="972b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="972b9-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="972b9-111">userDefined</span></span>|<span data-ttu-id="972b9-112">нуль</span><span class="sxs-lookup"><span data-stu-id="972b9-112">0</span></span>|<span data-ttu-id="972b9-113">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="972b9-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="972b9-114">асмессажесарриве</span><span class="sxs-lookup"><span data-stu-id="972b9-114">asMessagesArrive</span></span>|<span data-ttu-id="972b9-115">1,1</span><span class="sxs-lookup"><span data-stu-id="972b9-115">1</span></span>|<span data-ttu-id="972b9-116">Синхронизация по мере поступления сообщений.</span><span class="sxs-lookup"><span data-stu-id="972b9-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="972b9-117">Вручную</span><span class="sxs-lookup"><span data-stu-id="972b9-117">manual</span></span>|<span data-ttu-id="972b9-118">2</span><span class="sxs-lookup"><span data-stu-id="972b9-118">2</span></span>|<span data-ttu-id="972b9-119">Синхронизация вручную.</span><span class="sxs-lookup"><span data-stu-id="972b9-119">Sync manually.</span></span>|
|<span data-ttu-id="972b9-120">фифтинминутес</span><span class="sxs-lookup"><span data-stu-id="972b9-120">fifteenMinutes</span></span>|<span data-ttu-id="972b9-121">4</span><span class="sxs-lookup"><span data-stu-id="972b9-121">3</span></span>|<span data-ttu-id="972b9-122">Синхронизация каждые пятнадцать минут.</span><span class="sxs-lookup"><span data-stu-id="972b9-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="972b9-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="972b9-123">thirtyMinutes</span></span>|<span data-ttu-id="972b9-124">4 </span><span class="sxs-lookup"><span data-stu-id="972b9-124">4</span></span>|<span data-ttu-id="972b9-125">Синхронизация каждые 30 минут.</span><span class="sxs-lookup"><span data-stu-id="972b9-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="972b9-126">сикстиминутес</span><span class="sxs-lookup"><span data-stu-id="972b9-126">sixtyMinutes</span></span>|<span data-ttu-id="972b9-127">5 </span><span class="sxs-lookup"><span data-stu-id="972b9-127">5</span></span>|<span data-ttu-id="972b9-128">Синхронизация каждые 60 минут.</span><span class="sxs-lookup"><span data-stu-id="972b9-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="972b9-129">баседонмюсаже</span><span class="sxs-lookup"><span data-stu-id="972b9-129">basedOnMyUsage</span></span>|<span data-ttu-id="972b9-130">6 </span><span class="sxs-lookup"><span data-stu-id="972b9-130">6</span></span>|<span data-ttu-id="972b9-131">Синхронизация с учетом использования.</span><span class="sxs-lookup"><span data-stu-id="972b9-131">Sync based on my usage.</span></span>|



