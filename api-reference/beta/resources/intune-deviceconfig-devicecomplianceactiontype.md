---
title: тип перечисления deviceComplianceActionType
description: Перечисление типов запланированных действий
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bff5247237cc0d6daf45515c5bdbaaa3e675017a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526722"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="6cdce-103">тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="6cdce-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="6cdce-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6cdce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cdce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cdce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cdce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6cdce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cdce-107">Перечисление типов запланированных действий</span><span class="sxs-lookup"><span data-stu-id="6cdce-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="6cdce-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="6cdce-108">Members</span></span>
|<span data-ttu-id="6cdce-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="6cdce-109">Member</span></span>|<span data-ttu-id="6cdce-110">Значение</span><span class="sxs-lookup"><span data-stu-id="6cdce-110">Value</span></span>|<span data-ttu-id="6cdce-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6cdce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cdce-112">noAction</span><span class="sxs-lookup"><span data-stu-id="6cdce-112">noAction</span></span>|<span data-ttu-id="6cdce-113">нуль</span><span class="sxs-lookup"><span data-stu-id="6cdce-113">0</span></span>|<span data-ttu-id="6cdce-114">Без действий</span><span class="sxs-lookup"><span data-stu-id="6cdce-114">No Action</span></span>|
|<span data-ttu-id="6cdce-115">уведомляющее</span><span class="sxs-lookup"><span data-stu-id="6cdce-115">notification</span></span>|<span data-ttu-id="6cdce-116">1 </span><span class="sxs-lookup"><span data-stu-id="6cdce-116">1</span></span>|<span data-ttu-id="6cdce-117">Уведомление об отправке</span><span class="sxs-lookup"><span data-stu-id="6cdce-117">Send Notification</span></span>|
|<span data-ttu-id="6cdce-118">блок</span><span class="sxs-lookup"><span data-stu-id="6cdce-118">block</span></span>|<span data-ttu-id="6cdce-119">2 </span><span class="sxs-lookup"><span data-stu-id="6cdce-119">2</span></span>|<span data-ttu-id="6cdce-120">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="6cdce-120">Block the device in AAD</span></span>|
|<span data-ttu-id="6cdce-121">снять</span><span class="sxs-lookup"><span data-stu-id="6cdce-121">retire</span></span>|<span data-ttu-id="6cdce-122">3 </span><span class="sxs-lookup"><span data-stu-id="6cdce-122">3</span></span>|<span data-ttu-id="6cdce-123">Прекращение использования устройства</span><span class="sxs-lookup"><span data-stu-id="6cdce-123">Retire the device</span></span>|
|<span data-ttu-id="6cdce-124">Очистка</span><span class="sxs-lookup"><span data-stu-id="6cdce-124">wipe</span></span>|<span data-ttu-id="6cdce-125">4 </span><span class="sxs-lookup"><span data-stu-id="6cdce-125">4</span></span>|<span data-ttu-id="6cdce-126">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="6cdce-126">Wipe the device</span></span>|
|<span data-ttu-id="6cdce-127">ремовересаурцеакцесспрофилес</span><span class="sxs-lookup"><span data-stu-id="6cdce-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="6cdce-128">5 </span><span class="sxs-lookup"><span data-stu-id="6cdce-128">5</span></span>|<span data-ttu-id="6cdce-129">Удаление профилей доступа к ресурсам с устройства</span><span class="sxs-lookup"><span data-stu-id="6cdce-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="6cdce-130">пушнотификатион</span><span class="sxs-lookup"><span data-stu-id="6cdce-130">pushNotification</span></span>|<span data-ttu-id="6cdce-131">9 </span><span class="sxs-lookup"><span data-stu-id="6cdce-131">9</span></span>|<span data-ttu-id="6cdce-132">Отправка push-уведомления на устройство</span><span class="sxs-lookup"><span data-stu-id="6cdce-132">Send push notification to device</span></span>|
|<span data-ttu-id="6cdce-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="6cdce-133">remoteLock</span></span>|<span data-ttu-id="6cdce-134">10 </span><span class="sxs-lookup"><span data-stu-id="6cdce-134">10</span></span>|<span data-ttu-id="6cdce-135">Удаленная блокировка устройства</span><span class="sxs-lookup"><span data-stu-id="6cdce-135">Remotely lock the device</span></span>|



