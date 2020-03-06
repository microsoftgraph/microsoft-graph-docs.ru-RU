---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 869c902e8fc0b02fed1037d1d1273d8584ece9fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530368"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="94d2e-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="94d2e-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="94d2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94d2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94d2e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94d2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94d2e-106">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="94d2e-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="94d2e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="94d2e-107">Members</span></span>
|<span data-ttu-id="94d2e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="94d2e-108">Member</span></span>|<span data-ttu-id="94d2e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="94d2e-109">Value</span></span>|<span data-ttu-id="94d2e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="94d2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94d2e-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="94d2e-111">userDefined</span></span>|<span data-ttu-id="94d2e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="94d2e-112">0</span></span>|<span data-ttu-id="94d2e-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="94d2e-113">Allow the user to set.</span></span>|
|<span data-ttu-id="94d2e-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="94d2e-114">httpOnly</span></span>|<span data-ttu-id="94d2e-115">1 </span><span class="sxs-lookup"><span data-stu-id="94d2e-115">1</span></span>|<span data-ttu-id="94d2e-116">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="94d2e-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="94d2e-117">хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="94d2e-117">httpWithPeeringNat</span></span>|<span data-ttu-id="94d2e-118">2 </span><span class="sxs-lookup"><span data-stu-id="94d2e-118">2</span></span>|<span data-ttu-id="94d2e-119">Операционная система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="94d2e-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="94d2e-120">хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="94d2e-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="94d2e-121">3 </span><span class="sxs-lookup"><span data-stu-id="94d2e-121">3</span></span>|<span data-ttu-id="94d2e-122">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="94d2e-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="94d2e-123">хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="94d2e-123">httpWithInternetPeering</span></span>|<span data-ttu-id="94d2e-124">4 </span><span class="sxs-lookup"><span data-stu-id="94d2e-124">4</span></span>|<span data-ttu-id="94d2e-125">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="94d2e-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="94d2e-126">симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="94d2e-126">simpleDownload</span></span>|<span data-ttu-id="94d2e-127">99</span><span class="sxs-lookup"><span data-stu-id="94d2e-127">99</span></span>|<span data-ttu-id="94d2e-128">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="94d2e-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="94d2e-129">бипассмоде</span><span class="sxs-lookup"><span data-stu-id="94d2e-129">bypassMode</span></span>|<span data-ttu-id="94d2e-130">100</span><span class="sxs-lookup"><span data-stu-id="94d2e-130">100</span></span>|<span data-ttu-id="94d2e-131">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="94d2e-131">Bypass mode.</span></span> <span data-ttu-id="94d2e-132">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="94d2e-132">Do not use Delivery Optimization and use BITS instead</span></span>|




