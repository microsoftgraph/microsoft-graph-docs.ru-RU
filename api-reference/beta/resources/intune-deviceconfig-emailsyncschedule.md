---
title: тип перечисления Емаилсинксчедуле
description: Возможные значения для расписания синхронизации электронной почты.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 14b73fc4cfbf9cf53bdab4c2841403cac4077fa2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001427"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="a3b15-103">тип перечисления Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="a3b15-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="a3b15-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3b15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3b15-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3b15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3b15-106">Возможные значения для расписания синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a3b15-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="a3b15-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="a3b15-107">Members</span></span>
|<span data-ttu-id="a3b15-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="a3b15-108">Member</span></span>|<span data-ttu-id="a3b15-109">Значение</span><span class="sxs-lookup"><span data-stu-id="a3b15-109">Value</span></span>|<span data-ttu-id="a3b15-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a3b15-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3b15-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="a3b15-111">userDefined</span></span>|<span data-ttu-id="a3b15-112">нуль</span><span class="sxs-lookup"><span data-stu-id="a3b15-112">0</span></span>|<span data-ttu-id="a3b15-113">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="a3b15-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="a3b15-114">Асмессажесарриве</span><span class="sxs-lookup"><span data-stu-id="a3b15-114">asMessagesArrive</span></span>|<span data-ttu-id="a3b15-115">1,1</span><span class="sxs-lookup"><span data-stu-id="a3b15-115">1</span></span>|<span data-ttu-id="a3b15-116">Синхронизация по мере поступления сообщений.</span><span class="sxs-lookup"><span data-stu-id="a3b15-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="a3b15-117">Вручную</span><span class="sxs-lookup"><span data-stu-id="a3b15-117">manual</span></span>|<span data-ttu-id="a3b15-118">2</span><span class="sxs-lookup"><span data-stu-id="a3b15-118">2</span></span>|<span data-ttu-id="a3b15-119">Синхронизация вручную.</span><span class="sxs-lookup"><span data-stu-id="a3b15-119">Sync manually.</span></span>|
|<span data-ttu-id="a3b15-120">Фифтинминутес</span><span class="sxs-lookup"><span data-stu-id="a3b15-120">fifteenMinutes</span></span>|<span data-ttu-id="a3b15-121">4</span><span class="sxs-lookup"><span data-stu-id="a3b15-121">3</span></span>|<span data-ttu-id="a3b15-122">Синхронизация каждые пятнадцать минут.</span><span class="sxs-lookup"><span data-stu-id="a3b15-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="a3b15-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="a3b15-123">thirtyMinutes</span></span>|<span data-ttu-id="a3b15-124">SP4</span><span class="sxs-lookup"><span data-stu-id="a3b15-124">4</span></span>|<span data-ttu-id="a3b15-125">Синхронизация каждые 30 минут.</span><span class="sxs-lookup"><span data-stu-id="a3b15-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="a3b15-126">Сикстиминутес</span><span class="sxs-lookup"><span data-stu-id="a3b15-126">sixtyMinutes</span></span>|<span data-ttu-id="a3b15-127">17:00</span><span class="sxs-lookup"><span data-stu-id="a3b15-127">5</span></span>|<span data-ttu-id="a3b15-128">Синхронизация каждые 60 минут.</span><span class="sxs-lookup"><span data-stu-id="a3b15-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="a3b15-129">Баседонмюсаже</span><span class="sxs-lookup"><span data-stu-id="a3b15-129">basedOnMyUsage</span></span>|<span data-ttu-id="a3b15-130">6 </span><span class="sxs-lookup"><span data-stu-id="a3b15-130">6</span></span>|<span data-ttu-id="a3b15-131">Синхронизация с учетом использования.</span><span class="sxs-lookup"><span data-stu-id="a3b15-131">Sync based on my usage.</span></span>|





