---
title: тип перечисления Емаилсинксчедуле
description: Возможные значения для расписания синхронизации электронной почты.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e4d3645ea2c0eaa7f8f1cf8138f1c0727cfa0d8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325633"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="3e984-103">тип перечисления Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="3e984-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="3e984-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e984-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e984-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e984-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e984-106">Возможные значения для расписания синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3e984-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="3e984-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3e984-107">Members</span></span>
|<span data-ttu-id="3e984-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3e984-108">Member</span></span>|<span data-ttu-id="3e984-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3e984-109">Value</span></span>|<span data-ttu-id="3e984-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3e984-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e984-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="3e984-111">userDefined</span></span>|<span data-ttu-id="3e984-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3e984-112">0</span></span>|<span data-ttu-id="3e984-113">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="3e984-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="3e984-114">асмессажесарриве</span><span class="sxs-lookup"><span data-stu-id="3e984-114">asMessagesArrive</span></span>|<span data-ttu-id="3e984-115">1,1</span><span class="sxs-lookup"><span data-stu-id="3e984-115">1</span></span>|<span data-ttu-id="3e984-116">Синхронизация по мере поступления сообщений.</span><span class="sxs-lookup"><span data-stu-id="3e984-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="3e984-117">Вручную</span><span class="sxs-lookup"><span data-stu-id="3e984-117">manual</span></span>|<span data-ttu-id="3e984-118">2</span><span class="sxs-lookup"><span data-stu-id="3e984-118">2</span></span>|<span data-ttu-id="3e984-119">Синхронизация вручную.</span><span class="sxs-lookup"><span data-stu-id="3e984-119">Sync manually.</span></span>|
|<span data-ttu-id="3e984-120">фифтинминутес</span><span class="sxs-lookup"><span data-stu-id="3e984-120">fifteenMinutes</span></span>|<span data-ttu-id="3e984-121">4</span><span class="sxs-lookup"><span data-stu-id="3e984-121">3</span></span>|<span data-ttu-id="3e984-122">Синхронизация каждые пятнадцать минут.</span><span class="sxs-lookup"><span data-stu-id="3e984-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="3e984-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="3e984-123">thirtyMinutes</span></span>|<span data-ttu-id="3e984-124">SP4</span><span class="sxs-lookup"><span data-stu-id="3e984-124">4</span></span>|<span data-ttu-id="3e984-125">Синхронизация каждые 30 минут.</span><span class="sxs-lookup"><span data-stu-id="3e984-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="3e984-126">сикстиминутес</span><span class="sxs-lookup"><span data-stu-id="3e984-126">sixtyMinutes</span></span>|<span data-ttu-id="3e984-127">17:00</span><span class="sxs-lookup"><span data-stu-id="3e984-127">5</span></span>|<span data-ttu-id="3e984-128">Синхронизация каждые 60 минут.</span><span class="sxs-lookup"><span data-stu-id="3e984-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="3e984-129">баседонмюсаже</span><span class="sxs-lookup"><span data-stu-id="3e984-129">basedOnMyUsage</span></span>|<span data-ttu-id="3e984-130">6 </span><span class="sxs-lookup"><span data-stu-id="3e984-130">6</span></span>|<span data-ttu-id="3e984-131">Синхронизация с учетом использования.</span><span class="sxs-lookup"><span data-stu-id="3e984-131">Sync based on my usage.</span></span>|



