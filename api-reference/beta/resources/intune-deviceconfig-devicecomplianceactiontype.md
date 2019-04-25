---
title: тип перечисления deviceComplianceActionType
description: ПереЧисление типов запланированных действий
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba07cb2b0fe076642cb1157a5d5df09a04a63a47
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566033"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="725fb-103">тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="725fb-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="725fb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="725fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="725fb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="725fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="725fb-106">ПереЧисление типов запланированных действий</span><span class="sxs-lookup"><span data-stu-id="725fb-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="725fb-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="725fb-107">Members</span></span>
|<span data-ttu-id="725fb-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="725fb-108">Member</span></span>|<span data-ttu-id="725fb-109">Значение</span><span class="sxs-lookup"><span data-stu-id="725fb-109">Value</span></span>|<span data-ttu-id="725fb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="725fb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="725fb-111">noAction</span><span class="sxs-lookup"><span data-stu-id="725fb-111">noAction</span></span>|<span data-ttu-id="725fb-112">нуль</span><span class="sxs-lookup"><span data-stu-id="725fb-112">0</span></span>|<span data-ttu-id="725fb-113">Без действий</span><span class="sxs-lookup"><span data-stu-id="725fb-113">No Action</span></span>|
|<span data-ttu-id="725fb-114">уведомляющее</span><span class="sxs-lookup"><span data-stu-id="725fb-114">notification</span></span>|<span data-ttu-id="725fb-115">1 </span><span class="sxs-lookup"><span data-stu-id="725fb-115">1</span></span>|<span data-ttu-id="725fb-116">Уведомление об отПравке</span><span class="sxs-lookup"><span data-stu-id="725fb-116">Send Notification</span></span>|
|<span data-ttu-id="725fb-117">блок</span><span class="sxs-lookup"><span data-stu-id="725fb-117">block</span></span>|<span data-ttu-id="725fb-118">2 </span><span class="sxs-lookup"><span data-stu-id="725fb-118">2</span></span>|<span data-ttu-id="725fb-119">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="725fb-119">Block the device in AAD</span></span>|
|<span data-ttu-id="725fb-120">снять</span><span class="sxs-lookup"><span data-stu-id="725fb-120">retire</span></span>|<span data-ttu-id="725fb-121">3 </span><span class="sxs-lookup"><span data-stu-id="725fb-121">3</span></span>|<span data-ttu-id="725fb-122">Прекращение использования устройства</span><span class="sxs-lookup"><span data-stu-id="725fb-122">Retire the device</span></span>|
|<span data-ttu-id="725fb-123">Очистка</span><span class="sxs-lookup"><span data-stu-id="725fb-123">wipe</span></span>|<span data-ttu-id="725fb-124">4 </span><span class="sxs-lookup"><span data-stu-id="725fb-124">4</span></span>|<span data-ttu-id="725fb-125">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="725fb-125">Wipe the device</span></span>|
|<span data-ttu-id="725fb-126">Ремовересаурцеакцесспрофилес</span><span class="sxs-lookup"><span data-stu-id="725fb-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="725fb-127">5 </span><span class="sxs-lookup"><span data-stu-id="725fb-127">5</span></span>|<span data-ttu-id="725fb-128">Удаление профилей доступа к ресурсам с устройства</span><span class="sxs-lookup"><span data-stu-id="725fb-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="725fb-129">Пушнотификатион</span><span class="sxs-lookup"><span data-stu-id="725fb-129">pushNotification</span></span>|<span data-ttu-id="725fb-130">9 </span><span class="sxs-lookup"><span data-stu-id="725fb-130">9</span></span>|<span data-ttu-id="725fb-131">Отправка push-уведомления на устройство</span><span class="sxs-lookup"><span data-stu-id="725fb-131">Send push notification to device</span></span>|
|<span data-ttu-id="725fb-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="725fb-132">remoteLock</span></span>|<span data-ttu-id="725fb-133">10 </span><span class="sxs-lookup"><span data-stu-id="725fb-133">10</span></span>|<span data-ttu-id="725fb-134">Удаленная блокировка устройства</span><span class="sxs-lookup"><span data-stu-id="725fb-134">Remotely lock the device</span></span>|





