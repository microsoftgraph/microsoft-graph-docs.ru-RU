---
title: тип перечисления deviceComplianceActionType
description: Перечисление типов запланированных действий
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f0a5a3b4ab73bc0d97b5b47619cdcabb401400f2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437394"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="aff6a-103">тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="aff6a-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="aff6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aff6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aff6a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aff6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aff6a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aff6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aff6a-107">Перечисление типов запланированных действий</span><span class="sxs-lookup"><span data-stu-id="aff6a-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="aff6a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="aff6a-108">Members</span></span>
|<span data-ttu-id="aff6a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="aff6a-109">Member</span></span>|<span data-ttu-id="aff6a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="aff6a-110">Value</span></span>|<span data-ttu-id="aff6a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aff6a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aff6a-112">noAction</span><span class="sxs-lookup"><span data-stu-id="aff6a-112">noAction</span></span>|<span data-ttu-id="aff6a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="aff6a-113">0</span></span>|<span data-ttu-id="aff6a-114">Без действий</span><span class="sxs-lookup"><span data-stu-id="aff6a-114">No Action</span></span>|
|<span data-ttu-id="aff6a-115">уведомляющее</span><span class="sxs-lookup"><span data-stu-id="aff6a-115">notification</span></span>|<span data-ttu-id="aff6a-116">1,1</span><span class="sxs-lookup"><span data-stu-id="aff6a-116">1</span></span>|<span data-ttu-id="aff6a-117">Уведомление об отправке</span><span class="sxs-lookup"><span data-stu-id="aff6a-117">Send Notification</span></span>|
|<span data-ttu-id="aff6a-118">блок</span><span class="sxs-lookup"><span data-stu-id="aff6a-118">block</span></span>|<span data-ttu-id="aff6a-119">2</span><span class="sxs-lookup"><span data-stu-id="aff6a-119">2</span></span>|<span data-ttu-id="aff6a-120">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="aff6a-120">Block the device in AAD</span></span>|
|<span data-ttu-id="aff6a-121">снять</span><span class="sxs-lookup"><span data-stu-id="aff6a-121">retire</span></span>|<span data-ttu-id="aff6a-122">4</span><span class="sxs-lookup"><span data-stu-id="aff6a-122">3</span></span>|<span data-ttu-id="aff6a-123">Прекращение использования устройства</span><span class="sxs-lookup"><span data-stu-id="aff6a-123">Retire the device</span></span>|
|<span data-ttu-id="aff6a-124">Очистка</span><span class="sxs-lookup"><span data-stu-id="aff6a-124">wipe</span></span>|<span data-ttu-id="aff6a-125">4 </span><span class="sxs-lookup"><span data-stu-id="aff6a-125">4</span></span>|<span data-ttu-id="aff6a-126">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="aff6a-126">Wipe the device</span></span>|
|<span data-ttu-id="aff6a-127">ремовересаурцеакцесспрофилес</span><span class="sxs-lookup"><span data-stu-id="aff6a-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="aff6a-128">5 </span><span class="sxs-lookup"><span data-stu-id="aff6a-128">5</span></span>|<span data-ttu-id="aff6a-129">Удаление профилей доступа к ресурсам с устройства</span><span class="sxs-lookup"><span data-stu-id="aff6a-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="aff6a-130">пушнотификатион</span><span class="sxs-lookup"><span data-stu-id="aff6a-130">pushNotification</span></span>|<span data-ttu-id="aff6a-131">9 </span><span class="sxs-lookup"><span data-stu-id="aff6a-131">9</span></span>|<span data-ttu-id="aff6a-132">Отправка push-уведомления на устройство</span><span class="sxs-lookup"><span data-stu-id="aff6a-132">Send push notification to device</span></span>|
|<span data-ttu-id="aff6a-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="aff6a-133">remoteLock</span></span>|<span data-ttu-id="aff6a-134">10 </span><span class="sxs-lookup"><span data-stu-id="aff6a-134">10</span></span>|<span data-ttu-id="aff6a-135">Удаленная блокировка устройства</span><span class="sxs-lookup"><span data-stu-id="aff6a-135">Remotely lock the device</span></span>|



