---
title: тип перечисления Манажементстате
description: Состояние управления для устройства в Microsoft Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 316e4d2ce97311e1a45f3324f2636054afd62664
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963935"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="de413-103">тип перечисления Манажементстате</span><span class="sxs-lookup"><span data-stu-id="de413-103">managementState enum type</span></span>

> <span data-ttu-id="de413-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de413-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de413-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de413-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de413-106">Состояние управления для устройства в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="de413-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="de413-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="de413-107">Members</span></span>
|<span data-ttu-id="de413-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="de413-108">Member</span></span>|<span data-ttu-id="de413-109">Значение</span><span class="sxs-lookup"><span data-stu-id="de413-109">Value</span></span>|<span data-ttu-id="de413-110">Описание</span><span class="sxs-lookup"><span data-stu-id="de413-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de413-111">которыми</span><span class="sxs-lookup"><span data-stu-id="de413-111">managed</span></span>|<span data-ttu-id="de413-112">нуль</span><span class="sxs-lookup"><span data-stu-id="de413-112">0</span></span>|<span data-ttu-id="de413-113">Устройство находится в управлении</span><span class="sxs-lookup"><span data-stu-id="de413-113">The device is under management</span></span>|
|<span data-ttu-id="de413-114">Ретирепендинг</span><span class="sxs-lookup"><span data-stu-id="de413-114">retirePending</span></span>|<span data-ttu-id="de413-115">1,1</span><span class="sxs-lookup"><span data-stu-id="de413-115">1</span></span>|<span data-ttu-id="de413-116">Команда снятия с учета выполняется на устройстве и в процессе отмены регистрации из управления</span><span class="sxs-lookup"><span data-stu-id="de413-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="de413-117">Ретирефаилед</span><span class="sxs-lookup"><span data-stu-id="de413-117">retireFailed</span></span>|<span data-ttu-id="de413-118">2</span><span class="sxs-lookup"><span data-stu-id="de413-118">2</span></span>|<span data-ttu-id="de413-119">На устройстве не удалось выполнить команду снятия с учета</span><span class="sxs-lookup"><span data-stu-id="de413-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="de413-120">Випепендинг</span><span class="sxs-lookup"><span data-stu-id="de413-120">wipePending</span></span>|<span data-ttu-id="de413-121">4</span><span class="sxs-lookup"><span data-stu-id="de413-121">3</span></span>|<span data-ttu-id="de413-122">На устройстве и в процессе отмены регистрации в управлении возникает команда очистки.</span><span class="sxs-lookup"><span data-stu-id="de413-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="de413-123">Випефаилед</span><span class="sxs-lookup"><span data-stu-id="de413-123">wipeFailed</span></span>|<span data-ttu-id="de413-124">SP4</span><span class="sxs-lookup"><span data-stu-id="de413-124">4</span></span>|<span data-ttu-id="de413-125">Не удалось выполнить команду очистки на устройстве</span><span class="sxs-lookup"><span data-stu-id="de413-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="de413-126">неисправности</span><span class="sxs-lookup"><span data-stu-id="de413-126">unhealthy</span></span>|<span data-ttu-id="de413-127">17:00</span><span class="sxs-lookup"><span data-stu-id="de413-127">5</span></span>|<span data-ttu-id="de413-128">Устройство неработоспособно.</span><span class="sxs-lookup"><span data-stu-id="de413-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="de413-129">Делетепендинг</span><span class="sxs-lookup"><span data-stu-id="de413-129">deletePending</span></span>|<span data-ttu-id="de413-130">6 </span><span class="sxs-lookup"><span data-stu-id="de413-130">6</span></span>|<span data-ttu-id="de413-131">На устройстве выполняется команда Delete</span><span class="sxs-lookup"><span data-stu-id="de413-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="de413-132">Ретиреиссуед</span><span class="sxs-lookup"><span data-stu-id="de413-132">retireIssued</span></span>|<span data-ttu-id="de413-133">7 </span><span class="sxs-lookup"><span data-stu-id="de413-133">7</span></span>|<span data-ttu-id="de413-134">Для устройства была выпущена команда снятия с учета</span><span class="sxs-lookup"><span data-stu-id="de413-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="de413-135">Випеиссуед</span><span class="sxs-lookup"><span data-stu-id="de413-135">wipeIssued</span></span>|<span data-ttu-id="de413-136">8 </span><span class="sxs-lookup"><span data-stu-id="de413-136">8</span></span>|<span data-ttu-id="de413-137">Для устройства была выдана команда очистки.</span><span class="sxs-lookup"><span data-stu-id="de413-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="de413-138">Випеканцелед</span><span class="sxs-lookup"><span data-stu-id="de413-138">wipeCanceled</span></span>|<span data-ttu-id="de413-139">9 </span><span class="sxs-lookup"><span data-stu-id="de413-139">9</span></span>|<span data-ttu-id="de413-140">Команда стирания для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="de413-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="de413-141">Ретиреканцелед</span><span class="sxs-lookup"><span data-stu-id="de413-141">retireCanceled</span></span>|<span data-ttu-id="de413-142">10 </span><span class="sxs-lookup"><span data-stu-id="de413-142">10</span></span>|<span data-ttu-id="de413-143">Команда снятия с учета для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="de413-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="de413-144">были</span><span class="sxs-lookup"><span data-stu-id="de413-144">discovered</span></span>|<span data-ttu-id="de413-145">-11:00</span><span class="sxs-lookup"><span data-stu-id="de413-145">11</span></span>|<span data-ttu-id="de413-146">Устройство обнаружено, но не зарегистрировано полностью.</span><span class="sxs-lookup"><span data-stu-id="de413-146">The device is discovered but not fully enrolled.</span></span>|





