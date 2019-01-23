---
title: Тип перечисления managementState
description: Состояние управления устройство в Майкрософт Intune.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8d0801949125f3b0cceb865ac1f8546195112e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420019"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="70104-103">Тип перечисления managementState</span><span class="sxs-lookup"><span data-stu-id="70104-103">managementState enum type</span></span>

> <span data-ttu-id="70104-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="70104-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="70104-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70104-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70104-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70104-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70104-107">Состояние управления устройство в Майкрософт Intune.</span><span class="sxs-lookup"><span data-stu-id="70104-107">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="70104-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="70104-108">Members</span></span>
|<span data-ttu-id="70104-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="70104-109">Member</span></span>|<span data-ttu-id="70104-110">Значение</span><span class="sxs-lookup"><span data-stu-id="70104-110">Value</span></span>|<span data-ttu-id="70104-111">Описание</span><span class="sxs-lookup"><span data-stu-id="70104-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70104-112">управляемые</span><span class="sxs-lookup"><span data-stu-id="70104-112">managed</span></span>|<span data-ttu-id="70104-113">0</span><span class="sxs-lookup"><span data-stu-id="70104-113">0</span></span>|<span data-ttu-id="70104-114">Устройство находится в разделе Управление</span><span class="sxs-lookup"><span data-stu-id="70104-114">The device is under management</span></span>|
|<span data-ttu-id="70104-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="70104-115">retirePending</span></span>|<span data-ttu-id="70104-116">1</span><span class="sxs-lookup"><span data-stu-id="70104-116">1</span></span>|<span data-ttu-id="70104-117">Команда retire — отмену на устройстве и в процессе unenrolling из управления</span><span class="sxs-lookup"><span data-stu-id="70104-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="70104-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="70104-118">retireFailed</span></span>|<span data-ttu-id="70104-119">2</span><span class="sxs-lookup"><span data-stu-id="70104-119">2</span></span>|<span data-ttu-id="70104-120">Удаление команды не удалось выполнить на устройстве</span><span class="sxs-lookup"><span data-stu-id="70104-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="70104-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="70104-121">wipePending</span></span>|<span data-ttu-id="70104-122">3</span><span class="sxs-lookup"><span data-stu-id="70104-122">3</span></span>|<span data-ttu-id="70104-123">Команда очистки — отмену на устройстве и в процессе unenrolling из управления</span><span class="sxs-lookup"><span data-stu-id="70104-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="70104-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="70104-124">wipeFailed</span></span>|<span data-ttu-id="70104-125">4</span><span class="sxs-lookup"><span data-stu-id="70104-125">4</span></span>|<span data-ttu-id="70104-126">Не удалось выполнить команду очистки на устройстве</span><span class="sxs-lookup"><span data-stu-id="70104-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="70104-127">неработоспособные</span><span class="sxs-lookup"><span data-stu-id="70104-127">unhealthy</span></span>|<span data-ttu-id="70104-128">5</span><span class="sxs-lookup"><span data-stu-id="70104-128">5</span></span>|<span data-ttu-id="70104-129">Устройство работает неправильно.</span><span class="sxs-lookup"><span data-stu-id="70104-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="70104-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="70104-130">deletePending</span></span>|<span data-ttu-id="70104-131">6</span><span class="sxs-lookup"><span data-stu-id="70104-131">6</span></span>|<span data-ttu-id="70104-132">Команда Удалить является отмену на устройстве</span><span class="sxs-lookup"><span data-stu-id="70104-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="70104-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="70104-133">retireIssued</span></span>|<span data-ttu-id="70104-134">7</span><span class="sxs-lookup"><span data-stu-id="70104-134">7</span></span>|<span data-ttu-id="70104-135">Команда retire был отправлен для устройства</span><span class="sxs-lookup"><span data-stu-id="70104-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="70104-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="70104-136">wipeIssued</span></span>|<span data-ttu-id="70104-137">8</span><span class="sxs-lookup"><span data-stu-id="70104-137">8</span></span>|<span data-ttu-id="70104-138">Команда очистки был отправлен для устройства</span><span class="sxs-lookup"><span data-stu-id="70104-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="70104-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="70104-139">wipeCanceled</span></span>|<span data-ttu-id="70104-140">9</span><span class="sxs-lookup"><span data-stu-id="70104-140">9</span></span>|<span data-ttu-id="70104-141">Команда очистки для этого устройства была отменена</span><span class="sxs-lookup"><span data-stu-id="70104-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="70104-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="70104-142">retireCanceled</span></span>|<span data-ttu-id="70104-143">10</span><span class="sxs-lookup"><span data-stu-id="70104-143">10</span></span>|<span data-ttu-id="70104-144">Команда retire для этого устройства была отменена</span><span class="sxs-lookup"><span data-stu-id="70104-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="70104-145">Обнаружен</span><span class="sxs-lookup"><span data-stu-id="70104-145">discovered</span></span>|<span data-ttu-id="70104-146">11</span><span class="sxs-lookup"><span data-stu-id="70104-146">11</span></span>|<span data-ttu-id="70104-147">Устройство обнаружен, но не полностью зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="70104-147">The device is discovered but not fully enrolled.</span></span>|




