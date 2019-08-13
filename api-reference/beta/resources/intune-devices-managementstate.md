---
title: тип перечисления Манажементстате
description: Состояние управления для устройства в Microsoft Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a61b9d228589f1d0a1e380ed45720f66faa650af
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372155"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="652b2-103">тип перечисления Манажементстате</span><span class="sxs-lookup"><span data-stu-id="652b2-103">managementState enum type</span></span>

> <span data-ttu-id="652b2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="652b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="652b2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="652b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="652b2-106">Состояние управления для устройства в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="652b2-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="652b2-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="652b2-107">Members</span></span>
|<span data-ttu-id="652b2-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="652b2-108">Member</span></span>|<span data-ttu-id="652b2-109">Значение</span><span class="sxs-lookup"><span data-stu-id="652b2-109">Value</span></span>|<span data-ttu-id="652b2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="652b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="652b2-111">которыми</span><span class="sxs-lookup"><span data-stu-id="652b2-111">managed</span></span>|<span data-ttu-id="652b2-112">нуль</span><span class="sxs-lookup"><span data-stu-id="652b2-112">0</span></span>|<span data-ttu-id="652b2-113">Устройство находится в управлении</span><span class="sxs-lookup"><span data-stu-id="652b2-113">The device is under management</span></span>|
|<span data-ttu-id="652b2-114">ретирепендинг</span><span class="sxs-lookup"><span data-stu-id="652b2-114">retirePending</span></span>|<span data-ttu-id="652b2-115">1,1</span><span class="sxs-lookup"><span data-stu-id="652b2-115">1</span></span>|<span data-ttu-id="652b2-116">Команда снятия с учета выполняется на устройстве и в процессе отмены регистрации из управления</span><span class="sxs-lookup"><span data-stu-id="652b2-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="652b2-117">ретирефаилед</span><span class="sxs-lookup"><span data-stu-id="652b2-117">retireFailed</span></span>|<span data-ttu-id="652b2-118">2</span><span class="sxs-lookup"><span data-stu-id="652b2-118">2</span></span>|<span data-ttu-id="652b2-119">На устройстве не удалось выполнить команду снятия с учета</span><span class="sxs-lookup"><span data-stu-id="652b2-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="652b2-120">випепендинг</span><span class="sxs-lookup"><span data-stu-id="652b2-120">wipePending</span></span>|<span data-ttu-id="652b2-121">4</span><span class="sxs-lookup"><span data-stu-id="652b2-121">3</span></span>|<span data-ttu-id="652b2-122">На устройстве и в процессе отмены регистрации в управлении возникает команда очистки.</span><span class="sxs-lookup"><span data-stu-id="652b2-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="652b2-123">випефаилед</span><span class="sxs-lookup"><span data-stu-id="652b2-123">wipeFailed</span></span>|<span data-ttu-id="652b2-124">SP4</span><span class="sxs-lookup"><span data-stu-id="652b2-124">4</span></span>|<span data-ttu-id="652b2-125">Не удалось выполнить команду очистки на устройстве</span><span class="sxs-lookup"><span data-stu-id="652b2-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="652b2-126">неисправности</span><span class="sxs-lookup"><span data-stu-id="652b2-126">unhealthy</span></span>|<span data-ttu-id="652b2-127">17:00</span><span class="sxs-lookup"><span data-stu-id="652b2-127">5</span></span>|<span data-ttu-id="652b2-128">Устройство неработоспособно.</span><span class="sxs-lookup"><span data-stu-id="652b2-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="652b2-129">делетепендинг</span><span class="sxs-lookup"><span data-stu-id="652b2-129">deletePending</span></span>|<span data-ttu-id="652b2-130">6 </span><span class="sxs-lookup"><span data-stu-id="652b2-130">6</span></span>|<span data-ttu-id="652b2-131">На устройстве выполняется команда Delete</span><span class="sxs-lookup"><span data-stu-id="652b2-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="652b2-132">ретиреиссуед</span><span class="sxs-lookup"><span data-stu-id="652b2-132">retireIssued</span></span>|<span data-ttu-id="652b2-133">7 </span><span class="sxs-lookup"><span data-stu-id="652b2-133">7</span></span>|<span data-ttu-id="652b2-134">Для устройства была выпущена команда снятия с учета</span><span class="sxs-lookup"><span data-stu-id="652b2-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="652b2-135">випеиссуед</span><span class="sxs-lookup"><span data-stu-id="652b2-135">wipeIssued</span></span>|<span data-ttu-id="652b2-136">8 </span><span class="sxs-lookup"><span data-stu-id="652b2-136">8</span></span>|<span data-ttu-id="652b2-137">Для устройства была выдана команда очистки.</span><span class="sxs-lookup"><span data-stu-id="652b2-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="652b2-138">випеканцелед</span><span class="sxs-lookup"><span data-stu-id="652b2-138">wipeCanceled</span></span>|<span data-ttu-id="652b2-139">9 </span><span class="sxs-lookup"><span data-stu-id="652b2-139">9</span></span>|<span data-ttu-id="652b2-140">Команда стирания для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="652b2-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="652b2-141">ретиреканцелед</span><span class="sxs-lookup"><span data-stu-id="652b2-141">retireCanceled</span></span>|<span data-ttu-id="652b2-142">10 </span><span class="sxs-lookup"><span data-stu-id="652b2-142">10</span></span>|<span data-ttu-id="652b2-143">Команда снятия с учета для этого устройства отменена</span><span class="sxs-lookup"><span data-stu-id="652b2-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="652b2-144">были</span><span class="sxs-lookup"><span data-stu-id="652b2-144">discovered</span></span>|<span data-ttu-id="652b2-145">-11:00</span><span class="sxs-lookup"><span data-stu-id="652b2-145">11</span></span>|<span data-ttu-id="652b2-146">Устройство обнаружено, но не зарегистрировано полностью.</span><span class="sxs-lookup"><span data-stu-id="652b2-146">The device is discovered but not fully enrolled.</span></span>|



