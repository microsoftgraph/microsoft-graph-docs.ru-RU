---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e3b32f3a6480b236297a7d0217c9aed8eefd5c44
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084459"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="65918-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="65918-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="65918-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65918-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65918-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65918-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65918-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65918-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65918-107">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="65918-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="65918-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="65918-108">Members</span></span>
|<span data-ttu-id="65918-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="65918-109">Member</span></span>|<span data-ttu-id="65918-110">Значение</span><span class="sxs-lookup"><span data-stu-id="65918-110">Value</span></span>|<span data-ttu-id="65918-111">Описание</span><span class="sxs-lookup"><span data-stu-id="65918-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65918-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="65918-112">userDefined</span></span>|<span data-ttu-id="65918-113">нуль</span><span class="sxs-lookup"><span data-stu-id="65918-113">0</span></span>|<span data-ttu-id="65918-114">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="65918-114">Allow the user to set.</span></span>|
|<span data-ttu-id="65918-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="65918-115">httpOnly</span></span>|<span data-ttu-id="65918-116">1 </span><span class="sxs-lookup"><span data-stu-id="65918-116">1</span></span>|<span data-ttu-id="65918-117">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="65918-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="65918-118">хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="65918-118">httpWithPeeringNat</span></span>|<span data-ttu-id="65918-119">2 </span><span class="sxs-lookup"><span data-stu-id="65918-119">2</span></span>|<span data-ttu-id="65918-120">Операционная система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="65918-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="65918-121">хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="65918-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="65918-122">4</span><span class="sxs-lookup"><span data-stu-id="65918-122">3</span></span>|<span data-ttu-id="65918-123">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="65918-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="65918-124">хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="65918-124">httpWithInternetPeering</span></span>|<span data-ttu-id="65918-125">4 </span><span class="sxs-lookup"><span data-stu-id="65918-125">4</span></span>|<span data-ttu-id="65918-126">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="65918-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="65918-127">симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="65918-127">simpleDownload</span></span>|<span data-ttu-id="65918-128">99</span><span class="sxs-lookup"><span data-stu-id="65918-128">99</span></span>|<span data-ttu-id="65918-129">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="65918-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="65918-130">бипассмоде</span><span class="sxs-lookup"><span data-stu-id="65918-130">bypassMode</span></span>|<span data-ttu-id="65918-131">100</span><span class="sxs-lookup"><span data-stu-id="65918-131">100</span></span>|<span data-ttu-id="65918-132">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="65918-132">Bypass mode.</span></span> <span data-ttu-id="65918-133">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="65918-133">Do not use Delivery Optimization and use BITS instead</span></span>|






