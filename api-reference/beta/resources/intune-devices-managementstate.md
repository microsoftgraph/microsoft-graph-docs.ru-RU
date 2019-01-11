---
title: Тип перечисления managementState
description: Состояние управления устройство в Майкрософт Intune.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c439cf0ff830f471d2050eee81c91c6539e66d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844655"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="0a88a-103">Тип перечисления managementState</span><span class="sxs-lookup"><span data-stu-id="0a88a-103">managementState enum type</span></span>

> <span data-ttu-id="0a88a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a88a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a88a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a88a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a88a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0a88a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a88a-107">Состояние управления устройство в Майкрософт Intune.</span><span class="sxs-lookup"><span data-stu-id="0a88a-107">Management state of device in Microsoft Intune.</span></span>
## <a name="members"></a><span data-ttu-id="0a88a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0a88a-108">Members</span></span>
|<span data-ttu-id="0a88a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0a88a-109">Member</span></span>|<span data-ttu-id="0a88a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0a88a-110">Value</span></span>|<span data-ttu-id="0a88a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a88a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a88a-112">управляемые</span><span class="sxs-lookup"><span data-stu-id="0a88a-112">managed</span></span>|<span data-ttu-id="0a88a-113">0</span><span class="sxs-lookup"><span data-stu-id="0a88a-113">0</span></span>|<span data-ttu-id="0a88a-114">Устройство находится в разделе Управление</span><span class="sxs-lookup"><span data-stu-id="0a88a-114">The device is under management</span></span>|
|<span data-ttu-id="0a88a-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="0a88a-115">retirePending</span></span>|<span data-ttu-id="0a88a-116">1</span><span class="sxs-lookup"><span data-stu-id="0a88a-116">1</span></span>|<span data-ttu-id="0a88a-117">Команда retire — отмену на устройстве и в процессе unenrolling из управления</span><span class="sxs-lookup"><span data-stu-id="0a88a-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="0a88a-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="0a88a-118">retireFailed</span></span>|<span data-ttu-id="0a88a-119">2</span><span class="sxs-lookup"><span data-stu-id="0a88a-119">2</span></span>|<span data-ttu-id="0a88a-120">Удаление команды не удалось выполнить на устройстве</span><span class="sxs-lookup"><span data-stu-id="0a88a-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="0a88a-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="0a88a-121">wipePending</span></span>|<span data-ttu-id="0a88a-122">3</span><span class="sxs-lookup"><span data-stu-id="0a88a-122">3</span></span>|<span data-ttu-id="0a88a-123">Команда очистки — отмену на устройстве и в процессе unenrolling из управления</span><span class="sxs-lookup"><span data-stu-id="0a88a-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="0a88a-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="0a88a-124">wipeFailed</span></span>|<span data-ttu-id="0a88a-125">4</span><span class="sxs-lookup"><span data-stu-id="0a88a-125">4</span></span>|<span data-ttu-id="0a88a-126">Не удалось выполнить команду очистки на устройстве</span><span class="sxs-lookup"><span data-stu-id="0a88a-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="0a88a-127">неработоспособные</span><span class="sxs-lookup"><span data-stu-id="0a88a-127">unhealthy</span></span>|<span data-ttu-id="0a88a-128">5</span><span class="sxs-lookup"><span data-stu-id="0a88a-128">5</span></span>|<span data-ttu-id="0a88a-129">Устройство работает неправильно.</span><span class="sxs-lookup"><span data-stu-id="0a88a-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="0a88a-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="0a88a-130">deletePending</span></span>|<span data-ttu-id="0a88a-131">6</span><span class="sxs-lookup"><span data-stu-id="0a88a-131">6</span></span>|<span data-ttu-id="0a88a-132">Команда Удалить является отмену на устройстве</span><span class="sxs-lookup"><span data-stu-id="0a88a-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="0a88a-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="0a88a-133">retireIssued</span></span>|<span data-ttu-id="0a88a-134">7</span><span class="sxs-lookup"><span data-stu-id="0a88a-134">7</span></span>|<span data-ttu-id="0a88a-135">Команда retire был отправлен для устройства</span><span class="sxs-lookup"><span data-stu-id="0a88a-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="0a88a-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="0a88a-136">wipeIssued</span></span>|<span data-ttu-id="0a88a-137">8</span><span class="sxs-lookup"><span data-stu-id="0a88a-137">8</span></span>|<span data-ttu-id="0a88a-138">Команда очистки был отправлен для устройства</span><span class="sxs-lookup"><span data-stu-id="0a88a-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="0a88a-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="0a88a-139">wipeCanceled</span></span>|<span data-ttu-id="0a88a-140">9</span><span class="sxs-lookup"><span data-stu-id="0a88a-140">9</span></span>|<span data-ttu-id="0a88a-141">Команда очистки для этого устройства была отменена</span><span class="sxs-lookup"><span data-stu-id="0a88a-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="0a88a-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="0a88a-142">retireCanceled</span></span>|<span data-ttu-id="0a88a-143">10</span><span class="sxs-lookup"><span data-stu-id="0a88a-143">10</span></span>|<span data-ttu-id="0a88a-144">Команда retire для этого устройства была отменена</span><span class="sxs-lookup"><span data-stu-id="0a88a-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="0a88a-145">Обнаружен</span><span class="sxs-lookup"><span data-stu-id="0a88a-145">discovered</span></span>|<span data-ttu-id="0a88a-146">11</span><span class="sxs-lookup"><span data-stu-id="0a88a-146">11</span></span>|<span data-ttu-id="0a88a-147">Устройство обнаружен, но не полностью зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="0a88a-147">The device is discovered but not fully enrolled.</span></span>|





