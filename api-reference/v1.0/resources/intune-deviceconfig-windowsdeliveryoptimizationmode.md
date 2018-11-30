---
title: Тип перечисления windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для распространения peer
ms.openlocfilehash: 2d393a82f855f3e3a0226c8ccb450fa2dae1a95c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025793"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="8491d-103">Тип перечисления windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="8491d-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="8491d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8491d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8491d-105">Режим оптимизации доставки для распространения peer</span><span class="sxs-lookup"><span data-stu-id="8491d-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="8491d-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="8491d-106">Members</span></span>
|<span data-ttu-id="8491d-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="8491d-107">Member</span></span>|<span data-ttu-id="8491d-108">Значение</span><span class="sxs-lookup"><span data-stu-id="8491d-108">Value</span></span>|<span data-ttu-id="8491d-109">Description</span><span class="sxs-lookup"><span data-stu-id="8491d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8491d-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="8491d-110">userDefined</span></span>|<span data-ttu-id="8491d-111">0</span><span class="sxs-lookup"><span data-stu-id="8491d-111">0</span></span>|<span data-ttu-id="8491d-112">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="8491d-112">Allow the user to set.</span></span>|
|<span data-ttu-id="8491d-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="8491d-113">httpOnly</span></span>|<span data-ttu-id="8491d-114">1</span><span class="sxs-lookup"><span data-stu-id="8491d-114">1</span></span>|<span data-ttu-id="8491d-115">HTTP, не авторами</span><span class="sxs-lookup"><span data-stu-id="8491d-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="8491d-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="8491d-116">httpWithPeeringNat</span></span>|<span data-ttu-id="8491d-117">2</span><span class="sxs-lookup"><span data-stu-id="8491d-117">2</span></span>|<span data-ttu-id="8491d-118">Операционная система по умолчанию — Http смешиваются, авторами за же преобразования сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="8491d-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="8491d-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="8491d-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="8491d-120">3</span><span class="sxs-lookup"><span data-stu-id="8491d-120">3</span></span>|<span data-ttu-id="8491d-121">HTTP смешиваются, авторами в частной группой</span><span class="sxs-lookup"><span data-stu-id="8491d-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="8491d-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="8491d-122">httpWithInternetPeering</span></span>|<span data-ttu-id="8491d-123">4</span><span class="sxs-lookup"><span data-stu-id="8491d-123">4</span></span>|<span data-ttu-id="8491d-124">HTTP смешиваются, авторами Интернета</span><span class="sxs-lookup"><span data-stu-id="8491d-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="8491d-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="8491d-125">simpleDownload</span></span>|<span data-ttu-id="8491d-126">99</span><span class="sxs-lookup"><span data-stu-id="8491d-126">99</span></span>|<span data-ttu-id="8491d-127">Режим простой файл для загрузки с не авторами</span><span class="sxs-lookup"><span data-stu-id="8491d-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="8491d-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="8491d-128">bypassMode</span></span>|<span data-ttu-id="8491d-129">100</span><span class="sxs-lookup"><span data-stu-id="8491d-129">100</span></span>|<span data-ttu-id="8491d-130">Режим сервера-посредника.</span><span class="sxs-lookup"><span data-stu-id="8491d-130">Bypass mode.</span></span> <span data-ttu-id="8491d-131">Не используйте оптимизации доставки и вместо этого использовать бит</span><span class="sxs-lookup"><span data-stu-id="8491d-131">Do not use Delivery Optimization and use BITS instead</span></span>|



