---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9be3f6861076bed1ef2e6d45336d975c07cba576
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451489"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="e3732-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="e3732-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="e3732-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3732-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3732-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3732-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3732-106">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="e3732-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="e3732-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e3732-107">Members</span></span>
|<span data-ttu-id="e3732-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e3732-108">Member</span></span>|<span data-ttu-id="e3732-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e3732-109">Value</span></span>|<span data-ttu-id="e3732-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e3732-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3732-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="e3732-111">userDefined</span></span>|<span data-ttu-id="e3732-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e3732-112">0</span></span>|<span data-ttu-id="e3732-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="e3732-113">Allow the user to set.</span></span>|
|<span data-ttu-id="e3732-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="e3732-114">httpOnly</span></span>|<span data-ttu-id="e3732-115">1,1</span><span class="sxs-lookup"><span data-stu-id="e3732-115">1</span></span>|<span data-ttu-id="e3732-116">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="e3732-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="e3732-117">хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="e3732-117">httpWithPeeringNat</span></span>|<span data-ttu-id="e3732-118">2</span><span class="sxs-lookup"><span data-stu-id="e3732-118">2</span></span>|<span data-ttu-id="e3732-119">Операционная система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="e3732-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="e3732-120">хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="e3732-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="e3732-121">4</span><span class="sxs-lookup"><span data-stu-id="e3732-121">3</span></span>|<span data-ttu-id="e3732-122">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="e3732-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="e3732-123">хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="e3732-123">httpWithInternetPeering</span></span>|<span data-ttu-id="e3732-124">4 </span><span class="sxs-lookup"><span data-stu-id="e3732-124">4</span></span>|<span data-ttu-id="e3732-125">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="e3732-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="e3732-126">симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="e3732-126">simpleDownload</span></span>|<span data-ttu-id="e3732-127">99</span><span class="sxs-lookup"><span data-stu-id="e3732-127">99</span></span>|<span data-ttu-id="e3732-128">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="e3732-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="e3732-129">бипассмоде</span><span class="sxs-lookup"><span data-stu-id="e3732-129">bypassMode</span></span>|<span data-ttu-id="e3732-130">100</span><span class="sxs-lookup"><span data-stu-id="e3732-130">100</span></span>|<span data-ttu-id="e3732-131">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="e3732-131">Bypass mode.</span></span> <span data-ttu-id="e3732-132">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="e3732-132">Do not use Delivery Optimization and use BITS instead</span></span>|







