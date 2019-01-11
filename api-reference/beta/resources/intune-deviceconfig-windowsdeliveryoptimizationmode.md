---
title: Тип перечисления windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для распространения peer
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e62416328e596737c36d920d6877773c905680c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807723"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="acb1a-103">Тип перечисления windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="acb1a-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="acb1a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="acb1a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acb1a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acb1a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="acb1a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="acb1a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acb1a-107">Режим оптимизации доставки для распространения peer</span><span class="sxs-lookup"><span data-stu-id="acb1a-107">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="acb1a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="acb1a-108">Members</span></span>
|<span data-ttu-id="acb1a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="acb1a-109">Member</span></span>|<span data-ttu-id="acb1a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="acb1a-110">Value</span></span>|<span data-ttu-id="acb1a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="acb1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acb1a-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="acb1a-112">userDefined</span></span>|<span data-ttu-id="acb1a-113">0</span><span class="sxs-lookup"><span data-stu-id="acb1a-113">0</span></span>|<span data-ttu-id="acb1a-114">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="acb1a-114">Allow the user to set.</span></span>|
|<span data-ttu-id="acb1a-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="acb1a-115">httpOnly</span></span>|<span data-ttu-id="acb1a-116">1</span><span class="sxs-lookup"><span data-stu-id="acb1a-116">1</span></span>|<span data-ttu-id="acb1a-117">HTTP, не авторами</span><span class="sxs-lookup"><span data-stu-id="acb1a-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="acb1a-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="acb1a-118">httpWithPeeringNat</span></span>|<span data-ttu-id="acb1a-119">2</span><span class="sxs-lookup"><span data-stu-id="acb1a-119">2</span></span>|<span data-ttu-id="acb1a-120">Операционная система по умолчанию — Http смешиваются, авторами за же преобразования сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="acb1a-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="acb1a-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="acb1a-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="acb1a-122">3</span><span class="sxs-lookup"><span data-stu-id="acb1a-122">3</span></span>|<span data-ttu-id="acb1a-123">HTTP смешиваются, авторами в частной группой</span><span class="sxs-lookup"><span data-stu-id="acb1a-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="acb1a-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="acb1a-124">httpWithInternetPeering</span></span>|<span data-ttu-id="acb1a-125">4</span><span class="sxs-lookup"><span data-stu-id="acb1a-125">4</span></span>|<span data-ttu-id="acb1a-126">HTTP смешиваются, авторами Интернета</span><span class="sxs-lookup"><span data-stu-id="acb1a-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="acb1a-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="acb1a-127">simpleDownload</span></span>|<span data-ttu-id="acb1a-128">99</span><span class="sxs-lookup"><span data-stu-id="acb1a-128">99</span></span>|<span data-ttu-id="acb1a-129">Режим простой файл для загрузки с не авторами</span><span class="sxs-lookup"><span data-stu-id="acb1a-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="acb1a-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="acb1a-130">bypassMode</span></span>|<span data-ttu-id="acb1a-131">100</span><span class="sxs-lookup"><span data-stu-id="acb1a-131">100</span></span>|<span data-ttu-id="acb1a-132">Режим сервера-посредника.</span><span class="sxs-lookup"><span data-stu-id="acb1a-132">Bypass mode.</span></span> <span data-ttu-id="acb1a-133">Не используйте оптимизации доставки и вместо этого использовать бит</span><span class="sxs-lookup"><span data-stu-id="acb1a-133">Do not use Delivery Optimization and use BITS instead</span></span>|





