---
title: Тип перечисления windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для распространения peer
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af266b55fd58f788965d33d0d807511d263f6195
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888181"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="791d1-103">Тип перечисления windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="791d1-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="791d1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="791d1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="791d1-105">Режим оптимизации доставки для распространения peer</span><span class="sxs-lookup"><span data-stu-id="791d1-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="791d1-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="791d1-106">Members</span></span>
|<span data-ttu-id="791d1-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="791d1-107">Member</span></span>|<span data-ttu-id="791d1-108">Значение</span><span class="sxs-lookup"><span data-stu-id="791d1-108">Value</span></span>|<span data-ttu-id="791d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="791d1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="791d1-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="791d1-110">userDefined</span></span>|<span data-ttu-id="791d1-111">0</span><span class="sxs-lookup"><span data-stu-id="791d1-111">0</span></span>|<span data-ttu-id="791d1-112">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="791d1-112">Allow the user to set.</span></span>|
|<span data-ttu-id="791d1-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="791d1-113">httpOnly</span></span>|<span data-ttu-id="791d1-114">1</span><span class="sxs-lookup"><span data-stu-id="791d1-114">1</span></span>|<span data-ttu-id="791d1-115">HTTP, не авторами</span><span class="sxs-lookup"><span data-stu-id="791d1-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="791d1-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="791d1-116">httpWithPeeringNat</span></span>|<span data-ttu-id="791d1-117">2</span><span class="sxs-lookup"><span data-stu-id="791d1-117">2</span></span>|<span data-ttu-id="791d1-118">Операционная система по умолчанию — Http смешиваются, авторами за же преобразования сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="791d1-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="791d1-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="791d1-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="791d1-120">3</span><span class="sxs-lookup"><span data-stu-id="791d1-120">3</span></span>|<span data-ttu-id="791d1-121">HTTP смешиваются, авторами в частной группой</span><span class="sxs-lookup"><span data-stu-id="791d1-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="791d1-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="791d1-122">httpWithInternetPeering</span></span>|<span data-ttu-id="791d1-123">4</span><span class="sxs-lookup"><span data-stu-id="791d1-123">4</span></span>|<span data-ttu-id="791d1-124">HTTP смешиваются, авторами Интернета</span><span class="sxs-lookup"><span data-stu-id="791d1-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="791d1-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="791d1-125">simpleDownload</span></span>|<span data-ttu-id="791d1-126">99</span><span class="sxs-lookup"><span data-stu-id="791d1-126">99</span></span>|<span data-ttu-id="791d1-127">Режим простой файл для загрузки с не авторами</span><span class="sxs-lookup"><span data-stu-id="791d1-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="791d1-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="791d1-128">bypassMode</span></span>|<span data-ttu-id="791d1-129">100</span><span class="sxs-lookup"><span data-stu-id="791d1-129">100</span></span>|<span data-ttu-id="791d1-130">Режим сервера-посредника.</span><span class="sxs-lookup"><span data-stu-id="791d1-130">Bypass mode.</span></span> <span data-ttu-id="791d1-131">Не используйте оптимизации доставки и вместо этого использовать бит</span><span class="sxs-lookup"><span data-stu-id="791d1-131">Do not use Delivery Optimization and use BITS instead</span></span>|



