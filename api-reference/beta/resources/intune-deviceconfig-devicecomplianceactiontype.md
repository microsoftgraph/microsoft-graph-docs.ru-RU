---
title: тип перечисления deviceComplianceActionType
description: Перечисление типов запланированных действий
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f441179e425f341d55eaee02525894aec53e487c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085047"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="c38b3-103">тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="c38b3-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="c38b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c38b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c38b3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c38b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c38b3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c38b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c38b3-107">Перечисление типов запланированных действий</span><span class="sxs-lookup"><span data-stu-id="c38b3-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="c38b3-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c38b3-108">Members</span></span>
|<span data-ttu-id="c38b3-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c38b3-109">Member</span></span>|<span data-ttu-id="c38b3-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c38b3-110">Value</span></span>|<span data-ttu-id="c38b3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c38b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c38b3-112">noAction</span><span class="sxs-lookup"><span data-stu-id="c38b3-112">noAction</span></span>|<span data-ttu-id="c38b3-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c38b3-113">0</span></span>|<span data-ttu-id="c38b3-114">Без действий</span><span class="sxs-lookup"><span data-stu-id="c38b3-114">No Action</span></span>|
|<span data-ttu-id="c38b3-115">уведомляющее</span><span class="sxs-lookup"><span data-stu-id="c38b3-115">notification</span></span>|<span data-ttu-id="c38b3-116">1 </span><span class="sxs-lookup"><span data-stu-id="c38b3-116">1</span></span>|<span data-ttu-id="c38b3-117">Уведомление об отправке</span><span class="sxs-lookup"><span data-stu-id="c38b3-117">Send Notification</span></span>|
|<span data-ttu-id="c38b3-118">блок</span><span class="sxs-lookup"><span data-stu-id="c38b3-118">block</span></span>|<span data-ttu-id="c38b3-119">2 </span><span class="sxs-lookup"><span data-stu-id="c38b3-119">2</span></span>|<span data-ttu-id="c38b3-120">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="c38b3-120">Block the device in AAD</span></span>|
|<span data-ttu-id="c38b3-121">снять</span><span class="sxs-lookup"><span data-stu-id="c38b3-121">retire</span></span>|<span data-ttu-id="c38b3-122">4</span><span class="sxs-lookup"><span data-stu-id="c38b3-122">3</span></span>|<span data-ttu-id="c38b3-123">Прекращение использования устройства</span><span class="sxs-lookup"><span data-stu-id="c38b3-123">Retire the device</span></span>|
|<span data-ttu-id="c38b3-124">Очистка</span><span class="sxs-lookup"><span data-stu-id="c38b3-124">wipe</span></span>|<span data-ttu-id="c38b3-125">4 </span><span class="sxs-lookup"><span data-stu-id="c38b3-125">4</span></span>|<span data-ttu-id="c38b3-126">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="c38b3-126">Wipe the device</span></span>|
|<span data-ttu-id="c38b3-127">ремовересаурцеакцесспрофилес</span><span class="sxs-lookup"><span data-stu-id="c38b3-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="c38b3-128">5 </span><span class="sxs-lookup"><span data-stu-id="c38b3-128">5</span></span>|<span data-ttu-id="c38b3-129">Удаление профилей доступа к ресурсам с устройства</span><span class="sxs-lookup"><span data-stu-id="c38b3-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="c38b3-130">пушнотификатион</span><span class="sxs-lookup"><span data-stu-id="c38b3-130">pushNotification</span></span>|<span data-ttu-id="c38b3-131">9 </span><span class="sxs-lookup"><span data-stu-id="c38b3-131">9</span></span>|<span data-ttu-id="c38b3-132">Отправка push-уведомления на устройство</span><span class="sxs-lookup"><span data-stu-id="c38b3-132">Send push notification to device</span></span>|
|<span data-ttu-id="c38b3-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="c38b3-133">remoteLock</span></span>|<span data-ttu-id="c38b3-134">10 </span><span class="sxs-lookup"><span data-stu-id="c38b3-134">10</span></span>|<span data-ttu-id="c38b3-135">Удаленная блокировка устройства</span><span class="sxs-lookup"><span data-stu-id="c38b3-135">Remotely lock the device</span></span>|






