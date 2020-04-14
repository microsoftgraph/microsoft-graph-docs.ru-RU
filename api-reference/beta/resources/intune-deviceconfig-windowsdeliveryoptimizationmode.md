---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 71bc7e364ca18fefe9ebc5fa5ed75d5dac485a01
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411914"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="ed929-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="ed929-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="ed929-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed929-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed929-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed929-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed929-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed929-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed929-107">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="ed929-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="ed929-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ed929-108">Members</span></span>
|<span data-ttu-id="ed929-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ed929-109">Member</span></span>|<span data-ttu-id="ed929-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ed929-110">Value</span></span>|<span data-ttu-id="ed929-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ed929-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed929-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="ed929-112">userDefined</span></span>|<span data-ttu-id="ed929-113">нуль</span><span class="sxs-lookup"><span data-stu-id="ed929-113">0</span></span>|<span data-ttu-id="ed929-114">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="ed929-114">Allow the user to set.</span></span>|
|<span data-ttu-id="ed929-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="ed929-115">httpOnly</span></span>|<span data-ttu-id="ed929-116">1,1</span><span class="sxs-lookup"><span data-stu-id="ed929-116">1</span></span>|<span data-ttu-id="ed929-117">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="ed929-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="ed929-118">хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="ed929-118">httpWithPeeringNat</span></span>|<span data-ttu-id="ed929-119">2</span><span class="sxs-lookup"><span data-stu-id="ed929-119">2</span></span>|<span data-ttu-id="ed929-120">Операционная система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="ed929-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="ed929-121">хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="ed929-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="ed929-122">4</span><span class="sxs-lookup"><span data-stu-id="ed929-122">3</span></span>|<span data-ttu-id="ed929-123">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="ed929-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="ed929-124">хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="ed929-124">httpWithInternetPeering</span></span>|<span data-ttu-id="ed929-125">4 </span><span class="sxs-lookup"><span data-stu-id="ed929-125">4</span></span>|<span data-ttu-id="ed929-126">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="ed929-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="ed929-127">симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="ed929-127">simpleDownload</span></span>|<span data-ttu-id="ed929-128">99</span><span class="sxs-lookup"><span data-stu-id="ed929-128">99</span></span>|<span data-ttu-id="ed929-129">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="ed929-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="ed929-130">бипассмоде</span><span class="sxs-lookup"><span data-stu-id="ed929-130">bypassMode</span></span>|<span data-ttu-id="ed929-131">100</span><span class="sxs-lookup"><span data-stu-id="ed929-131">100</span></span>|<span data-ttu-id="ed929-132">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="ed929-132">Bypass mode.</span></span> <span data-ttu-id="ed929-133">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="ed929-133">Do not use Delivery Optimization and use BITS instead</span></span>|



