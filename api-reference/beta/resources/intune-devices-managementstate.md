---
title: Тип перечисления managementState
description: Состояние управления устройство в Майкрософт Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7d9d083c56df366b9f896432328d51c295f62190
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961948"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="a0873-103">Тип перечисления managementState</span><span class="sxs-lookup"><span data-stu-id="a0873-103">managementState enum type</span></span>

> <span data-ttu-id="a0873-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a0873-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0873-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0873-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0873-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a0873-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0873-107">Состояние управления устройство в Майкрософт Intune.</span><span class="sxs-lookup"><span data-stu-id="a0873-107">Management state of device in Microsoft Intune.</span></span>
## <a name="members"></a><span data-ttu-id="a0873-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a0873-108">Members</span></span>
|<span data-ttu-id="a0873-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a0873-109">Member</span></span>|<span data-ttu-id="a0873-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a0873-110">Value</span></span>|<span data-ttu-id="a0873-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a0873-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0873-112">управляемые</span><span class="sxs-lookup"><span data-stu-id="a0873-112">managed</span></span>|<span data-ttu-id="a0873-113">0</span><span class="sxs-lookup"><span data-stu-id="a0873-113">0</span></span>|<span data-ttu-id="a0873-114">Устройство находится в разделе Управление</span><span class="sxs-lookup"><span data-stu-id="a0873-114">The device is under management</span></span>|
|<span data-ttu-id="a0873-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="a0873-115">retirePending</span></span>|<span data-ttu-id="a0873-116">1</span><span class="sxs-lookup"><span data-stu-id="a0873-116">1</span></span>|<span data-ttu-id="a0873-117">Команда retire — отмену на устройстве и в процессе unenrolling из управления</span><span class="sxs-lookup"><span data-stu-id="a0873-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="a0873-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="a0873-118">retireFailed</span></span>|<span data-ttu-id="a0873-119">2</span><span class="sxs-lookup"><span data-stu-id="a0873-119">2</span></span>|<span data-ttu-id="a0873-120">Удаление команды не удалось выполнить на устройстве</span><span class="sxs-lookup"><span data-stu-id="a0873-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="a0873-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="a0873-121">wipePending</span></span>|<span data-ttu-id="a0873-122">3</span><span class="sxs-lookup"><span data-stu-id="a0873-122">3</span></span>|<span data-ttu-id="a0873-123">Команда очистки — отмену на устройстве и в процессе unenrolling из управления</span><span class="sxs-lookup"><span data-stu-id="a0873-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="a0873-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="a0873-124">wipeFailed</span></span>|<span data-ttu-id="a0873-125">4</span><span class="sxs-lookup"><span data-stu-id="a0873-125">4</span></span>|<span data-ttu-id="a0873-126">Не удалось выполнить команду очистки на устройстве</span><span class="sxs-lookup"><span data-stu-id="a0873-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="a0873-127">неработоспособные</span><span class="sxs-lookup"><span data-stu-id="a0873-127">unhealthy</span></span>|<span data-ttu-id="a0873-128">5</span><span class="sxs-lookup"><span data-stu-id="a0873-128">5</span></span>|<span data-ttu-id="a0873-129">Устройство работает неправильно.</span><span class="sxs-lookup"><span data-stu-id="a0873-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="a0873-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="a0873-130">deletePending</span></span>|<span data-ttu-id="a0873-131">6</span><span class="sxs-lookup"><span data-stu-id="a0873-131">6</span></span>|<span data-ttu-id="a0873-132">Команда Удалить является отмену на устройстве</span><span class="sxs-lookup"><span data-stu-id="a0873-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="a0873-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="a0873-133">retireIssued</span></span>|<span data-ttu-id="a0873-134">7</span><span class="sxs-lookup"><span data-stu-id="a0873-134">7</span></span>|<span data-ttu-id="a0873-135">Команда retire был отправлен для устройства</span><span class="sxs-lookup"><span data-stu-id="a0873-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="a0873-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="a0873-136">wipeIssued</span></span>|<span data-ttu-id="a0873-137">8</span><span class="sxs-lookup"><span data-stu-id="a0873-137">8</span></span>|<span data-ttu-id="a0873-138">Команда очистки был отправлен для устройства</span><span class="sxs-lookup"><span data-stu-id="a0873-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="a0873-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="a0873-139">wipeCanceled</span></span>|<span data-ttu-id="a0873-140">9</span><span class="sxs-lookup"><span data-stu-id="a0873-140">9</span></span>|<span data-ttu-id="a0873-141">Команда очистки для этого устройства была отменена</span><span class="sxs-lookup"><span data-stu-id="a0873-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="a0873-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="a0873-142">retireCanceled</span></span>|<span data-ttu-id="a0873-143">10</span><span class="sxs-lookup"><span data-stu-id="a0873-143">10</span></span>|<span data-ttu-id="a0873-144">Команда retire для этого устройства была отменена</span><span class="sxs-lookup"><span data-stu-id="a0873-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="a0873-145">Обнаружен</span><span class="sxs-lookup"><span data-stu-id="a0873-145">discovered</span></span>|<span data-ttu-id="a0873-146">11</span><span class="sxs-lookup"><span data-stu-id="a0873-146">11</span></span>|<span data-ttu-id="a0873-147">Устройство обнаружен, но не полностью зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="a0873-147">The device is discovered but not fully enrolled.</span></span>|





