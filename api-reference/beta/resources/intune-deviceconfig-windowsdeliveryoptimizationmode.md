---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c24689f5690d3bd6d507c1ebb4fae36d010ee26d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268337"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="c40e2-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="c40e2-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="c40e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c40e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c40e2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c40e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c40e2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c40e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c40e2-107">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="c40e2-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="c40e2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c40e2-108">Members</span></span>
|<span data-ttu-id="c40e2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c40e2-109">Member</span></span>|<span data-ttu-id="c40e2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c40e2-110">Value</span></span>|<span data-ttu-id="c40e2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c40e2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c40e2-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="c40e2-112">userDefined</span></span>|<span data-ttu-id="c40e2-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c40e2-113">0</span></span>|<span data-ttu-id="c40e2-114">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="c40e2-114">Allow the user to set.</span></span>|
|<span data-ttu-id="c40e2-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="c40e2-115">httpOnly</span></span>|<span data-ttu-id="c40e2-116">1,1</span><span class="sxs-lookup"><span data-stu-id="c40e2-116">1</span></span>|<span data-ttu-id="c40e2-117">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="c40e2-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="c40e2-118">хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="c40e2-118">httpWithPeeringNat</span></span>|<span data-ttu-id="c40e2-119">2</span><span class="sxs-lookup"><span data-stu-id="c40e2-119">2</span></span>|<span data-ttu-id="c40e2-120">Операционная система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="c40e2-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="c40e2-121">хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="c40e2-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="c40e2-122">4</span><span class="sxs-lookup"><span data-stu-id="c40e2-122">3</span></span>|<span data-ttu-id="c40e2-123">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="c40e2-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="c40e2-124">хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="c40e2-124">httpWithInternetPeering</span></span>|<span data-ttu-id="c40e2-125">4 </span><span class="sxs-lookup"><span data-stu-id="c40e2-125">4</span></span>|<span data-ttu-id="c40e2-126">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="c40e2-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="c40e2-127">симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="c40e2-127">simpleDownload</span></span>|<span data-ttu-id="c40e2-128">99</span><span class="sxs-lookup"><span data-stu-id="c40e2-128">99</span></span>|<span data-ttu-id="c40e2-129">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="c40e2-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="c40e2-130">бипассмоде</span><span class="sxs-lookup"><span data-stu-id="c40e2-130">bypassMode</span></span>|<span data-ttu-id="c40e2-131">100</span><span class="sxs-lookup"><span data-stu-id="c40e2-131">100</span></span>|<span data-ttu-id="c40e2-132">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="c40e2-132">Bypass mode.</span></span> <span data-ttu-id="c40e2-133">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="c40e2-133">Do not use Delivery Optimization and use BITS instead</span></span>|




