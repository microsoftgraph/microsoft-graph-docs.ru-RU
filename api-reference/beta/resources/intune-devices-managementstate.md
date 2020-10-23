---
title: тип перечисления Манажементстате
description: Состояние управления для устройства в Microsoft Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0ce5fc93bfd48d4beaccac1552573c228f1e6f09
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725444"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="c7214-103">тип перечисления Манажементстате</span><span class="sxs-lookup"><span data-stu-id="c7214-103">managementState enum type</span></span>

<span data-ttu-id="c7214-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7214-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7214-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7214-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7214-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7214-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7214-107">Состояние управления для устройства в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="c7214-107">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="c7214-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c7214-108">Members</span></span>
|<span data-ttu-id="c7214-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c7214-109">Member</span></span>|<span data-ttu-id="c7214-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c7214-110">Value</span></span>|<span data-ttu-id="c7214-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c7214-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7214-112">которыми</span><span class="sxs-lookup"><span data-stu-id="c7214-112">managed</span></span>|<span data-ttu-id="c7214-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c7214-113">0</span></span>|<span data-ttu-id="c7214-114">Устройство находится в управлении</span><span class="sxs-lookup"><span data-stu-id="c7214-114">The device is under management</span></span>|
|<span data-ttu-id="c7214-115">ретирепендинг</span><span class="sxs-lookup"><span data-stu-id="c7214-115">retirePending</span></span>|<span data-ttu-id="c7214-116">1,1</span><span class="sxs-lookup"><span data-stu-id="c7214-116">1</span></span>|<span data-ttu-id="c7214-117">Команда снятия с учета выполняется на устройстве и в процессе отмены регистрации из управления</span><span class="sxs-lookup"><span data-stu-id="c7214-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="c7214-118">ретирефаилед</span><span class="sxs-lookup"><span data-stu-id="c7214-118">retireFailed</span></span>|<span data-ttu-id="c7214-119">2</span><span class="sxs-lookup"><span data-stu-id="c7214-119">2</span></span>|<span data-ttu-id="c7214-120">На устройстве не удалось выполнить команду снятия с учета</span><span class="sxs-lookup"><span data-stu-id="c7214-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="c7214-121">випепендинг</span><span class="sxs-lookup"><span data-stu-id="c7214-121">wipePending</span></span>|<span data-ttu-id="c7214-122">4</span><span class="sxs-lookup"><span data-stu-id="c7214-122">3</span></span>|<span data-ttu-id="c7214-123">На устройстве и в процессе отмены регистрации в управлении возникает команда очистки.</span><span class="sxs-lookup"><span data-stu-id="c7214-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="c7214-124">випефаилед</span><span class="sxs-lookup"><span data-stu-id="c7214-124">wipeFailed</span></span>|<span data-ttu-id="c7214-125">4 </span><span class="sxs-lookup"><span data-stu-id="c7214-125">4</span></span>|<span data-ttu-id="c7214-126">Не удалось выполнить команду очистки на устройстве</span><span class="sxs-lookup"><span data-stu-id="c7214-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="c7214-127">неисправности</span><span class="sxs-lookup"><span data-stu-id="c7214-127">unhealthy</span></span>|<span data-ttu-id="c7214-128">5 </span><span class="sxs-lookup"><span data-stu-id="c7214-128">5</span></span>|<span data-ttu-id="c7214-129">Устройство неработоспособно.</span><span class="sxs-lookup"><span data-stu-id="c7214-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="c7214-130">делетепендинг</span><span class="sxs-lookup"><span data-stu-id="c7214-130">deletePending</span></span>|<span data-ttu-id="c7214-131">6 </span><span class="sxs-lookup"><span data-stu-id="c7214-131">6</span></span>|<span data-ttu-id="c7214-132">На устройстве выполняется команда Delete</span><span class="sxs-lookup"><span data-stu-id="c7214-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="c7214-133">ретиреиссуед</span><span class="sxs-lookup"><span data-stu-id="c7214-133">retireIssued</span></span>|<span data-ttu-id="c7214-134">7 </span><span class="sxs-lookup"><span data-stu-id="c7214-134">7</span></span>|<span data-ttu-id="c7214-135">Для устройства была выпущена команда снятия с учета</span><span class="sxs-lookup"><span data-stu-id="c7214-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="c7214-136">випеиссуед</span><span class="sxs-lookup"><span data-stu-id="c7214-136">wipeIssued</span></span>|<span data-ttu-id="c7214-137">8 </span><span class="sxs-lookup"><span data-stu-id="c7214-137">8</span></span>|<span data-ttu-id="c7214-138">Для устройства была выдана команда очистки.</span><span class="sxs-lookup"><span data-stu-id="c7214-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="c7214-139">випеканцелед</span><span class="sxs-lookup"><span data-stu-id="c7214-139">wipeCanceled</span></span>|<span data-ttu-id="c7214-140">9 </span><span class="sxs-lookup"><span data-stu-id="c7214-140">9</span></span>|<span data-ttu-id="c7214-141">Команда стирания для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="c7214-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="c7214-142">ретиреканцелед</span><span class="sxs-lookup"><span data-stu-id="c7214-142">retireCanceled</span></span>|<span data-ttu-id="c7214-143">10 </span><span class="sxs-lookup"><span data-stu-id="c7214-143">10</span></span>|<span data-ttu-id="c7214-144">Команда снятия с учета для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="c7214-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="c7214-145">были</span><span class="sxs-lookup"><span data-stu-id="c7214-145">discovered</span></span>|<span data-ttu-id="c7214-146">-11:00</span><span class="sxs-lookup"><span data-stu-id="c7214-146">11</span></span>|<span data-ttu-id="c7214-147">Устройство обнаружено, но не зарегистрировано полностью.</span><span class="sxs-lookup"><span data-stu-id="c7214-147">The device is discovered but not fully enrolled.</span></span>|





