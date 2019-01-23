---
title: Тип перечисления windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для распространения peer
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5565965f9ba9395d7cd07b2935e6772478e0bb50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406887"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="762a4-103">Тип перечисления windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="762a4-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="762a4-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="762a4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="762a4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="762a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="762a4-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="762a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="762a4-107">Режим оптимизации доставки для распространения peer</span><span class="sxs-lookup"><span data-stu-id="762a4-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="762a4-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="762a4-108">Members</span></span>
|<span data-ttu-id="762a4-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="762a4-109">Member</span></span>|<span data-ttu-id="762a4-110">Значение</span><span class="sxs-lookup"><span data-stu-id="762a4-110">Value</span></span>|<span data-ttu-id="762a4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="762a4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="762a4-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="762a4-112">userDefined</span></span>|<span data-ttu-id="762a4-113">0</span><span class="sxs-lookup"><span data-stu-id="762a4-113">0</span></span>|<span data-ttu-id="762a4-114">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="762a4-114">Allow the user to set.</span></span>|
|<span data-ttu-id="762a4-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="762a4-115">httpOnly</span></span>|<span data-ttu-id="762a4-116">1</span><span class="sxs-lookup"><span data-stu-id="762a4-116">1</span></span>|<span data-ttu-id="762a4-117">HTTP, не авторами</span><span class="sxs-lookup"><span data-stu-id="762a4-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="762a4-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="762a4-118">httpWithPeeringNat</span></span>|<span data-ttu-id="762a4-119">2</span><span class="sxs-lookup"><span data-stu-id="762a4-119">2</span></span>|<span data-ttu-id="762a4-120">Операционная система по умолчанию — Http смешиваются, авторами за же преобразования сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="762a4-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="762a4-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="762a4-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="762a4-122">3</span><span class="sxs-lookup"><span data-stu-id="762a4-122">3</span></span>|<span data-ttu-id="762a4-123">HTTP смешиваются, авторами в частной группой</span><span class="sxs-lookup"><span data-stu-id="762a4-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="762a4-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="762a4-124">httpWithInternetPeering</span></span>|<span data-ttu-id="762a4-125">4</span><span class="sxs-lookup"><span data-stu-id="762a4-125">4</span></span>|<span data-ttu-id="762a4-126">HTTP смешиваются, авторами Интернета</span><span class="sxs-lookup"><span data-stu-id="762a4-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="762a4-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="762a4-127">simpleDownload</span></span>|<span data-ttu-id="762a4-128">99</span><span class="sxs-lookup"><span data-stu-id="762a4-128">99</span></span>|<span data-ttu-id="762a4-129">Режим простой файл для загрузки с не авторами</span><span class="sxs-lookup"><span data-stu-id="762a4-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="762a4-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="762a4-130">bypassMode</span></span>|<span data-ttu-id="762a4-131">100</span><span class="sxs-lookup"><span data-stu-id="762a4-131">100</span></span>|<span data-ttu-id="762a4-132">Режим сервера-посредника.</span><span class="sxs-lookup"><span data-stu-id="762a4-132">Bypass mode.</span></span> <span data-ttu-id="762a4-133">Не используйте оптимизации доставки и вместо этого использовать бит</span><span class="sxs-lookup"><span data-stu-id="762a4-133">Do not use Delivery Optimization and use BITS instead</span></span>|




