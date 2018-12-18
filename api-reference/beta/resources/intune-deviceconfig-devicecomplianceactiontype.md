---
title: Тип перечисления deviceComplianceActionType
description: Запланировано действие типа Enum
author: tfitzmac
ms.openlocfilehash: 9fd0a8bd045ad04fe0acf55f899e693d7fcce5d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335688"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="ef5df-103">Тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="ef5df-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="ef5df-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ef5df-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef5df-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef5df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef5df-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ef5df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef5df-107">Запланировано действие типа Enum</span><span class="sxs-lookup"><span data-stu-id="ef5df-107">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="ef5df-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ef5df-108">Members</span></span>
|<span data-ttu-id="ef5df-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ef5df-109">Member</span></span>|<span data-ttu-id="ef5df-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ef5df-110">Value</span></span>|<span data-ttu-id="ef5df-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ef5df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef5df-112">noAction</span><span class="sxs-lookup"><span data-stu-id="ef5df-112">noAction</span></span>|<span data-ttu-id="ef5df-113">0</span><span class="sxs-lookup"><span data-stu-id="ef5df-113">0</span></span>|<span data-ttu-id="ef5df-114">Никаких действий</span><span class="sxs-lookup"><span data-stu-id="ef5df-114">No Action</span></span>|
|<span data-ttu-id="ef5df-115">уведомления</span><span class="sxs-lookup"><span data-stu-id="ef5df-115">notification</span></span>|<span data-ttu-id="ef5df-116">1</span><span class="sxs-lookup"><span data-stu-id="ef5df-116">1</span></span>|<span data-ttu-id="ef5df-117">Отправить уведомление</span><span class="sxs-lookup"><span data-stu-id="ef5df-117">Send Notification</span></span>|
|<span data-ttu-id="ef5df-118">блок</span><span class="sxs-lookup"><span data-stu-id="ef5df-118">block</span></span>|<span data-ttu-id="ef5df-119">2</span><span class="sxs-lookup"><span data-stu-id="ef5df-119">2</span></span>|<span data-ttu-id="ef5df-120">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="ef5df-120">Block the device in AAD</span></span>|
|<span data-ttu-id="ef5df-121">Удаление</span><span class="sxs-lookup"><span data-stu-id="ef5df-121">retire</span></span>|<span data-ttu-id="ef5df-122">3</span><span class="sxs-lookup"><span data-stu-id="ef5df-122">3</span></span>|<span data-ttu-id="ef5df-123">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="ef5df-123">Retire the device</span></span>|
|<span data-ttu-id="ef5df-124">Очистка</span><span class="sxs-lookup"><span data-stu-id="ef5df-124">wipe</span></span>|<span data-ttu-id="ef5df-125">4</span><span class="sxs-lookup"><span data-stu-id="ef5df-125">4</span></span>|<span data-ttu-id="ef5df-126">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="ef5df-126">Wipe the device</span></span>|
|<span data-ttu-id="ef5df-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="ef5df-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="ef5df-128">5</span><span class="sxs-lookup"><span data-stu-id="ef5df-128">5</span></span>|<span data-ttu-id="ef5df-129">Удаление профилей доступа ресурсов с устройства</span><span class="sxs-lookup"><span data-stu-id="ef5df-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="ef5df-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="ef5df-130">pushNotification</span></span>|<span data-ttu-id="ef5df-131">9</span><span class="sxs-lookup"><span data-stu-id="ef5df-131">9</span></span>|<span data-ttu-id="ef5df-132">Отправить push-уведомлений для устройств</span><span class="sxs-lookup"><span data-stu-id="ef5df-132">Send push notification to device</span></span>|
|<span data-ttu-id="ef5df-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="ef5df-133">remoteLock</span></span>|<span data-ttu-id="ef5df-134">10</span><span class="sxs-lookup"><span data-stu-id="ef5df-134">10</span></span>|<span data-ttu-id="ef5df-135">Удаленно блокировка устройства</span><span class="sxs-lookup"><span data-stu-id="ef5df-135">Remotely lock the device</span></span>|





