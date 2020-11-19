---
title: тип перечисления deviceComplianceActionType
description: Перечисление типов запланированных действий
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b2af0545dda4461115ed5f11975a6c9371d4010d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283681"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="c0c28-103">тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="c0c28-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="c0c28-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0c28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0c28-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0c28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0c28-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0c28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0c28-107">Перечисление типов запланированных действий</span><span class="sxs-lookup"><span data-stu-id="c0c28-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="c0c28-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c0c28-108">Members</span></span>
|<span data-ttu-id="c0c28-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c0c28-109">Member</span></span>|<span data-ttu-id="c0c28-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c0c28-110">Value</span></span>|<span data-ttu-id="c0c28-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c0c28-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0c28-112">noAction</span><span class="sxs-lookup"><span data-stu-id="c0c28-112">noAction</span></span>|<span data-ttu-id="c0c28-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c0c28-113">0</span></span>|<span data-ttu-id="c0c28-114">Без действий</span><span class="sxs-lookup"><span data-stu-id="c0c28-114">No Action</span></span>|
|<span data-ttu-id="c0c28-115">уведомляющее</span><span class="sxs-lookup"><span data-stu-id="c0c28-115">notification</span></span>|<span data-ttu-id="c0c28-116">1,1</span><span class="sxs-lookup"><span data-stu-id="c0c28-116">1</span></span>|<span data-ttu-id="c0c28-117">Уведомление об отправке</span><span class="sxs-lookup"><span data-stu-id="c0c28-117">Send Notification</span></span>|
|<span data-ttu-id="c0c28-118">блок</span><span class="sxs-lookup"><span data-stu-id="c0c28-118">block</span></span>|<span data-ttu-id="c0c28-119">2</span><span class="sxs-lookup"><span data-stu-id="c0c28-119">2</span></span>|<span data-ttu-id="c0c28-120">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="c0c28-120">Block the device in AAD</span></span>|
|<span data-ttu-id="c0c28-121">снять</span><span class="sxs-lookup"><span data-stu-id="c0c28-121">retire</span></span>|<span data-ttu-id="c0c28-122">4</span><span class="sxs-lookup"><span data-stu-id="c0c28-122">3</span></span>|<span data-ttu-id="c0c28-123">Прекращение использования устройства</span><span class="sxs-lookup"><span data-stu-id="c0c28-123">Retire the device</span></span>|
|<span data-ttu-id="c0c28-124">Очистка</span><span class="sxs-lookup"><span data-stu-id="c0c28-124">wipe</span></span>|<span data-ttu-id="c0c28-125">4 </span><span class="sxs-lookup"><span data-stu-id="c0c28-125">4</span></span>|<span data-ttu-id="c0c28-126">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="c0c28-126">Wipe the device</span></span>|
|<span data-ttu-id="c0c28-127">ремовересаурцеакцесспрофилес</span><span class="sxs-lookup"><span data-stu-id="c0c28-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="c0c28-128">5 </span><span class="sxs-lookup"><span data-stu-id="c0c28-128">5</span></span>|<span data-ttu-id="c0c28-129">Удаление профилей доступа к ресурсам с устройства</span><span class="sxs-lookup"><span data-stu-id="c0c28-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="c0c28-130">пушнотификатион</span><span class="sxs-lookup"><span data-stu-id="c0c28-130">pushNotification</span></span>|<span data-ttu-id="c0c28-131">9 </span><span class="sxs-lookup"><span data-stu-id="c0c28-131">9</span></span>|<span data-ttu-id="c0c28-132">Отправка push-уведомления на устройство</span><span class="sxs-lookup"><span data-stu-id="c0c28-132">Send push notification to device</span></span>|
|<span data-ttu-id="c0c28-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="c0c28-133">remoteLock</span></span>|<span data-ttu-id="c0c28-134">10 </span><span class="sxs-lookup"><span data-stu-id="c0c28-134">10</span></span>|<span data-ttu-id="c0c28-135">Удаленная блокировка устройства</span><span class="sxs-lookup"><span data-stu-id="c0c28-135">Remotely lock the device</span></span>|




