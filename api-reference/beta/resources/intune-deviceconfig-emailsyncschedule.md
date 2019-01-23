---
title: Тип перечисления emailSyncSchedule
description: Возможные значения для расписание синхронизации электронной почты.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8285b9a34e208b86b7c53c38e6aa015fd8c37560
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425185"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="034ca-103">Тип перечисления emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="034ca-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="034ca-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="034ca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="034ca-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="034ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="034ca-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="034ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="034ca-107">Возможные значения для расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="034ca-107">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="034ca-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="034ca-108">Members</span></span>
|<span data-ttu-id="034ca-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="034ca-109">Member</span></span>|<span data-ttu-id="034ca-110">Значение</span><span class="sxs-lookup"><span data-stu-id="034ca-110">Value</span></span>|<span data-ttu-id="034ca-111">Описание</span><span class="sxs-lookup"><span data-stu-id="034ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="034ca-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="034ca-112">userDefined</span></span>|<span data-ttu-id="034ca-113">0</span><span class="sxs-lookup"><span data-stu-id="034ca-113">0</span></span>|<span data-ttu-id="034ca-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="034ca-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="034ca-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="034ca-115">asMessagesArrive</span></span>|<span data-ttu-id="034ca-116">1</span><span class="sxs-lookup"><span data-stu-id="034ca-116">1</span></span>|<span data-ttu-id="034ca-117">Синхронизация по мере поступления сообщений.</span><span class="sxs-lookup"><span data-stu-id="034ca-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="034ca-118">Вручную</span><span class="sxs-lookup"><span data-stu-id="034ca-118">manual</span></span>|<span data-ttu-id="034ca-119">2</span><span class="sxs-lookup"><span data-stu-id="034ca-119">2</span></span>|<span data-ttu-id="034ca-120">Синхронизируйте вручную.</span><span class="sxs-lookup"><span data-stu-id="034ca-120">Sync manually.</span></span>|
|<span data-ttu-id="034ca-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="034ca-121">fifteenMinutes</span></span>|<span data-ttu-id="034ca-122">3</span><span class="sxs-lookup"><span data-stu-id="034ca-122">3</span></span>|<span data-ttu-id="034ca-123">Синхронизация каждые 15 минут.</span><span class="sxs-lookup"><span data-stu-id="034ca-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="034ca-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="034ca-124">thirtyMinutes</span></span>|<span data-ttu-id="034ca-125">4</span><span class="sxs-lookup"><span data-stu-id="034ca-125">4</span></span>|<span data-ttu-id="034ca-126">Синхронизация каждые 30 минут.</span><span class="sxs-lookup"><span data-stu-id="034ca-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="034ca-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="034ca-127">sixtyMinutes</span></span>|<span data-ttu-id="034ca-128">5</span><span class="sxs-lookup"><span data-stu-id="034ca-128">5</span></span>|<span data-ttu-id="034ca-129">Синхронизация каждые 60 минут.</span><span class="sxs-lookup"><span data-stu-id="034ca-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="034ca-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="034ca-130">basedOnMyUsage</span></span>|<span data-ttu-id="034ca-131">6</span><span class="sxs-lookup"><span data-stu-id="034ca-131">6</span></span>|<span data-ttu-id="034ca-132">Синхронизация на основе Мои использования.</span><span class="sxs-lookup"><span data-stu-id="034ca-132">Sync based on my usage.</span></span>|




