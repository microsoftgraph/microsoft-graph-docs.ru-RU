---
title: тип перечисления deviceComplianceActionType
description: Перечисление типов запланированных действий
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2a8b74f0bb668a9354bc2d68d21a7c45e52d1c06
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530851"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="d76f1-103">тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="d76f1-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="d76f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d76f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d76f1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d76f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d76f1-106">Перечисление типов запланированных действий</span><span class="sxs-lookup"><span data-stu-id="d76f1-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="d76f1-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="d76f1-107">Members</span></span>
|<span data-ttu-id="d76f1-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="d76f1-108">Member</span></span>|<span data-ttu-id="d76f1-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d76f1-109">Value</span></span>|<span data-ttu-id="d76f1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d76f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d76f1-111">noAction</span><span class="sxs-lookup"><span data-stu-id="d76f1-111">noAction</span></span>|<span data-ttu-id="d76f1-112">нуль</span><span class="sxs-lookup"><span data-stu-id="d76f1-112">0</span></span>|<span data-ttu-id="d76f1-113">Без действий</span><span class="sxs-lookup"><span data-stu-id="d76f1-113">No Action</span></span>|
|<span data-ttu-id="d76f1-114">уведомляющее</span><span class="sxs-lookup"><span data-stu-id="d76f1-114">notification</span></span>|<span data-ttu-id="d76f1-115">1 </span><span class="sxs-lookup"><span data-stu-id="d76f1-115">1</span></span>|<span data-ttu-id="d76f1-116">Уведомление об отправке</span><span class="sxs-lookup"><span data-stu-id="d76f1-116">Send Notification</span></span>|
|<span data-ttu-id="d76f1-117">блок</span><span class="sxs-lookup"><span data-stu-id="d76f1-117">block</span></span>|<span data-ttu-id="d76f1-118">2 </span><span class="sxs-lookup"><span data-stu-id="d76f1-118">2</span></span>|<span data-ttu-id="d76f1-119">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="d76f1-119">Block the device in AAD</span></span>|
|<span data-ttu-id="d76f1-120">снять</span><span class="sxs-lookup"><span data-stu-id="d76f1-120">retire</span></span>|<span data-ttu-id="d76f1-121">3 </span><span class="sxs-lookup"><span data-stu-id="d76f1-121">3</span></span>|<span data-ttu-id="d76f1-122">Прекращение использования устройства</span><span class="sxs-lookup"><span data-stu-id="d76f1-122">Retire the device</span></span>|
|<span data-ttu-id="d76f1-123">Очистка</span><span class="sxs-lookup"><span data-stu-id="d76f1-123">wipe</span></span>|<span data-ttu-id="d76f1-124">4 </span><span class="sxs-lookup"><span data-stu-id="d76f1-124">4</span></span>|<span data-ttu-id="d76f1-125">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="d76f1-125">Wipe the device</span></span>|
|<span data-ttu-id="d76f1-126">ремовересаурцеакцесспрофилес</span><span class="sxs-lookup"><span data-stu-id="d76f1-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="d76f1-127">5 </span><span class="sxs-lookup"><span data-stu-id="d76f1-127">5</span></span>|<span data-ttu-id="d76f1-128">Удаление профилей доступа к ресурсам с устройства</span><span class="sxs-lookup"><span data-stu-id="d76f1-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="d76f1-129">пушнотификатион</span><span class="sxs-lookup"><span data-stu-id="d76f1-129">pushNotification</span></span>|<span data-ttu-id="d76f1-130">9 </span><span class="sxs-lookup"><span data-stu-id="d76f1-130">9</span></span>|<span data-ttu-id="d76f1-131">Отправка push-уведомления на устройство</span><span class="sxs-lookup"><span data-stu-id="d76f1-131">Send push notification to device</span></span>|




