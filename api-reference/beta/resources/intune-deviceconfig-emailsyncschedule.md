---
title: Тип перечисления emailSyncSchedule
description: Возможные значения для расписание синхронизации электронной почты.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 178cba9e226b7f20e3fd917145e7bbd06f6c3a1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838397"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="bd14f-103">Тип перечисления emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="bd14f-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="bd14f-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bd14f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd14f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd14f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd14f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bd14f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd14f-107">Возможные значения для расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="bd14f-107">Possible values for email sync schedule.</span></span>
## <a name="members"></a><span data-ttu-id="bd14f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="bd14f-108">Members</span></span>
|<span data-ttu-id="bd14f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="bd14f-109">Member</span></span>|<span data-ttu-id="bd14f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="bd14f-110">Value</span></span>|<span data-ttu-id="bd14f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bd14f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd14f-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="bd14f-112">userDefined</span></span>|<span data-ttu-id="bd14f-113">0</span><span class="sxs-lookup"><span data-stu-id="bd14f-113">0</span></span>|<span data-ttu-id="bd14f-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="bd14f-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="bd14f-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="bd14f-115">asMessagesArrive</span></span>|<span data-ttu-id="bd14f-116">1</span><span class="sxs-lookup"><span data-stu-id="bd14f-116">1</span></span>|<span data-ttu-id="bd14f-117">Синхронизация по мере поступления сообщений.</span><span class="sxs-lookup"><span data-stu-id="bd14f-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="bd14f-118">Вручную</span><span class="sxs-lookup"><span data-stu-id="bd14f-118">manual</span></span>|<span data-ttu-id="bd14f-119">2</span><span class="sxs-lookup"><span data-stu-id="bd14f-119">2</span></span>|<span data-ttu-id="bd14f-120">Синхронизируйте вручную.</span><span class="sxs-lookup"><span data-stu-id="bd14f-120">Sync manually.</span></span>|
|<span data-ttu-id="bd14f-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="bd14f-121">fifteenMinutes</span></span>|<span data-ttu-id="bd14f-122">3</span><span class="sxs-lookup"><span data-stu-id="bd14f-122">3</span></span>|<span data-ttu-id="bd14f-123">Синхронизация каждые 15 минут.</span><span class="sxs-lookup"><span data-stu-id="bd14f-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="bd14f-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="bd14f-124">thirtyMinutes</span></span>|<span data-ttu-id="bd14f-125">4</span><span class="sxs-lookup"><span data-stu-id="bd14f-125">4</span></span>|<span data-ttu-id="bd14f-126">Синхронизация каждые 30 минут.</span><span class="sxs-lookup"><span data-stu-id="bd14f-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="bd14f-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="bd14f-127">sixtyMinutes</span></span>|<span data-ttu-id="bd14f-128">5</span><span class="sxs-lookup"><span data-stu-id="bd14f-128">5</span></span>|<span data-ttu-id="bd14f-129">Синхронизация каждые 60 минут.</span><span class="sxs-lookup"><span data-stu-id="bd14f-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="bd14f-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="bd14f-130">basedOnMyUsage</span></span>|<span data-ttu-id="bd14f-131">6</span><span class="sxs-lookup"><span data-stu-id="bd14f-131">6</span></span>|<span data-ttu-id="bd14f-132">Синхронизация на основе Мои использования.</span><span class="sxs-lookup"><span data-stu-id="bd14f-132">Sync based on my usage.</span></span>|





