---
title: Тип перечисления deviceComplianceActionType
description: Запланировано действие типа Enum
author: tfitzmac
ms.openlocfilehash: 84bef94d7352c13b49f223b859cea218932f8cad
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328688"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="a51d1-103">Тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="a51d1-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="a51d1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a51d1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a51d1-105">Запланировано действие типа Enum</span><span class="sxs-lookup"><span data-stu-id="a51d1-105">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="a51d1-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="a51d1-106">Members</span></span>
|<span data-ttu-id="a51d1-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="a51d1-107">Member</span></span>|<span data-ttu-id="a51d1-108">Значение</span><span class="sxs-lookup"><span data-stu-id="a51d1-108">Value</span></span>|<span data-ttu-id="a51d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a51d1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a51d1-110">noAction</span><span class="sxs-lookup"><span data-stu-id="a51d1-110">noAction</span></span>|<span data-ttu-id="a51d1-111">0</span><span class="sxs-lookup"><span data-stu-id="a51d1-111">0</span></span>|<span data-ttu-id="a51d1-112">Никаких действий</span><span class="sxs-lookup"><span data-stu-id="a51d1-112">No Action</span></span>|
|<span data-ttu-id="a51d1-113">уведомления</span><span class="sxs-lookup"><span data-stu-id="a51d1-113">notification</span></span>|<span data-ttu-id="a51d1-114">1</span><span class="sxs-lookup"><span data-stu-id="a51d1-114">1</span></span>|<span data-ttu-id="a51d1-115">Отправить уведомление</span><span class="sxs-lookup"><span data-stu-id="a51d1-115">Send Notification</span></span>|
|<span data-ttu-id="a51d1-116">блок</span><span class="sxs-lookup"><span data-stu-id="a51d1-116">block</span></span>|<span data-ttu-id="a51d1-117">2</span><span class="sxs-lookup"><span data-stu-id="a51d1-117">2</span></span>|<span data-ttu-id="a51d1-118">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="a51d1-118">Block the device in AAD</span></span>|
|<span data-ttu-id="a51d1-119">Удаление</span><span class="sxs-lookup"><span data-stu-id="a51d1-119">retire</span></span>|<span data-ttu-id="a51d1-120">3</span><span class="sxs-lookup"><span data-stu-id="a51d1-120">3</span></span>|<span data-ttu-id="a51d1-121">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="a51d1-121">Retire the device</span></span>|
|<span data-ttu-id="a51d1-122">Очистка</span><span class="sxs-lookup"><span data-stu-id="a51d1-122">wipe</span></span>|<span data-ttu-id="a51d1-123">4</span><span class="sxs-lookup"><span data-stu-id="a51d1-123">4</span></span>|<span data-ttu-id="a51d1-124">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="a51d1-124">Wipe the device</span></span>|
|<span data-ttu-id="a51d1-125">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="a51d1-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="a51d1-126">5</span><span class="sxs-lookup"><span data-stu-id="a51d1-126">5</span></span>|<span data-ttu-id="a51d1-127">Удаление профилей доступа ресурсов с устройства</span><span class="sxs-lookup"><span data-stu-id="a51d1-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="a51d1-128">pushNotification</span><span class="sxs-lookup"><span data-stu-id="a51d1-128">pushNotification</span></span>|<span data-ttu-id="a51d1-129">9</span><span class="sxs-lookup"><span data-stu-id="a51d1-129">9</span></span>|<span data-ttu-id="a51d1-130">Отправить push-уведомлений для устройств</span><span class="sxs-lookup"><span data-stu-id="a51d1-130">Send push notification to device</span></span>|



