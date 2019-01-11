---
title: Тип перечисления deviceComplianceActionType
description: Запланировано действие типа Enum
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e2b89dbdaa3e67918b1b0c3e76eb6638e492994c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881874"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="73cf8-103">Тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="73cf8-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="73cf8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="73cf8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73cf8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73cf8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73cf8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="73cf8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73cf8-107">Запланировано действие типа Enum</span><span class="sxs-lookup"><span data-stu-id="73cf8-107">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="73cf8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="73cf8-108">Members</span></span>
|<span data-ttu-id="73cf8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="73cf8-109">Member</span></span>|<span data-ttu-id="73cf8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="73cf8-110">Value</span></span>|<span data-ttu-id="73cf8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="73cf8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73cf8-112">noAction</span><span class="sxs-lookup"><span data-stu-id="73cf8-112">noAction</span></span>|<span data-ttu-id="73cf8-113">0</span><span class="sxs-lookup"><span data-stu-id="73cf8-113">0</span></span>|<span data-ttu-id="73cf8-114">Никаких действий</span><span class="sxs-lookup"><span data-stu-id="73cf8-114">No Action</span></span>|
|<span data-ttu-id="73cf8-115">уведомления</span><span class="sxs-lookup"><span data-stu-id="73cf8-115">notification</span></span>|<span data-ttu-id="73cf8-116">1</span><span class="sxs-lookup"><span data-stu-id="73cf8-116">1</span></span>|<span data-ttu-id="73cf8-117">Отправить уведомление</span><span class="sxs-lookup"><span data-stu-id="73cf8-117">Send Notification</span></span>|
|<span data-ttu-id="73cf8-118">блок</span><span class="sxs-lookup"><span data-stu-id="73cf8-118">block</span></span>|<span data-ttu-id="73cf8-119">2</span><span class="sxs-lookup"><span data-stu-id="73cf8-119">2</span></span>|<span data-ttu-id="73cf8-120">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="73cf8-120">Block the device in AAD</span></span>|
|<span data-ttu-id="73cf8-121">Удаление</span><span class="sxs-lookup"><span data-stu-id="73cf8-121">retire</span></span>|<span data-ttu-id="73cf8-122">3</span><span class="sxs-lookup"><span data-stu-id="73cf8-122">3</span></span>|<span data-ttu-id="73cf8-123">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="73cf8-123">Retire the device</span></span>|
|<span data-ttu-id="73cf8-124">Очистка</span><span class="sxs-lookup"><span data-stu-id="73cf8-124">wipe</span></span>|<span data-ttu-id="73cf8-125">4</span><span class="sxs-lookup"><span data-stu-id="73cf8-125">4</span></span>|<span data-ttu-id="73cf8-126">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="73cf8-126">Wipe the device</span></span>|
|<span data-ttu-id="73cf8-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="73cf8-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="73cf8-128">5</span><span class="sxs-lookup"><span data-stu-id="73cf8-128">5</span></span>|<span data-ttu-id="73cf8-129">Удаление профилей доступа ресурсов с устройства</span><span class="sxs-lookup"><span data-stu-id="73cf8-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="73cf8-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="73cf8-130">pushNotification</span></span>|<span data-ttu-id="73cf8-131">9</span><span class="sxs-lookup"><span data-stu-id="73cf8-131">9</span></span>|<span data-ttu-id="73cf8-132">Отправить push-уведомлений для устройств</span><span class="sxs-lookup"><span data-stu-id="73cf8-132">Send push notification to device</span></span>|
|<span data-ttu-id="73cf8-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="73cf8-133">remoteLock</span></span>|<span data-ttu-id="73cf8-134">10</span><span class="sxs-lookup"><span data-stu-id="73cf8-134">10</span></span>|<span data-ttu-id="73cf8-135">Удаленно блокировка устройства</span><span class="sxs-lookup"><span data-stu-id="73cf8-135">Remotely lock the device</span></span>|





