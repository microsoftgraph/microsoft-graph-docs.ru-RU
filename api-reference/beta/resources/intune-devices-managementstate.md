---
title: тип перечисления Манажементстате
description: Состояние управления для устройства в Microsoft Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fb41df389eea60d3bebc07e6ce62da3c4a3924b3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49230886"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="89843-103">тип перечисления Манажементстате</span><span class="sxs-lookup"><span data-stu-id="89843-103">managementState enum type</span></span>

<span data-ttu-id="89843-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89843-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89843-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89843-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89843-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89843-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89843-107">Состояние управления для устройства в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="89843-107">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="89843-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="89843-108">Members</span></span>
|<span data-ttu-id="89843-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="89843-109">Member</span></span>|<span data-ttu-id="89843-110">Значение</span><span class="sxs-lookup"><span data-stu-id="89843-110">Value</span></span>|<span data-ttu-id="89843-111">Описание</span><span class="sxs-lookup"><span data-stu-id="89843-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89843-112">которыми</span><span class="sxs-lookup"><span data-stu-id="89843-112">managed</span></span>|<span data-ttu-id="89843-113">нуль</span><span class="sxs-lookup"><span data-stu-id="89843-113">0</span></span>|<span data-ttu-id="89843-114">Устройство находится в управлении</span><span class="sxs-lookup"><span data-stu-id="89843-114">The device is under management</span></span>|
|<span data-ttu-id="89843-115">ретирепендинг</span><span class="sxs-lookup"><span data-stu-id="89843-115">retirePending</span></span>|<span data-ttu-id="89843-116">1,1</span><span class="sxs-lookup"><span data-stu-id="89843-116">1</span></span>|<span data-ttu-id="89843-117">Команда снятия с учета выполняется на устройстве и в процессе отмены регистрации из управления</span><span class="sxs-lookup"><span data-stu-id="89843-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="89843-118">ретирефаилед</span><span class="sxs-lookup"><span data-stu-id="89843-118">retireFailed</span></span>|<span data-ttu-id="89843-119">2</span><span class="sxs-lookup"><span data-stu-id="89843-119">2</span></span>|<span data-ttu-id="89843-120">На устройстве не удалось выполнить команду снятия с учета</span><span class="sxs-lookup"><span data-stu-id="89843-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="89843-121">випепендинг</span><span class="sxs-lookup"><span data-stu-id="89843-121">wipePending</span></span>|<span data-ttu-id="89843-122">4</span><span class="sxs-lookup"><span data-stu-id="89843-122">3</span></span>|<span data-ttu-id="89843-123">На устройстве и в процессе отмены регистрации в управлении возникает команда очистки.</span><span class="sxs-lookup"><span data-stu-id="89843-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="89843-124">випефаилед</span><span class="sxs-lookup"><span data-stu-id="89843-124">wipeFailed</span></span>|<span data-ttu-id="89843-125">4 </span><span class="sxs-lookup"><span data-stu-id="89843-125">4</span></span>|<span data-ttu-id="89843-126">Не удалось выполнить команду очистки на устройстве</span><span class="sxs-lookup"><span data-stu-id="89843-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="89843-127">неисправности</span><span class="sxs-lookup"><span data-stu-id="89843-127">unhealthy</span></span>|<span data-ttu-id="89843-128">5 </span><span class="sxs-lookup"><span data-stu-id="89843-128">5</span></span>|<span data-ttu-id="89843-129">Устройство неработоспособно.</span><span class="sxs-lookup"><span data-stu-id="89843-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="89843-130">делетепендинг</span><span class="sxs-lookup"><span data-stu-id="89843-130">deletePending</span></span>|<span data-ttu-id="89843-131">6 </span><span class="sxs-lookup"><span data-stu-id="89843-131">6</span></span>|<span data-ttu-id="89843-132">На устройстве выполняется команда Delete</span><span class="sxs-lookup"><span data-stu-id="89843-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="89843-133">ретиреиссуед</span><span class="sxs-lookup"><span data-stu-id="89843-133">retireIssued</span></span>|<span data-ttu-id="89843-134">7 </span><span class="sxs-lookup"><span data-stu-id="89843-134">7</span></span>|<span data-ttu-id="89843-135">Для устройства была выпущена команда снятия с учета</span><span class="sxs-lookup"><span data-stu-id="89843-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="89843-136">випеиссуед</span><span class="sxs-lookup"><span data-stu-id="89843-136">wipeIssued</span></span>|<span data-ttu-id="89843-137">8 </span><span class="sxs-lookup"><span data-stu-id="89843-137">8</span></span>|<span data-ttu-id="89843-138">Для устройства была выдана команда очистки.</span><span class="sxs-lookup"><span data-stu-id="89843-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="89843-139">випеканцелед</span><span class="sxs-lookup"><span data-stu-id="89843-139">wipeCanceled</span></span>|<span data-ttu-id="89843-140">9 </span><span class="sxs-lookup"><span data-stu-id="89843-140">9</span></span>|<span data-ttu-id="89843-141">Команда стирания для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="89843-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="89843-142">ретиреканцелед</span><span class="sxs-lookup"><span data-stu-id="89843-142">retireCanceled</span></span>|<span data-ttu-id="89843-143">10 </span><span class="sxs-lookup"><span data-stu-id="89843-143">10</span></span>|<span data-ttu-id="89843-144">Команда снятия с учета для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="89843-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="89843-145">были</span><span class="sxs-lookup"><span data-stu-id="89843-145">discovered</span></span>|<span data-ttu-id="89843-146">11 </span><span class="sxs-lookup"><span data-stu-id="89843-146">11</span></span>|<span data-ttu-id="89843-147">Устройство обнаружено, но не зарегистрировано полностью.</span><span class="sxs-lookup"><span data-stu-id="89843-147">The device is discovered but not fully enrolled.</span></span>|




