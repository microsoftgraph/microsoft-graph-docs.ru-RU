---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 674dd699831afd0e733adb4d436cf8d42d35a0b6
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357257"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="c717f-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="c717f-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="c717f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c717f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c717f-105">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="c717f-105">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="c717f-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="c717f-106">Members</span></span>
|<span data-ttu-id="c717f-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="c717f-107">Member</span></span>|<span data-ttu-id="c717f-108">Значение</span><span class="sxs-lookup"><span data-stu-id="c717f-108">Value</span></span>|<span data-ttu-id="c717f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c717f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c717f-110">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="c717f-110">userDefined</span></span>|<span data-ttu-id="c717f-111">нуль</span><span class="sxs-lookup"><span data-stu-id="c717f-111">0</span></span>|<span data-ttu-id="c717f-112">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="c717f-112">Allow the user to set.</span></span>|
|<span data-ttu-id="c717f-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="c717f-113">httpOnly</span></span>|<span data-ttu-id="c717f-114">1,1</span><span class="sxs-lookup"><span data-stu-id="c717f-114">1</span></span>|<span data-ttu-id="c717f-115">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="c717f-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="c717f-116">хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="c717f-116">httpWithPeeringNat</span></span>|<span data-ttu-id="c717f-117">2</span><span class="sxs-lookup"><span data-stu-id="c717f-117">2</span></span>|<span data-ttu-id="c717f-118">Операционная система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="c717f-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="c717f-119">хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="c717f-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="c717f-120">4</span><span class="sxs-lookup"><span data-stu-id="c717f-120">3</span></span>|<span data-ttu-id="c717f-121">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="c717f-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="c717f-122">хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="c717f-122">httpWithInternetPeering</span></span>|<span data-ttu-id="c717f-123">SP4</span><span class="sxs-lookup"><span data-stu-id="c717f-123">4</span></span>|<span data-ttu-id="c717f-124">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="c717f-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="c717f-125">симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="c717f-125">simpleDownload</span></span>|<span data-ttu-id="c717f-126">99</span><span class="sxs-lookup"><span data-stu-id="c717f-126">99</span></span>|<span data-ttu-id="c717f-127">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="c717f-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="c717f-128">бипассмоде</span><span class="sxs-lookup"><span data-stu-id="c717f-128">bypassMode</span></span>|<span data-ttu-id="c717f-129">100</span><span class="sxs-lookup"><span data-stu-id="c717f-129">100</span></span>|<span data-ttu-id="c717f-130">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="c717f-130">Bypass mode.</span></span> <span data-ttu-id="c717f-131">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="c717f-131">Do not use Delivery Optimization and use BITS instead</span></span>|




