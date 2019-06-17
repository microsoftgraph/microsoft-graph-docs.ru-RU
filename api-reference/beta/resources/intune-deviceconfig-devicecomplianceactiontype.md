---
title: тип перечисления deviceComplianceActionType
description: Перечисление типов запланированных действий
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05f9df39c563a47fa571a4badcf789ea4ddb08b1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979531"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="3af6e-103">тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="3af6e-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="3af6e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3af6e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3af6e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3af6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3af6e-106">Перечисление типов запланированных действий</span><span class="sxs-lookup"><span data-stu-id="3af6e-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="3af6e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3af6e-107">Members</span></span>
|<span data-ttu-id="3af6e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3af6e-108">Member</span></span>|<span data-ttu-id="3af6e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3af6e-109">Value</span></span>|<span data-ttu-id="3af6e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3af6e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3af6e-111">noAction</span><span class="sxs-lookup"><span data-stu-id="3af6e-111">noAction</span></span>|<span data-ttu-id="3af6e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3af6e-112">0</span></span>|<span data-ttu-id="3af6e-113">Без действий</span><span class="sxs-lookup"><span data-stu-id="3af6e-113">No Action</span></span>|
|<span data-ttu-id="3af6e-114">уведомляющее</span><span class="sxs-lookup"><span data-stu-id="3af6e-114">notification</span></span>|<span data-ttu-id="3af6e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="3af6e-115">1</span></span>|<span data-ttu-id="3af6e-116">Уведомление об отправке</span><span class="sxs-lookup"><span data-stu-id="3af6e-116">Send Notification</span></span>|
|<span data-ttu-id="3af6e-117">блок</span><span class="sxs-lookup"><span data-stu-id="3af6e-117">block</span></span>|<span data-ttu-id="3af6e-118">2</span><span class="sxs-lookup"><span data-stu-id="3af6e-118">2</span></span>|<span data-ttu-id="3af6e-119">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="3af6e-119">Block the device in AAD</span></span>|
|<span data-ttu-id="3af6e-120">снять</span><span class="sxs-lookup"><span data-stu-id="3af6e-120">retire</span></span>|<span data-ttu-id="3af6e-121">4</span><span class="sxs-lookup"><span data-stu-id="3af6e-121">3</span></span>|<span data-ttu-id="3af6e-122">Прекращение использования устройства</span><span class="sxs-lookup"><span data-stu-id="3af6e-122">Retire the device</span></span>|
|<span data-ttu-id="3af6e-123">Очистка</span><span class="sxs-lookup"><span data-stu-id="3af6e-123">wipe</span></span>|<span data-ttu-id="3af6e-124">SP4</span><span class="sxs-lookup"><span data-stu-id="3af6e-124">4</span></span>|<span data-ttu-id="3af6e-125">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="3af6e-125">Wipe the device</span></span>|
|<span data-ttu-id="3af6e-126">Ремовересаурцеакцесспрофилес</span><span class="sxs-lookup"><span data-stu-id="3af6e-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="3af6e-127">17:00</span><span class="sxs-lookup"><span data-stu-id="3af6e-127">5</span></span>|<span data-ttu-id="3af6e-128">Удаление профилей доступа к ресурсам с устройства</span><span class="sxs-lookup"><span data-stu-id="3af6e-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="3af6e-129">Пушнотификатион</span><span class="sxs-lookup"><span data-stu-id="3af6e-129">pushNotification</span></span>|<span data-ttu-id="3af6e-130">9 </span><span class="sxs-lookup"><span data-stu-id="3af6e-130">9</span></span>|<span data-ttu-id="3af6e-131">Отправка push-уведомления на устройство</span><span class="sxs-lookup"><span data-stu-id="3af6e-131">Send push notification to device</span></span>|
|<span data-ttu-id="3af6e-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="3af6e-132">remoteLock</span></span>|<span data-ttu-id="3af6e-133">10 </span><span class="sxs-lookup"><span data-stu-id="3af6e-133">10</span></span>|<span data-ttu-id="3af6e-134">Удаленная блокировка устройства</span><span class="sxs-lookup"><span data-stu-id="3af6e-134">Remotely lock the device</span></span>|





