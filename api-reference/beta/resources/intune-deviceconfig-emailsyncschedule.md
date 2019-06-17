---
title: тип перечисления Емаилсинксчедуле
description: Возможные значения для расписания синхронизации электронной почты.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f84c9a5cdb5d9608a34553c2a3a6f05a989b78a8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995065"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="5601e-103">тип перечисления Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="5601e-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="5601e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5601e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5601e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5601e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5601e-106">Возможные значения для расписания синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5601e-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="5601e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5601e-107">Members</span></span>
|<span data-ttu-id="5601e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5601e-108">Member</span></span>|<span data-ttu-id="5601e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5601e-109">Value</span></span>|<span data-ttu-id="5601e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5601e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5601e-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="5601e-111">userDefined</span></span>|<span data-ttu-id="5601e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5601e-112">0</span></span>|<span data-ttu-id="5601e-113">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="5601e-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="5601e-114">Асмессажесарриве</span><span class="sxs-lookup"><span data-stu-id="5601e-114">asMessagesArrive</span></span>|<span data-ttu-id="5601e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="5601e-115">1</span></span>|<span data-ttu-id="5601e-116">Синхронизация по мере поступления сообщений.</span><span class="sxs-lookup"><span data-stu-id="5601e-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="5601e-117">Вручную</span><span class="sxs-lookup"><span data-stu-id="5601e-117">manual</span></span>|<span data-ttu-id="5601e-118">2</span><span class="sxs-lookup"><span data-stu-id="5601e-118">2</span></span>|<span data-ttu-id="5601e-119">Синхронизация вручную.</span><span class="sxs-lookup"><span data-stu-id="5601e-119">Sync manually.</span></span>|
|<span data-ttu-id="5601e-120">Фифтинминутес</span><span class="sxs-lookup"><span data-stu-id="5601e-120">fifteenMinutes</span></span>|<span data-ttu-id="5601e-121">4</span><span class="sxs-lookup"><span data-stu-id="5601e-121">3</span></span>|<span data-ttu-id="5601e-122">Синхронизация каждые пятнадцать минут.</span><span class="sxs-lookup"><span data-stu-id="5601e-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="5601e-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="5601e-123">thirtyMinutes</span></span>|<span data-ttu-id="5601e-124">SP4</span><span class="sxs-lookup"><span data-stu-id="5601e-124">4</span></span>|<span data-ttu-id="5601e-125">Синхронизация каждые 30 минут.</span><span class="sxs-lookup"><span data-stu-id="5601e-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="5601e-126">Сикстиминутес</span><span class="sxs-lookup"><span data-stu-id="5601e-126">sixtyMinutes</span></span>|<span data-ttu-id="5601e-127">17:00</span><span class="sxs-lookup"><span data-stu-id="5601e-127">5</span></span>|<span data-ttu-id="5601e-128">Синхронизация каждые 60 минут.</span><span class="sxs-lookup"><span data-stu-id="5601e-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="5601e-129">Баседонмюсаже</span><span class="sxs-lookup"><span data-stu-id="5601e-129">basedOnMyUsage</span></span>|<span data-ttu-id="5601e-130">6 </span><span class="sxs-lookup"><span data-stu-id="5601e-130">6</span></span>|<span data-ttu-id="5601e-131">Синхронизация с учетом использования.</span><span class="sxs-lookup"><span data-stu-id="5601e-131">Sync based on my usage.</span></span>|





