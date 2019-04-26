---
title: тип перечисления Емаилсинксчедуле
description: Возможные значения для расписания синхронизации электронной почты.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1da569d7050e88dd5eb41640bc2d8eaa602bb2b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556223"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="284c9-103">тип перечисления Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="284c9-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="284c9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="284c9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="284c9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="284c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="284c9-106">Возможные значения для расписания синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="284c9-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="284c9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="284c9-107">Members</span></span>
|<span data-ttu-id="284c9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="284c9-108">Member</span></span>|<span data-ttu-id="284c9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="284c9-109">Value</span></span>|<span data-ttu-id="284c9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="284c9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="284c9-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="284c9-111">userDefined</span></span>|<span data-ttu-id="284c9-112">нуль</span><span class="sxs-lookup"><span data-stu-id="284c9-112">0</span></span>|<span data-ttu-id="284c9-113">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="284c9-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="284c9-114">Асмессажесарриве</span><span class="sxs-lookup"><span data-stu-id="284c9-114">asMessagesArrive</span></span>|<span data-ttu-id="284c9-115">1 </span><span class="sxs-lookup"><span data-stu-id="284c9-115">1</span></span>|<span data-ttu-id="284c9-116">Синхронизация по мере поступления сообщений.</span><span class="sxs-lookup"><span data-stu-id="284c9-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="284c9-117">Вручную</span><span class="sxs-lookup"><span data-stu-id="284c9-117">manual</span></span>|<span data-ttu-id="284c9-118">2 </span><span class="sxs-lookup"><span data-stu-id="284c9-118">2</span></span>|<span data-ttu-id="284c9-119">Синхронизация вручную.</span><span class="sxs-lookup"><span data-stu-id="284c9-119">Sync manually.</span></span>|
|<span data-ttu-id="284c9-120">Фифтинминутес</span><span class="sxs-lookup"><span data-stu-id="284c9-120">fifteenMinutes</span></span>|<span data-ttu-id="284c9-121">3 </span><span class="sxs-lookup"><span data-stu-id="284c9-121">3</span></span>|<span data-ttu-id="284c9-122">Синхронизация каждые пятнадцать минут.</span><span class="sxs-lookup"><span data-stu-id="284c9-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="284c9-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="284c9-123">thirtyMinutes</span></span>|<span data-ttu-id="284c9-124">4 </span><span class="sxs-lookup"><span data-stu-id="284c9-124">4</span></span>|<span data-ttu-id="284c9-125">Синхронизация каждые 30 минут.</span><span class="sxs-lookup"><span data-stu-id="284c9-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="284c9-126">Сикстиминутес</span><span class="sxs-lookup"><span data-stu-id="284c9-126">sixtyMinutes</span></span>|<span data-ttu-id="284c9-127">5 </span><span class="sxs-lookup"><span data-stu-id="284c9-127">5</span></span>|<span data-ttu-id="284c9-128">Синхронизация каждые 60 минут.</span><span class="sxs-lookup"><span data-stu-id="284c9-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="284c9-129">Баседонмюсаже</span><span class="sxs-lookup"><span data-stu-id="284c9-129">basedOnMyUsage</span></span>|<span data-ttu-id="284c9-130">6 </span><span class="sxs-lookup"><span data-stu-id="284c9-130">6</span></span>|<span data-ttu-id="284c9-131">Синхронизация с учетом использования.</span><span class="sxs-lookup"><span data-stu-id="284c9-131">Sync based on my usage.</span></span>|





