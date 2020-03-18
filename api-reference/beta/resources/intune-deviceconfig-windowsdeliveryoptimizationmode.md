---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: faf70d8cb1122b09d5fcc6a5dcbf221cf3a6991c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786518"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="4142e-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="4142e-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="4142e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4142e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4142e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4142e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4142e-106">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="4142e-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="4142e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4142e-107">Members</span></span>
|<span data-ttu-id="4142e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4142e-108">Member</span></span>|<span data-ttu-id="4142e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4142e-109">Value</span></span>|<span data-ttu-id="4142e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4142e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4142e-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="4142e-111">userDefined</span></span>|<span data-ttu-id="4142e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4142e-112">0</span></span>|<span data-ttu-id="4142e-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="4142e-113">Allow the user to set.</span></span>|
|<span data-ttu-id="4142e-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="4142e-114">httpOnly</span></span>|<span data-ttu-id="4142e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="4142e-115">1</span></span>|<span data-ttu-id="4142e-116">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="4142e-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="4142e-117">хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="4142e-117">httpWithPeeringNat</span></span>|<span data-ttu-id="4142e-118">2</span><span class="sxs-lookup"><span data-stu-id="4142e-118">2</span></span>|<span data-ttu-id="4142e-119">Операционная система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="4142e-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="4142e-120">хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="4142e-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="4142e-121">4</span><span class="sxs-lookup"><span data-stu-id="4142e-121">3</span></span>|<span data-ttu-id="4142e-122">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="4142e-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="4142e-123">хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="4142e-123">httpWithInternetPeering</span></span>|<span data-ttu-id="4142e-124">4 </span><span class="sxs-lookup"><span data-stu-id="4142e-124">4</span></span>|<span data-ttu-id="4142e-125">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="4142e-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="4142e-126">симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="4142e-126">simpleDownload</span></span>|<span data-ttu-id="4142e-127">99</span><span class="sxs-lookup"><span data-stu-id="4142e-127">99</span></span>|<span data-ttu-id="4142e-128">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="4142e-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="4142e-129">бипассмоде</span><span class="sxs-lookup"><span data-stu-id="4142e-129">bypassMode</span></span>|<span data-ttu-id="4142e-130">100</span><span class="sxs-lookup"><span data-stu-id="4142e-130">100</span></span>|<span data-ttu-id="4142e-131">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="4142e-131">Bypass mode.</span></span> <span data-ttu-id="4142e-132">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="4142e-132">Do not use Delivery Optimization and use BITS instead</span></span>|



