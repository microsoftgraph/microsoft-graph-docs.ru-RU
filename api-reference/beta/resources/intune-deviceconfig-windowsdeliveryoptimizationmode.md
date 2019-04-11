---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3872b7c09c8934e95725565b83cc195d9b9d8da5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785295"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="1e0d3-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="1e0d3-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="1e0d3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e0d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e0d3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e0d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e0d3-106">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="1e0d3-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="1e0d3-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="1e0d3-107">Members</span></span>
|<span data-ttu-id="1e0d3-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="1e0d3-108">Member</span></span>|<span data-ttu-id="1e0d3-109">Значение</span><span class="sxs-lookup"><span data-stu-id="1e0d3-109">Value</span></span>|<span data-ttu-id="1e0d3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1e0d3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e0d3-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="1e0d3-111">userDefined</span></span>|<span data-ttu-id="1e0d3-112">нуль</span><span class="sxs-lookup"><span data-stu-id="1e0d3-112">0</span></span>|<span data-ttu-id="1e0d3-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="1e0d3-113">Allow the user to set.</span></span>|
|<span data-ttu-id="1e0d3-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="1e0d3-114">httpOnly</span></span>|<span data-ttu-id="1e0d3-115">1,1</span><span class="sxs-lookup"><span data-stu-id="1e0d3-115">1</span></span>|<span data-ttu-id="1e0d3-116">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="1e0d3-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="1e0d3-117">Хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="1e0d3-117">httpWithPeeringNat</span></span>|<span data-ttu-id="1e0d3-118">2</span><span class="sxs-lookup"><span data-stu-id="1e0d3-118">2</span></span>|<span data-ttu-id="1e0d3-119">ОПЕРАЦИОННАЯ система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="1e0d3-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="1e0d3-120">Хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="1e0d3-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="1e0d3-121">4</span><span class="sxs-lookup"><span data-stu-id="1e0d3-121">3</span></span>|<span data-ttu-id="1e0d3-122">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="1e0d3-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="1e0d3-123">Хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="1e0d3-123">httpWithInternetPeering</span></span>|<span data-ttu-id="1e0d3-124">SP4</span><span class="sxs-lookup"><span data-stu-id="1e0d3-124">4</span></span>|<span data-ttu-id="1e0d3-125">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="1e0d3-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="1e0d3-126">Симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="1e0d3-126">simpleDownload</span></span>|<span data-ttu-id="1e0d3-127">99</span><span class="sxs-lookup"><span data-stu-id="1e0d3-127">99</span></span>|<span data-ttu-id="1e0d3-128">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="1e0d3-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="1e0d3-129">Бипассмоде</span><span class="sxs-lookup"><span data-stu-id="1e0d3-129">bypassMode</span></span>|<span data-ttu-id="1e0d3-130">100</span><span class="sxs-lookup"><span data-stu-id="1e0d3-130">100</span></span>|<span data-ttu-id="1e0d3-131">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="1e0d3-131">Bypass mode.</span></span> <span data-ttu-id="1e0d3-132">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="1e0d3-132">Do not use Delivery Optimization and use BITS instead</span></span>|





