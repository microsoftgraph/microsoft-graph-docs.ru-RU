---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: eabc09c8eba7267041eaf5bb318d6269373f48b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091553"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="68c6e-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="68c6e-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="68c6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68c6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68c6e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68c6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68c6e-106">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="68c6e-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="68c6e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="68c6e-107">Members</span></span>
|<span data-ttu-id="68c6e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="68c6e-108">Member</span></span>|<span data-ttu-id="68c6e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="68c6e-109">Value</span></span>|<span data-ttu-id="68c6e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="68c6e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68c6e-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="68c6e-111">userDefined</span></span>|<span data-ttu-id="68c6e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="68c6e-112">0</span></span>|<span data-ttu-id="68c6e-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="68c6e-113">Allow the user to set.</span></span>|
|<span data-ttu-id="68c6e-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="68c6e-114">httpOnly</span></span>|<span data-ttu-id="68c6e-115">1 </span><span class="sxs-lookup"><span data-stu-id="68c6e-115">1</span></span>|<span data-ttu-id="68c6e-116">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="68c6e-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="68c6e-117">хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="68c6e-117">httpWithPeeringNat</span></span>|<span data-ttu-id="68c6e-118">2 </span><span class="sxs-lookup"><span data-stu-id="68c6e-118">2</span></span>|<span data-ttu-id="68c6e-119">Операционная система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="68c6e-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="68c6e-120">хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="68c6e-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="68c6e-121">4</span><span class="sxs-lookup"><span data-stu-id="68c6e-121">3</span></span>|<span data-ttu-id="68c6e-122">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="68c6e-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="68c6e-123">хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="68c6e-123">httpWithInternetPeering</span></span>|<span data-ttu-id="68c6e-124">4 </span><span class="sxs-lookup"><span data-stu-id="68c6e-124">4</span></span>|<span data-ttu-id="68c6e-125">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="68c6e-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="68c6e-126">симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="68c6e-126">simpleDownload</span></span>|<span data-ttu-id="68c6e-127">99</span><span class="sxs-lookup"><span data-stu-id="68c6e-127">99</span></span>|<span data-ttu-id="68c6e-128">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="68c6e-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="68c6e-129">бипассмоде</span><span class="sxs-lookup"><span data-stu-id="68c6e-129">bypassMode</span></span>|<span data-ttu-id="68c6e-130">100</span><span class="sxs-lookup"><span data-stu-id="68c6e-130">100</span></span>|<span data-ttu-id="68c6e-131">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="68c6e-131">Bypass mode.</span></span> <span data-ttu-id="68c6e-132">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="68c6e-132">Do not use Delivery Optimization and use BITS instead</span></span>|









