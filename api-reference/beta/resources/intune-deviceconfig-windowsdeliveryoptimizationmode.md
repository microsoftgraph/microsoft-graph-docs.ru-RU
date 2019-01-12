---
title: Тип перечисления windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для распространения peer
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 004bb3d3984d8d304f89dc339899035d218546a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972658"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="4bb74-103">Тип перечисления windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="4bb74-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="4bb74-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4bb74-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bb74-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb74-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4bb74-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4bb74-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4bb74-107">Режим оптимизации доставки для распространения peer</span><span class="sxs-lookup"><span data-stu-id="4bb74-107">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="4bb74-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4bb74-108">Members</span></span>
|<span data-ttu-id="4bb74-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4bb74-109">Member</span></span>|<span data-ttu-id="4bb74-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4bb74-110">Value</span></span>|<span data-ttu-id="4bb74-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4bb74-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bb74-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="4bb74-112">userDefined</span></span>|<span data-ttu-id="4bb74-113">0</span><span class="sxs-lookup"><span data-stu-id="4bb74-113">0</span></span>|<span data-ttu-id="4bb74-114">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="4bb74-114">Allow the user to set.</span></span>|
|<span data-ttu-id="4bb74-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="4bb74-115">httpOnly</span></span>|<span data-ttu-id="4bb74-116">1</span><span class="sxs-lookup"><span data-stu-id="4bb74-116">1</span></span>|<span data-ttu-id="4bb74-117">HTTP, не авторами</span><span class="sxs-lookup"><span data-stu-id="4bb74-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="4bb74-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="4bb74-118">httpWithPeeringNat</span></span>|<span data-ttu-id="4bb74-119">2</span><span class="sxs-lookup"><span data-stu-id="4bb74-119">2</span></span>|<span data-ttu-id="4bb74-120">Операционная система по умолчанию — Http смешиваются, авторами за же преобразования сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="4bb74-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="4bb74-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="4bb74-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="4bb74-122">3</span><span class="sxs-lookup"><span data-stu-id="4bb74-122">3</span></span>|<span data-ttu-id="4bb74-123">HTTP смешиваются, авторами в частной группой</span><span class="sxs-lookup"><span data-stu-id="4bb74-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="4bb74-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="4bb74-124">httpWithInternetPeering</span></span>|<span data-ttu-id="4bb74-125">4</span><span class="sxs-lookup"><span data-stu-id="4bb74-125">4</span></span>|<span data-ttu-id="4bb74-126">HTTP смешиваются, авторами Интернета</span><span class="sxs-lookup"><span data-stu-id="4bb74-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="4bb74-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="4bb74-127">simpleDownload</span></span>|<span data-ttu-id="4bb74-128">99</span><span class="sxs-lookup"><span data-stu-id="4bb74-128">99</span></span>|<span data-ttu-id="4bb74-129">Режим простой файл для загрузки с не авторами</span><span class="sxs-lookup"><span data-stu-id="4bb74-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="4bb74-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="4bb74-130">bypassMode</span></span>|<span data-ttu-id="4bb74-131">100</span><span class="sxs-lookup"><span data-stu-id="4bb74-131">100</span></span>|<span data-ttu-id="4bb74-132">Режим сервера-посредника.</span><span class="sxs-lookup"><span data-stu-id="4bb74-132">Bypass mode.</span></span> <span data-ttu-id="4bb74-133">Не используйте оптимизации доставки и вместо этого использовать бит</span><span class="sxs-lookup"><span data-stu-id="4bb74-133">Do not use Delivery Optimization and use BITS instead</span></span>|





