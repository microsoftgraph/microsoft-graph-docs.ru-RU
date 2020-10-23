---
title: тип перечисления deviceComplianceActionType
description: Перечисление типов запланированных действий
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 33b18120e5ae0d928fbd7a7a42e87bf7f71d10ec
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735850"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="67eb2-103">тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="67eb2-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="67eb2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67eb2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67eb2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67eb2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67eb2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67eb2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67eb2-107">Перечисление типов запланированных действий</span><span class="sxs-lookup"><span data-stu-id="67eb2-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="67eb2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="67eb2-108">Members</span></span>
|<span data-ttu-id="67eb2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="67eb2-109">Member</span></span>|<span data-ttu-id="67eb2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="67eb2-110">Value</span></span>|<span data-ttu-id="67eb2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="67eb2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67eb2-112">noAction</span><span class="sxs-lookup"><span data-stu-id="67eb2-112">noAction</span></span>|<span data-ttu-id="67eb2-113">нуль</span><span class="sxs-lookup"><span data-stu-id="67eb2-113">0</span></span>|<span data-ttu-id="67eb2-114">Без действий</span><span class="sxs-lookup"><span data-stu-id="67eb2-114">No Action</span></span>|
|<span data-ttu-id="67eb2-115">уведомляющее</span><span class="sxs-lookup"><span data-stu-id="67eb2-115">notification</span></span>|<span data-ttu-id="67eb2-116">1,1</span><span class="sxs-lookup"><span data-stu-id="67eb2-116">1</span></span>|<span data-ttu-id="67eb2-117">Уведомление об отправке</span><span class="sxs-lookup"><span data-stu-id="67eb2-117">Send Notification</span></span>|
|<span data-ttu-id="67eb2-118">блок</span><span class="sxs-lookup"><span data-stu-id="67eb2-118">block</span></span>|<span data-ttu-id="67eb2-119">2</span><span class="sxs-lookup"><span data-stu-id="67eb2-119">2</span></span>|<span data-ttu-id="67eb2-120">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="67eb2-120">Block the device in AAD</span></span>|
|<span data-ttu-id="67eb2-121">снять</span><span class="sxs-lookup"><span data-stu-id="67eb2-121">retire</span></span>|<span data-ttu-id="67eb2-122">4</span><span class="sxs-lookup"><span data-stu-id="67eb2-122">3</span></span>|<span data-ttu-id="67eb2-123">Прекращение использования устройства</span><span class="sxs-lookup"><span data-stu-id="67eb2-123">Retire the device</span></span>|
|<span data-ttu-id="67eb2-124">Очистка</span><span class="sxs-lookup"><span data-stu-id="67eb2-124">wipe</span></span>|<span data-ttu-id="67eb2-125">4 </span><span class="sxs-lookup"><span data-stu-id="67eb2-125">4</span></span>|<span data-ttu-id="67eb2-126">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="67eb2-126">Wipe the device</span></span>|
|<span data-ttu-id="67eb2-127">ремовересаурцеакцесспрофилес</span><span class="sxs-lookup"><span data-stu-id="67eb2-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="67eb2-128">5 </span><span class="sxs-lookup"><span data-stu-id="67eb2-128">5</span></span>|<span data-ttu-id="67eb2-129">Удаление профилей доступа к ресурсам с устройства</span><span class="sxs-lookup"><span data-stu-id="67eb2-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="67eb2-130">пушнотификатион</span><span class="sxs-lookup"><span data-stu-id="67eb2-130">pushNotification</span></span>|<span data-ttu-id="67eb2-131">9 </span><span class="sxs-lookup"><span data-stu-id="67eb2-131">9</span></span>|<span data-ttu-id="67eb2-132">Отправка push-уведомления на устройство</span><span class="sxs-lookup"><span data-stu-id="67eb2-132">Send push notification to device</span></span>|
|<span data-ttu-id="67eb2-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="67eb2-133">remoteLock</span></span>|<span data-ttu-id="67eb2-134">10 </span><span class="sxs-lookup"><span data-stu-id="67eb2-134">10</span></span>|<span data-ttu-id="67eb2-135">Удаленная блокировка устройства</span><span class="sxs-lookup"><span data-stu-id="67eb2-135">Remotely lock the device</span></span>|





