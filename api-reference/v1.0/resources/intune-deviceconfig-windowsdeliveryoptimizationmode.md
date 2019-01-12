---
title: Тип перечисления windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для распространения peer
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f80c6b5cbe7316c851954154bdb559f370f02b79
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951518"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="93f4a-103">Тип перечисления windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="93f4a-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="93f4a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="93f4a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93f4a-105">Режим оптимизации доставки для распространения peer</span><span class="sxs-lookup"><span data-stu-id="93f4a-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="93f4a-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="93f4a-106">Members</span></span>
|<span data-ttu-id="93f4a-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="93f4a-107">Member</span></span>|<span data-ttu-id="93f4a-108">Значение</span><span class="sxs-lookup"><span data-stu-id="93f4a-108">Value</span></span>|<span data-ttu-id="93f4a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="93f4a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93f4a-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="93f4a-110">userDefined</span></span>|<span data-ttu-id="93f4a-111">0</span><span class="sxs-lookup"><span data-stu-id="93f4a-111">0</span></span>|<span data-ttu-id="93f4a-112">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="93f4a-112">Allow the user to set.</span></span>|
|<span data-ttu-id="93f4a-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="93f4a-113">httpOnly</span></span>|<span data-ttu-id="93f4a-114">1</span><span class="sxs-lookup"><span data-stu-id="93f4a-114">1</span></span>|<span data-ttu-id="93f4a-115">HTTP, не авторами</span><span class="sxs-lookup"><span data-stu-id="93f4a-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="93f4a-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="93f4a-116">httpWithPeeringNat</span></span>|<span data-ttu-id="93f4a-117">2</span><span class="sxs-lookup"><span data-stu-id="93f4a-117">2</span></span>|<span data-ttu-id="93f4a-118">Операционная система по умолчанию — Http смешиваются, авторами за же преобразования сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="93f4a-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="93f4a-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="93f4a-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="93f4a-120">3</span><span class="sxs-lookup"><span data-stu-id="93f4a-120">3</span></span>|<span data-ttu-id="93f4a-121">HTTP смешиваются, авторами в частной группой</span><span class="sxs-lookup"><span data-stu-id="93f4a-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="93f4a-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="93f4a-122">httpWithInternetPeering</span></span>|<span data-ttu-id="93f4a-123">4</span><span class="sxs-lookup"><span data-stu-id="93f4a-123">4</span></span>|<span data-ttu-id="93f4a-124">HTTP смешиваются, авторами Интернета</span><span class="sxs-lookup"><span data-stu-id="93f4a-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="93f4a-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="93f4a-125">simpleDownload</span></span>|<span data-ttu-id="93f4a-126">99</span><span class="sxs-lookup"><span data-stu-id="93f4a-126">99</span></span>|<span data-ttu-id="93f4a-127">Режим простой файл для загрузки с не авторами</span><span class="sxs-lookup"><span data-stu-id="93f4a-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="93f4a-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="93f4a-128">bypassMode</span></span>|<span data-ttu-id="93f4a-129">100</span><span class="sxs-lookup"><span data-stu-id="93f4a-129">100</span></span>|<span data-ttu-id="93f4a-130">Режим сервера-посредника.</span><span class="sxs-lookup"><span data-stu-id="93f4a-130">Bypass mode.</span></span> <span data-ttu-id="93f4a-131">Не используйте оптимизации доставки и вместо этого использовать бит</span><span class="sxs-lookup"><span data-stu-id="93f4a-131">Do not use Delivery Optimization and use BITS instead</span></span>|



