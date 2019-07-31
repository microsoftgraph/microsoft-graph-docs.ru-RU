---
title: тип перечисления Манажементстате
description: Состояние управления для устройства в Microsoft Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 928f2c1c9e7eb1530bdf7839691cf2469af11077
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968339"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="e205a-103">тип перечисления Манажементстате</span><span class="sxs-lookup"><span data-stu-id="e205a-103">managementState enum type</span></span>

> <span data-ttu-id="e205a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e205a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e205a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e205a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e205a-106">Состояние управления для устройства в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="e205a-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="e205a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e205a-107">Members</span></span>
|<span data-ttu-id="e205a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e205a-108">Member</span></span>|<span data-ttu-id="e205a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e205a-109">Value</span></span>|<span data-ttu-id="e205a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e205a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e205a-111">которыми</span><span class="sxs-lookup"><span data-stu-id="e205a-111">managed</span></span>|<span data-ttu-id="e205a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e205a-112">0</span></span>|<span data-ttu-id="e205a-113">Устройство находится в управлении</span><span class="sxs-lookup"><span data-stu-id="e205a-113">The device is under management</span></span>|
|<span data-ttu-id="e205a-114">Ретирепендинг</span><span class="sxs-lookup"><span data-stu-id="e205a-114">retirePending</span></span>|<span data-ttu-id="e205a-115">1,1</span><span class="sxs-lookup"><span data-stu-id="e205a-115">1</span></span>|<span data-ttu-id="e205a-116">Команда снятия с учета выполняется на устройстве и в процессе отмены регистрации из управления</span><span class="sxs-lookup"><span data-stu-id="e205a-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="e205a-117">Ретирефаилед</span><span class="sxs-lookup"><span data-stu-id="e205a-117">retireFailed</span></span>|<span data-ttu-id="e205a-118">2</span><span class="sxs-lookup"><span data-stu-id="e205a-118">2</span></span>|<span data-ttu-id="e205a-119">На устройстве не удалось выполнить команду снятия с учета</span><span class="sxs-lookup"><span data-stu-id="e205a-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="e205a-120">Випепендинг</span><span class="sxs-lookup"><span data-stu-id="e205a-120">wipePending</span></span>|<span data-ttu-id="e205a-121">4</span><span class="sxs-lookup"><span data-stu-id="e205a-121">3</span></span>|<span data-ttu-id="e205a-122">На устройстве и в процессе отмены регистрации в управлении возникает команда очистки.</span><span class="sxs-lookup"><span data-stu-id="e205a-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="e205a-123">Випефаилед</span><span class="sxs-lookup"><span data-stu-id="e205a-123">wipeFailed</span></span>|<span data-ttu-id="e205a-124">SP4</span><span class="sxs-lookup"><span data-stu-id="e205a-124">4</span></span>|<span data-ttu-id="e205a-125">Не удалось выполнить команду очистки на устройстве</span><span class="sxs-lookup"><span data-stu-id="e205a-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="e205a-126">неисправности</span><span class="sxs-lookup"><span data-stu-id="e205a-126">unhealthy</span></span>|<span data-ttu-id="e205a-127">17:00</span><span class="sxs-lookup"><span data-stu-id="e205a-127">5</span></span>|<span data-ttu-id="e205a-128">Устройство неработоспособно.</span><span class="sxs-lookup"><span data-stu-id="e205a-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="e205a-129">Делетепендинг</span><span class="sxs-lookup"><span data-stu-id="e205a-129">deletePending</span></span>|<span data-ttu-id="e205a-130">6 </span><span class="sxs-lookup"><span data-stu-id="e205a-130">6</span></span>|<span data-ttu-id="e205a-131">На устройстве выполняется команда Delete</span><span class="sxs-lookup"><span data-stu-id="e205a-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="e205a-132">Ретиреиссуед</span><span class="sxs-lookup"><span data-stu-id="e205a-132">retireIssued</span></span>|<span data-ttu-id="e205a-133">7 </span><span class="sxs-lookup"><span data-stu-id="e205a-133">7</span></span>|<span data-ttu-id="e205a-134">Для устройства была выпущена команда снятия с учета</span><span class="sxs-lookup"><span data-stu-id="e205a-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="e205a-135">Випеиссуед</span><span class="sxs-lookup"><span data-stu-id="e205a-135">wipeIssued</span></span>|<span data-ttu-id="e205a-136">8 </span><span class="sxs-lookup"><span data-stu-id="e205a-136">8</span></span>|<span data-ttu-id="e205a-137">Для устройства была выдана команда очистки.</span><span class="sxs-lookup"><span data-stu-id="e205a-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="e205a-138">Випеканцелед</span><span class="sxs-lookup"><span data-stu-id="e205a-138">wipeCanceled</span></span>|<span data-ttu-id="e205a-139">9 </span><span class="sxs-lookup"><span data-stu-id="e205a-139">9</span></span>|<span data-ttu-id="e205a-140">Команда стирания для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="e205a-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="e205a-141">Ретиреканцелед</span><span class="sxs-lookup"><span data-stu-id="e205a-141">retireCanceled</span></span>|<span data-ttu-id="e205a-142">10 </span><span class="sxs-lookup"><span data-stu-id="e205a-142">10</span></span>|<span data-ttu-id="e205a-143">Команда снятия с учета для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="e205a-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="e205a-144">были</span><span class="sxs-lookup"><span data-stu-id="e205a-144">discovered</span></span>|<span data-ttu-id="e205a-145">-11:00</span><span class="sxs-lookup"><span data-stu-id="e205a-145">11</span></span>|<span data-ttu-id="e205a-146">Устройство обнаружено, но не зарегистрировано полностью.</span><span class="sxs-lookup"><span data-stu-id="e205a-146">The device is discovered but not fully enrolled.</span></span>|





