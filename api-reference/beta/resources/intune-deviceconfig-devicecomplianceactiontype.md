---
title: тип перечисления deviceComplianceActionType
description: Перечисление типов запланированных действий
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4ebf4df22787d19e5718ebd2099cd81af3925271
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793361"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="3932f-103">тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="3932f-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="3932f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3932f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3932f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3932f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3932f-106">Перечисление типов запланированных действий</span><span class="sxs-lookup"><span data-stu-id="3932f-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="3932f-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3932f-107">Members</span></span>
|<span data-ttu-id="3932f-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3932f-108">Member</span></span>|<span data-ttu-id="3932f-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3932f-109">Value</span></span>|<span data-ttu-id="3932f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3932f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3932f-111">noAction</span><span class="sxs-lookup"><span data-stu-id="3932f-111">noAction</span></span>|<span data-ttu-id="3932f-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3932f-112">0</span></span>|<span data-ttu-id="3932f-113">Без действий</span><span class="sxs-lookup"><span data-stu-id="3932f-113">No Action</span></span>|
|<span data-ttu-id="3932f-114">уведомляющее</span><span class="sxs-lookup"><span data-stu-id="3932f-114">notification</span></span>|<span data-ttu-id="3932f-115">1,1</span><span class="sxs-lookup"><span data-stu-id="3932f-115">1</span></span>|<span data-ttu-id="3932f-116">Уведомление об отправке</span><span class="sxs-lookup"><span data-stu-id="3932f-116">Send Notification</span></span>|
|<span data-ttu-id="3932f-117">блок</span><span class="sxs-lookup"><span data-stu-id="3932f-117">block</span></span>|<span data-ttu-id="3932f-118">2</span><span class="sxs-lookup"><span data-stu-id="3932f-118">2</span></span>|<span data-ttu-id="3932f-119">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="3932f-119">Block the device in AAD</span></span>|
|<span data-ttu-id="3932f-120">снять</span><span class="sxs-lookup"><span data-stu-id="3932f-120">retire</span></span>|<span data-ttu-id="3932f-121">4</span><span class="sxs-lookup"><span data-stu-id="3932f-121">3</span></span>|<span data-ttu-id="3932f-122">Прекращение использования устройства</span><span class="sxs-lookup"><span data-stu-id="3932f-122">Retire the device</span></span>|
|<span data-ttu-id="3932f-123">Очистка</span><span class="sxs-lookup"><span data-stu-id="3932f-123">wipe</span></span>|<span data-ttu-id="3932f-124">4 </span><span class="sxs-lookup"><span data-stu-id="3932f-124">4</span></span>|<span data-ttu-id="3932f-125">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="3932f-125">Wipe the device</span></span>|
|<span data-ttu-id="3932f-126">ремовересаурцеакцесспрофилес</span><span class="sxs-lookup"><span data-stu-id="3932f-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="3932f-127">5 </span><span class="sxs-lookup"><span data-stu-id="3932f-127">5</span></span>|<span data-ttu-id="3932f-128">Удаление профилей доступа к ресурсам с устройства</span><span class="sxs-lookup"><span data-stu-id="3932f-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="3932f-129">пушнотификатион</span><span class="sxs-lookup"><span data-stu-id="3932f-129">pushNotification</span></span>|<span data-ttu-id="3932f-130">9 </span><span class="sxs-lookup"><span data-stu-id="3932f-130">9</span></span>|<span data-ttu-id="3932f-131">Отправка push-уведомления на устройство</span><span class="sxs-lookup"><span data-stu-id="3932f-131">Send push notification to device</span></span>|
|<span data-ttu-id="3932f-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="3932f-132">remoteLock</span></span>|<span data-ttu-id="3932f-133">10 </span><span class="sxs-lookup"><span data-stu-id="3932f-133">10</span></span>|<span data-ttu-id="3932f-134">Удаленная блокировка устройства</span><span class="sxs-lookup"><span data-stu-id="3932f-134">Remotely lock the device</span></span>|



