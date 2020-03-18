---
title: тип перечисления Манажементстате
description: Состояние управления для устройства в Microsoft Intune.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fd0a4616f6f35c91ae6ce6269d452a00d3275bc5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783930"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="bdcfa-103">тип перечисления Манажементстате</span><span class="sxs-lookup"><span data-stu-id="bdcfa-103">managementState enum type</span></span>

> <span data-ttu-id="bdcfa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdcfa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdcfa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bdcfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdcfa-106">Состояние управления для устройства в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="bdcfa-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="bdcfa-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bdcfa-107">Members</span></span>
|<span data-ttu-id="bdcfa-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bdcfa-108">Member</span></span>|<span data-ttu-id="bdcfa-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bdcfa-109">Value</span></span>|<span data-ttu-id="bdcfa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bdcfa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdcfa-111">которыми</span><span class="sxs-lookup"><span data-stu-id="bdcfa-111">managed</span></span>|<span data-ttu-id="bdcfa-112">нуль</span><span class="sxs-lookup"><span data-stu-id="bdcfa-112">0</span></span>|<span data-ttu-id="bdcfa-113">Устройство находится в управлении</span><span class="sxs-lookup"><span data-stu-id="bdcfa-113">The device is under management</span></span>|
|<span data-ttu-id="bdcfa-114">ретирепендинг</span><span class="sxs-lookup"><span data-stu-id="bdcfa-114">retirePending</span></span>|<span data-ttu-id="bdcfa-115">1,1</span><span class="sxs-lookup"><span data-stu-id="bdcfa-115">1</span></span>|<span data-ttu-id="bdcfa-116">Команда снятия с учета выполняется на устройстве и в процессе отмены регистрации из управления</span><span class="sxs-lookup"><span data-stu-id="bdcfa-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="bdcfa-117">ретирефаилед</span><span class="sxs-lookup"><span data-stu-id="bdcfa-117">retireFailed</span></span>|<span data-ttu-id="bdcfa-118">2</span><span class="sxs-lookup"><span data-stu-id="bdcfa-118">2</span></span>|<span data-ttu-id="bdcfa-119">На устройстве не удалось выполнить команду снятия с учета</span><span class="sxs-lookup"><span data-stu-id="bdcfa-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="bdcfa-120">випепендинг</span><span class="sxs-lookup"><span data-stu-id="bdcfa-120">wipePending</span></span>|<span data-ttu-id="bdcfa-121">4</span><span class="sxs-lookup"><span data-stu-id="bdcfa-121">3</span></span>|<span data-ttu-id="bdcfa-122">На устройстве и в процессе отмены регистрации в управлении возникает команда очистки.</span><span class="sxs-lookup"><span data-stu-id="bdcfa-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="bdcfa-123">випефаилед</span><span class="sxs-lookup"><span data-stu-id="bdcfa-123">wipeFailed</span></span>|<span data-ttu-id="bdcfa-124">4 </span><span class="sxs-lookup"><span data-stu-id="bdcfa-124">4</span></span>|<span data-ttu-id="bdcfa-125">Не удалось выполнить команду очистки на устройстве</span><span class="sxs-lookup"><span data-stu-id="bdcfa-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="bdcfa-126">неисправности</span><span class="sxs-lookup"><span data-stu-id="bdcfa-126">unhealthy</span></span>|<span data-ttu-id="bdcfa-127">5 </span><span class="sxs-lookup"><span data-stu-id="bdcfa-127">5</span></span>|<span data-ttu-id="bdcfa-128">Устройство неработоспособно.</span><span class="sxs-lookup"><span data-stu-id="bdcfa-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="bdcfa-129">делетепендинг</span><span class="sxs-lookup"><span data-stu-id="bdcfa-129">deletePending</span></span>|<span data-ttu-id="bdcfa-130">6 </span><span class="sxs-lookup"><span data-stu-id="bdcfa-130">6</span></span>|<span data-ttu-id="bdcfa-131">На устройстве выполняется команда Delete</span><span class="sxs-lookup"><span data-stu-id="bdcfa-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="bdcfa-132">ретиреиссуед</span><span class="sxs-lookup"><span data-stu-id="bdcfa-132">retireIssued</span></span>|<span data-ttu-id="bdcfa-133">7 </span><span class="sxs-lookup"><span data-stu-id="bdcfa-133">7</span></span>|<span data-ttu-id="bdcfa-134">Для устройства была выпущена команда снятия с учета</span><span class="sxs-lookup"><span data-stu-id="bdcfa-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="bdcfa-135">випеиссуед</span><span class="sxs-lookup"><span data-stu-id="bdcfa-135">wipeIssued</span></span>|<span data-ttu-id="bdcfa-136">8 </span><span class="sxs-lookup"><span data-stu-id="bdcfa-136">8</span></span>|<span data-ttu-id="bdcfa-137">Для устройства была выдана команда очистки.</span><span class="sxs-lookup"><span data-stu-id="bdcfa-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="bdcfa-138">випеканцелед</span><span class="sxs-lookup"><span data-stu-id="bdcfa-138">wipeCanceled</span></span>|<span data-ttu-id="bdcfa-139">9 </span><span class="sxs-lookup"><span data-stu-id="bdcfa-139">9</span></span>|<span data-ttu-id="bdcfa-140">Команда стирания для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="bdcfa-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="bdcfa-141">ретиреканцелед</span><span class="sxs-lookup"><span data-stu-id="bdcfa-141">retireCanceled</span></span>|<span data-ttu-id="bdcfa-142">10 </span><span class="sxs-lookup"><span data-stu-id="bdcfa-142">10</span></span>|<span data-ttu-id="bdcfa-143">Команда снятия с учета для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="bdcfa-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="bdcfa-144">были</span><span class="sxs-lookup"><span data-stu-id="bdcfa-144">discovered</span></span>|<span data-ttu-id="bdcfa-145">-11:00</span><span class="sxs-lookup"><span data-stu-id="bdcfa-145">11</span></span>|<span data-ttu-id="bdcfa-146">Устройство обнаружено, но не зарегистрировано полностью.</span><span class="sxs-lookup"><span data-stu-id="bdcfa-146">The device is discovered but not fully enrolled.</span></span>|



