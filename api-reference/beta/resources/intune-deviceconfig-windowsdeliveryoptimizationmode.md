---
title: Тип перечисления windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для распространения peer
ms.openlocfilehash: 99795f3d901b538990d4dfec7a426e66794c5946
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077245"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="4f92c-103">Тип перечисления windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="4f92c-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="4f92c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4f92c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f92c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f92c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f92c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4f92c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f92c-107">Режим оптимизации доставки для распространения peer</span><span class="sxs-lookup"><span data-stu-id="4f92c-107">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="4f92c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4f92c-108">Members</span></span>
|<span data-ttu-id="4f92c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4f92c-109">Member</span></span>|<span data-ttu-id="4f92c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4f92c-110">Value</span></span>|<span data-ttu-id="4f92c-111">Description</span><span class="sxs-lookup"><span data-stu-id="4f92c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f92c-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="4f92c-112">userDefined</span></span>|<span data-ttu-id="4f92c-113">0</span><span class="sxs-lookup"><span data-stu-id="4f92c-113">0</span></span>|<span data-ttu-id="4f92c-114">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="4f92c-114">Allow the user to set.</span></span>|
|<span data-ttu-id="4f92c-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="4f92c-115">httpOnly</span></span>|<span data-ttu-id="4f92c-116">1</span><span class="sxs-lookup"><span data-stu-id="4f92c-116">1</span></span>|<span data-ttu-id="4f92c-117">HTTP, не авторами</span><span class="sxs-lookup"><span data-stu-id="4f92c-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="4f92c-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="4f92c-118">httpWithPeeringNat</span></span>|<span data-ttu-id="4f92c-119">2</span><span class="sxs-lookup"><span data-stu-id="4f92c-119">2</span></span>|<span data-ttu-id="4f92c-120">Операционная система по умолчанию — Http смешиваются, авторами за же преобразования сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="4f92c-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="4f92c-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="4f92c-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="4f92c-122">3</span><span class="sxs-lookup"><span data-stu-id="4f92c-122">3</span></span>|<span data-ttu-id="4f92c-123">HTTP смешиваются, авторами в частной группой</span><span class="sxs-lookup"><span data-stu-id="4f92c-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="4f92c-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="4f92c-124">httpWithInternetPeering</span></span>|<span data-ttu-id="4f92c-125">4</span><span class="sxs-lookup"><span data-stu-id="4f92c-125">4</span></span>|<span data-ttu-id="4f92c-126">HTTP смешиваются, авторами Интернета</span><span class="sxs-lookup"><span data-stu-id="4f92c-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="4f92c-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="4f92c-127">simpleDownload</span></span>|<span data-ttu-id="4f92c-128">99</span><span class="sxs-lookup"><span data-stu-id="4f92c-128">99</span></span>|<span data-ttu-id="4f92c-129">Режим простой файл для загрузки с не авторами</span><span class="sxs-lookup"><span data-stu-id="4f92c-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="4f92c-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="4f92c-130">bypassMode</span></span>|<span data-ttu-id="4f92c-131">100</span><span class="sxs-lookup"><span data-stu-id="4f92c-131">100</span></span>|<span data-ttu-id="4f92c-132">Режим сервера-посредника.</span><span class="sxs-lookup"><span data-stu-id="4f92c-132">Bypass mode.</span></span> <span data-ttu-id="4f92c-133">Не используйте оптимизации доставки и вместо этого использовать бит</span><span class="sxs-lookup"><span data-stu-id="4f92c-133">Do not use Delivery Optimization and use BITS instead</span></span>|





