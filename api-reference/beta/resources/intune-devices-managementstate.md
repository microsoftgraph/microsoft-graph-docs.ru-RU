---
title: тип перечисления Манажементстате
description: Состояние управления для устройства в Microsoft Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05dc0db1ecbe88616ca36db82bad2081b4133e3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521294"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="f8520-103">тип перечисления Манажементстате</span><span class="sxs-lookup"><span data-stu-id="f8520-103">managementState enum type</span></span>

> <span data-ttu-id="f8520-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8520-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8520-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8520-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8520-106">Состояние управления для устройства в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="f8520-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="f8520-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f8520-107">Members</span></span>
|<span data-ttu-id="f8520-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f8520-108">Member</span></span>|<span data-ttu-id="f8520-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f8520-109">Value</span></span>|<span data-ttu-id="f8520-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f8520-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8520-111">которыми</span><span class="sxs-lookup"><span data-stu-id="f8520-111">managed</span></span>|<span data-ttu-id="f8520-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f8520-112">0</span></span>|<span data-ttu-id="f8520-113">Устройство находится в управлении</span><span class="sxs-lookup"><span data-stu-id="f8520-113">The device is under management</span></span>|
|<span data-ttu-id="f8520-114">Ретирепендинг</span><span class="sxs-lookup"><span data-stu-id="f8520-114">retirePending</span></span>|<span data-ttu-id="f8520-115">1 </span><span class="sxs-lookup"><span data-stu-id="f8520-115">1</span></span>|<span data-ttu-id="f8520-116">Команда снятия с учета выполняется на устройстве и в процессе отмены регистрации из управления</span><span class="sxs-lookup"><span data-stu-id="f8520-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="f8520-117">Ретирефаилед</span><span class="sxs-lookup"><span data-stu-id="f8520-117">retireFailed</span></span>|<span data-ttu-id="f8520-118">2 </span><span class="sxs-lookup"><span data-stu-id="f8520-118">2</span></span>|<span data-ttu-id="f8520-119">На устройстве не удалось выполнить команду снятия с учета</span><span class="sxs-lookup"><span data-stu-id="f8520-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="f8520-120">Випепендинг</span><span class="sxs-lookup"><span data-stu-id="f8520-120">wipePending</span></span>|<span data-ttu-id="f8520-121">3 </span><span class="sxs-lookup"><span data-stu-id="f8520-121">3</span></span>|<span data-ttu-id="f8520-122">На устройстве и в процессе отмены регистрации в управлении возникает команда очистки.</span><span class="sxs-lookup"><span data-stu-id="f8520-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="f8520-123">Випефаилед</span><span class="sxs-lookup"><span data-stu-id="f8520-123">wipeFailed</span></span>|<span data-ttu-id="f8520-124">4 </span><span class="sxs-lookup"><span data-stu-id="f8520-124">4</span></span>|<span data-ttu-id="f8520-125">Не удалось выполнить команду очистки на устройстве</span><span class="sxs-lookup"><span data-stu-id="f8520-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="f8520-126">неисправности</span><span class="sxs-lookup"><span data-stu-id="f8520-126">unhealthy</span></span>|<span data-ttu-id="f8520-127">5 </span><span class="sxs-lookup"><span data-stu-id="f8520-127">5</span></span>|<span data-ttu-id="f8520-128">Устройство неработоспособно.</span><span class="sxs-lookup"><span data-stu-id="f8520-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="f8520-129">Делетепендинг</span><span class="sxs-lookup"><span data-stu-id="f8520-129">deletePending</span></span>|<span data-ttu-id="f8520-130">6 </span><span class="sxs-lookup"><span data-stu-id="f8520-130">6</span></span>|<span data-ttu-id="f8520-131">На устройстве выполняется команда Delete</span><span class="sxs-lookup"><span data-stu-id="f8520-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="f8520-132">Ретиреиссуед</span><span class="sxs-lookup"><span data-stu-id="f8520-132">retireIssued</span></span>|<span data-ttu-id="f8520-133">7 </span><span class="sxs-lookup"><span data-stu-id="f8520-133">7</span></span>|<span data-ttu-id="f8520-134">Для устройства была выпущена команда снятия С учета</span><span class="sxs-lookup"><span data-stu-id="f8520-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="f8520-135">Випеиссуед</span><span class="sxs-lookup"><span data-stu-id="f8520-135">wipeIssued</span></span>|<span data-ttu-id="f8520-136">8 </span><span class="sxs-lookup"><span data-stu-id="f8520-136">8</span></span>|<span data-ttu-id="f8520-137">Для устройства была выдана команда очистки.</span><span class="sxs-lookup"><span data-stu-id="f8520-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="f8520-138">Випеканцелед</span><span class="sxs-lookup"><span data-stu-id="f8520-138">wipeCanceled</span></span>|<span data-ttu-id="f8520-139">9 </span><span class="sxs-lookup"><span data-stu-id="f8520-139">9</span></span>|<span data-ttu-id="f8520-140">Команда стирания для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="f8520-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="f8520-141">Ретиреканцелед</span><span class="sxs-lookup"><span data-stu-id="f8520-141">retireCanceled</span></span>|<span data-ttu-id="f8520-142">10 </span><span class="sxs-lookup"><span data-stu-id="f8520-142">10</span></span>|<span data-ttu-id="f8520-143">Команда снятия С учета для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="f8520-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="f8520-144">были</span><span class="sxs-lookup"><span data-stu-id="f8520-144">discovered</span></span>|<span data-ttu-id="f8520-145">11 </span><span class="sxs-lookup"><span data-stu-id="f8520-145">11</span></span>|<span data-ttu-id="f8520-146">Устройство обнаружено, но не зарегистрировано полностью.</span><span class="sxs-lookup"><span data-stu-id="f8520-146">The device is discovered but not fully enrolled.</span></span>|





