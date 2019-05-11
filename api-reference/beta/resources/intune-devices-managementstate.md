---
title: тип перечисления Манажементстате
description: Состояние управления для устройства в Microsoft Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ceb46d11042c0e6d879bf0708a5f64807ce5fe3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941875"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="0f351-103">тип перечисления Манажементстате</span><span class="sxs-lookup"><span data-stu-id="0f351-103">managementState enum type</span></span>

> <span data-ttu-id="0f351-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f351-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f351-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f351-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f351-106">Состояние управления для устройства в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="0f351-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="0f351-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="0f351-107">Members</span></span>
|<span data-ttu-id="0f351-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="0f351-108">Member</span></span>|<span data-ttu-id="0f351-109">Значение</span><span class="sxs-lookup"><span data-stu-id="0f351-109">Value</span></span>|<span data-ttu-id="0f351-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0f351-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f351-111">которыми</span><span class="sxs-lookup"><span data-stu-id="0f351-111">managed</span></span>|<span data-ttu-id="0f351-112">нуль</span><span class="sxs-lookup"><span data-stu-id="0f351-112">0</span></span>|<span data-ttu-id="0f351-113">Устройство находится в управлении</span><span class="sxs-lookup"><span data-stu-id="0f351-113">The device is under management</span></span>|
|<span data-ttu-id="0f351-114">Ретирепендинг</span><span class="sxs-lookup"><span data-stu-id="0f351-114">retirePending</span></span>|<span data-ttu-id="0f351-115">1,1</span><span class="sxs-lookup"><span data-stu-id="0f351-115">1</span></span>|<span data-ttu-id="0f351-116">Команда снятия с учета выполняется на устройстве и в процессе отмены регистрации из управления</span><span class="sxs-lookup"><span data-stu-id="0f351-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="0f351-117">Ретирефаилед</span><span class="sxs-lookup"><span data-stu-id="0f351-117">retireFailed</span></span>|<span data-ttu-id="0f351-118">2</span><span class="sxs-lookup"><span data-stu-id="0f351-118">2</span></span>|<span data-ttu-id="0f351-119">На устройстве не удалось выполнить команду снятия с учета</span><span class="sxs-lookup"><span data-stu-id="0f351-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="0f351-120">Випепендинг</span><span class="sxs-lookup"><span data-stu-id="0f351-120">wipePending</span></span>|<span data-ttu-id="0f351-121">4</span><span class="sxs-lookup"><span data-stu-id="0f351-121">3</span></span>|<span data-ttu-id="0f351-122">На устройстве и в процессе отмены регистрации в управлении возникает команда очистки.</span><span class="sxs-lookup"><span data-stu-id="0f351-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="0f351-123">Випефаилед</span><span class="sxs-lookup"><span data-stu-id="0f351-123">wipeFailed</span></span>|<span data-ttu-id="0f351-124">SP4</span><span class="sxs-lookup"><span data-stu-id="0f351-124">4</span></span>|<span data-ttu-id="0f351-125">Не удалось выполнить команду очистки на устройстве</span><span class="sxs-lookup"><span data-stu-id="0f351-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="0f351-126">неисправности</span><span class="sxs-lookup"><span data-stu-id="0f351-126">unhealthy</span></span>|<span data-ttu-id="0f351-127">17:00</span><span class="sxs-lookup"><span data-stu-id="0f351-127">5</span></span>|<span data-ttu-id="0f351-128">Устройство неработоспособно.</span><span class="sxs-lookup"><span data-stu-id="0f351-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="0f351-129">Делетепендинг</span><span class="sxs-lookup"><span data-stu-id="0f351-129">deletePending</span></span>|<span data-ttu-id="0f351-130">6 </span><span class="sxs-lookup"><span data-stu-id="0f351-130">6</span></span>|<span data-ttu-id="0f351-131">На устройстве выполняется команда Delete</span><span class="sxs-lookup"><span data-stu-id="0f351-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="0f351-132">Ретиреиссуед</span><span class="sxs-lookup"><span data-stu-id="0f351-132">retireIssued</span></span>|<span data-ttu-id="0f351-133">7 </span><span class="sxs-lookup"><span data-stu-id="0f351-133">7</span></span>|<span data-ttu-id="0f351-134">Для устройства была выпущена команда снятия С учета</span><span class="sxs-lookup"><span data-stu-id="0f351-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="0f351-135">Випеиссуед</span><span class="sxs-lookup"><span data-stu-id="0f351-135">wipeIssued</span></span>|<span data-ttu-id="0f351-136">8 </span><span class="sxs-lookup"><span data-stu-id="0f351-136">8</span></span>|<span data-ttu-id="0f351-137">Для устройства была выдана команда очистки.</span><span class="sxs-lookup"><span data-stu-id="0f351-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="0f351-138">Випеканцелед</span><span class="sxs-lookup"><span data-stu-id="0f351-138">wipeCanceled</span></span>|<span data-ttu-id="0f351-139">9 </span><span class="sxs-lookup"><span data-stu-id="0f351-139">9</span></span>|<span data-ttu-id="0f351-140">Команда стирания для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="0f351-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="0f351-141">Ретиреканцелед</span><span class="sxs-lookup"><span data-stu-id="0f351-141">retireCanceled</span></span>|<span data-ttu-id="0f351-142">10 </span><span class="sxs-lookup"><span data-stu-id="0f351-142">10</span></span>|<span data-ttu-id="0f351-143">Команда снятия С учета для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="0f351-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="0f351-144">были</span><span class="sxs-lookup"><span data-stu-id="0f351-144">discovered</span></span>|<span data-ttu-id="0f351-145">-11:00</span><span class="sxs-lookup"><span data-stu-id="0f351-145">11</span></span>|<span data-ttu-id="0f351-146">Устройство обнаружено, но не зарегистрировано полностью.</span><span class="sxs-lookup"><span data-stu-id="0f351-146">The device is discovered but not fully enrolled.</span></span>|




