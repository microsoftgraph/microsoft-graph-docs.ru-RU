---
title: Тип перечисления deviceComplianceActionType
description: Запланировано действие типа Enum
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cd0db68a21fff79ddbab924e8a1d9bd2ff2e542d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425745"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="d8865-103">Тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="d8865-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="d8865-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d8865-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d8865-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8865-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8865-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8865-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8865-107">Запланировано действие типа Enum</span><span class="sxs-lookup"><span data-stu-id="d8865-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="d8865-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d8865-108">Members</span></span>
|<span data-ttu-id="d8865-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d8865-109">Member</span></span>|<span data-ttu-id="d8865-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d8865-110">Value</span></span>|<span data-ttu-id="d8865-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d8865-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8865-112">noAction</span><span class="sxs-lookup"><span data-stu-id="d8865-112">noAction</span></span>|<span data-ttu-id="d8865-113">0</span><span class="sxs-lookup"><span data-stu-id="d8865-113">0</span></span>|<span data-ttu-id="d8865-114">Никаких действий</span><span class="sxs-lookup"><span data-stu-id="d8865-114">No Action</span></span>|
|<span data-ttu-id="d8865-115">уведомления</span><span class="sxs-lookup"><span data-stu-id="d8865-115">notification</span></span>|<span data-ttu-id="d8865-116">1</span><span class="sxs-lookup"><span data-stu-id="d8865-116">1</span></span>|<span data-ttu-id="d8865-117">Отправить уведомление</span><span class="sxs-lookup"><span data-stu-id="d8865-117">Send Notification</span></span>|
|<span data-ttu-id="d8865-118">блок</span><span class="sxs-lookup"><span data-stu-id="d8865-118">block</span></span>|<span data-ttu-id="d8865-119">2</span><span class="sxs-lookup"><span data-stu-id="d8865-119">2</span></span>|<span data-ttu-id="d8865-120">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="d8865-120">Block the device in AAD</span></span>|
|<span data-ttu-id="d8865-121">Удаление</span><span class="sxs-lookup"><span data-stu-id="d8865-121">retire</span></span>|<span data-ttu-id="d8865-122">3</span><span class="sxs-lookup"><span data-stu-id="d8865-122">3</span></span>|<span data-ttu-id="d8865-123">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="d8865-123">Retire the device</span></span>|
|<span data-ttu-id="d8865-124">Очистка</span><span class="sxs-lookup"><span data-stu-id="d8865-124">wipe</span></span>|<span data-ttu-id="d8865-125">4</span><span class="sxs-lookup"><span data-stu-id="d8865-125">4</span></span>|<span data-ttu-id="d8865-126">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="d8865-126">Wipe the device</span></span>|
|<span data-ttu-id="d8865-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="d8865-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="d8865-128">5</span><span class="sxs-lookup"><span data-stu-id="d8865-128">5</span></span>|<span data-ttu-id="d8865-129">Удаление профилей доступа ресурсов с устройства</span><span class="sxs-lookup"><span data-stu-id="d8865-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="d8865-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="d8865-130">pushNotification</span></span>|<span data-ttu-id="d8865-131">9</span><span class="sxs-lookup"><span data-stu-id="d8865-131">9</span></span>|<span data-ttu-id="d8865-132">Отправить push-уведомлений для устройств</span><span class="sxs-lookup"><span data-stu-id="d8865-132">Send push notification to device</span></span>|
|<span data-ttu-id="d8865-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="d8865-133">remoteLock</span></span>|<span data-ttu-id="d8865-134">10</span><span class="sxs-lookup"><span data-stu-id="d8865-134">10</span></span>|<span data-ttu-id="d8865-135">Удаленно блокировка устройства</span><span class="sxs-lookup"><span data-stu-id="d8865-135">Remotely lock the device</span></span>|




