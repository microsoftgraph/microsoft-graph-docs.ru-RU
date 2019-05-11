---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e020b4f32cc9075acab6c783b4e9df3eb19a438b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944126"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="2768e-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="2768e-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="2768e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2768e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2768e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2768e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2768e-106">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="2768e-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="2768e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="2768e-107">Members</span></span>
|<span data-ttu-id="2768e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="2768e-108">Member</span></span>|<span data-ttu-id="2768e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="2768e-109">Value</span></span>|<span data-ttu-id="2768e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2768e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2768e-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="2768e-111">userDefined</span></span>|<span data-ttu-id="2768e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="2768e-112">0</span></span>|<span data-ttu-id="2768e-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="2768e-113">Allow the user to set.</span></span>|
|<span data-ttu-id="2768e-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="2768e-114">httpOnly</span></span>|<span data-ttu-id="2768e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="2768e-115">1</span></span>|<span data-ttu-id="2768e-116">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="2768e-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="2768e-117">Хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="2768e-117">httpWithPeeringNat</span></span>|<span data-ttu-id="2768e-118">2</span><span class="sxs-lookup"><span data-stu-id="2768e-118">2</span></span>|<span data-ttu-id="2768e-119">ОПЕРАЦИОННАЯ система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="2768e-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="2768e-120">Хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="2768e-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="2768e-121">4</span><span class="sxs-lookup"><span data-stu-id="2768e-121">3</span></span>|<span data-ttu-id="2768e-122">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="2768e-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="2768e-123">Хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="2768e-123">httpWithInternetPeering</span></span>|<span data-ttu-id="2768e-124">SP4</span><span class="sxs-lookup"><span data-stu-id="2768e-124">4</span></span>|<span data-ttu-id="2768e-125">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="2768e-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="2768e-126">Симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="2768e-126">simpleDownload</span></span>|<span data-ttu-id="2768e-127">99</span><span class="sxs-lookup"><span data-stu-id="2768e-127">99</span></span>|<span data-ttu-id="2768e-128">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="2768e-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="2768e-129">Бипассмоде</span><span class="sxs-lookup"><span data-stu-id="2768e-129">bypassMode</span></span>|<span data-ttu-id="2768e-130">100</span><span class="sxs-lookup"><span data-stu-id="2768e-130">100</span></span>|<span data-ttu-id="2768e-131">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="2768e-131">Bypass mode.</span></span> <span data-ttu-id="2768e-132">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="2768e-132">Do not use Delivery Optimization and use BITS instead</span></span>|




