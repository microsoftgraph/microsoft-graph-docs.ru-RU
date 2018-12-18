---
title: Тип перечисления windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для распространения peer
author: tfitzmac
ms.openlocfilehash: ae61d7dde5fc02ff329eaf9cc970ee7078c3a254
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360160"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="7d166-103">Тип перечисления windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="7d166-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="7d166-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7d166-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d166-105">Режим оптимизации доставки для распространения peer</span><span class="sxs-lookup"><span data-stu-id="7d166-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="7d166-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="7d166-106">Members</span></span>
|<span data-ttu-id="7d166-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="7d166-107">Member</span></span>|<span data-ttu-id="7d166-108">Значение</span><span class="sxs-lookup"><span data-stu-id="7d166-108">Value</span></span>|<span data-ttu-id="7d166-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7d166-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d166-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="7d166-110">userDefined</span></span>|<span data-ttu-id="7d166-111">0</span><span class="sxs-lookup"><span data-stu-id="7d166-111">0</span></span>|<span data-ttu-id="7d166-112">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="7d166-112">Allow the user to set.</span></span>|
|<span data-ttu-id="7d166-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="7d166-113">httpOnly</span></span>|<span data-ttu-id="7d166-114">1</span><span class="sxs-lookup"><span data-stu-id="7d166-114">1</span></span>|<span data-ttu-id="7d166-115">HTTP, не авторами</span><span class="sxs-lookup"><span data-stu-id="7d166-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="7d166-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="7d166-116">httpWithPeeringNat</span></span>|<span data-ttu-id="7d166-117">2</span><span class="sxs-lookup"><span data-stu-id="7d166-117">2</span></span>|<span data-ttu-id="7d166-118">Операционная система по умолчанию — Http смешиваются, авторами за же преобразования сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="7d166-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="7d166-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="7d166-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="7d166-120">3</span><span class="sxs-lookup"><span data-stu-id="7d166-120">3</span></span>|<span data-ttu-id="7d166-121">HTTP смешиваются, авторами в частной группой</span><span class="sxs-lookup"><span data-stu-id="7d166-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="7d166-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="7d166-122">httpWithInternetPeering</span></span>|<span data-ttu-id="7d166-123">4</span><span class="sxs-lookup"><span data-stu-id="7d166-123">4</span></span>|<span data-ttu-id="7d166-124">HTTP смешиваются, авторами Интернета</span><span class="sxs-lookup"><span data-stu-id="7d166-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="7d166-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="7d166-125">simpleDownload</span></span>|<span data-ttu-id="7d166-126">99</span><span class="sxs-lookup"><span data-stu-id="7d166-126">99</span></span>|<span data-ttu-id="7d166-127">Режим простой файл для загрузки с не авторами</span><span class="sxs-lookup"><span data-stu-id="7d166-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="7d166-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="7d166-128">bypassMode</span></span>|<span data-ttu-id="7d166-129">100</span><span class="sxs-lookup"><span data-stu-id="7d166-129">100</span></span>|<span data-ttu-id="7d166-130">Режим сервера-посредника.</span><span class="sxs-lookup"><span data-stu-id="7d166-130">Bypass mode.</span></span> <span data-ttu-id="7d166-131">Не используйте оптимизации доставки и вместо этого использовать бит</span><span class="sxs-lookup"><span data-stu-id="7d166-131">Do not use Delivery Optimization and use BITS instead</span></span>|



