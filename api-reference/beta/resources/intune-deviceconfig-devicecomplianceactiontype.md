---
title: тип перечисления deviceComplianceActionType
description: Перечисление типов запланированных действий
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37caa3ca741c752a67a9f90222856b31fa4978c3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947206"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="865ed-103">тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="865ed-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="865ed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="865ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="865ed-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="865ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="865ed-106">Перечисление типов запланированных действий</span><span class="sxs-lookup"><span data-stu-id="865ed-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="865ed-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="865ed-107">Members</span></span>
|<span data-ttu-id="865ed-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="865ed-108">Member</span></span>|<span data-ttu-id="865ed-109">Значение</span><span class="sxs-lookup"><span data-stu-id="865ed-109">Value</span></span>|<span data-ttu-id="865ed-110">Описание</span><span class="sxs-lookup"><span data-stu-id="865ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="865ed-111">noAction</span><span class="sxs-lookup"><span data-stu-id="865ed-111">noAction</span></span>|<span data-ttu-id="865ed-112">нуль</span><span class="sxs-lookup"><span data-stu-id="865ed-112">0</span></span>|<span data-ttu-id="865ed-113">Без действий</span><span class="sxs-lookup"><span data-stu-id="865ed-113">No Action</span></span>|
|<span data-ttu-id="865ed-114">уведомляющее</span><span class="sxs-lookup"><span data-stu-id="865ed-114">notification</span></span>|<span data-ttu-id="865ed-115">1,1</span><span class="sxs-lookup"><span data-stu-id="865ed-115">1</span></span>|<span data-ttu-id="865ed-116">Уведомление об отправке</span><span class="sxs-lookup"><span data-stu-id="865ed-116">Send Notification</span></span>|
|<span data-ttu-id="865ed-117">блок</span><span class="sxs-lookup"><span data-stu-id="865ed-117">block</span></span>|<span data-ttu-id="865ed-118">2</span><span class="sxs-lookup"><span data-stu-id="865ed-118">2</span></span>|<span data-ttu-id="865ed-119">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="865ed-119">Block the device in AAD</span></span>|
|<span data-ttu-id="865ed-120">снять</span><span class="sxs-lookup"><span data-stu-id="865ed-120">retire</span></span>|<span data-ttu-id="865ed-121">4</span><span class="sxs-lookup"><span data-stu-id="865ed-121">3</span></span>|<span data-ttu-id="865ed-122">Прекращение использования устройства</span><span class="sxs-lookup"><span data-stu-id="865ed-122">Retire the device</span></span>|
|<span data-ttu-id="865ed-123">Очистка</span><span class="sxs-lookup"><span data-stu-id="865ed-123">wipe</span></span>|<span data-ttu-id="865ed-124">SP4</span><span class="sxs-lookup"><span data-stu-id="865ed-124">4</span></span>|<span data-ttu-id="865ed-125">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="865ed-125">Wipe the device</span></span>|
|<span data-ttu-id="865ed-126">Ремовересаурцеакцесспрофилес</span><span class="sxs-lookup"><span data-stu-id="865ed-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="865ed-127">17:00</span><span class="sxs-lookup"><span data-stu-id="865ed-127">5</span></span>|<span data-ttu-id="865ed-128">Удаление профилей доступа к ресурсам с устройства</span><span class="sxs-lookup"><span data-stu-id="865ed-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="865ed-129">Пушнотификатион</span><span class="sxs-lookup"><span data-stu-id="865ed-129">pushNotification</span></span>|<span data-ttu-id="865ed-130">9 </span><span class="sxs-lookup"><span data-stu-id="865ed-130">9</span></span>|<span data-ttu-id="865ed-131">Отправка push-уведомления на устройство</span><span class="sxs-lookup"><span data-stu-id="865ed-131">Send push notification to device</span></span>|
|<span data-ttu-id="865ed-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="865ed-132">remoteLock</span></span>|<span data-ttu-id="865ed-133">10 </span><span class="sxs-lookup"><span data-stu-id="865ed-133">10</span></span>|<span data-ttu-id="865ed-134">Удаленная блокировка устройства</span><span class="sxs-lookup"><span data-stu-id="865ed-134">Remotely lock the device</span></span>|




