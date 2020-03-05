---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 66ea4d13059cb9d3333c958481e711e5cd49b416
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529094"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="2cc8f-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="2cc8f-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="2cc8f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2cc8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cc8f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cc8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cc8f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cc8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cc8f-107">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="2cc8f-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="2cc8f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2cc8f-108">Members</span></span>
|<span data-ttu-id="2cc8f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2cc8f-109">Member</span></span>|<span data-ttu-id="2cc8f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2cc8f-110">Value</span></span>|<span data-ttu-id="2cc8f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2cc8f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cc8f-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="2cc8f-112">userDefined</span></span>|<span data-ttu-id="2cc8f-113">нуль</span><span class="sxs-lookup"><span data-stu-id="2cc8f-113">0</span></span>|<span data-ttu-id="2cc8f-114">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="2cc8f-114">Allow the user to set.</span></span>|
|<span data-ttu-id="2cc8f-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="2cc8f-115">httpOnly</span></span>|<span data-ttu-id="2cc8f-116">1 </span><span class="sxs-lookup"><span data-stu-id="2cc8f-116">1</span></span>|<span data-ttu-id="2cc8f-117">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="2cc8f-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="2cc8f-118">хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="2cc8f-118">httpWithPeeringNat</span></span>|<span data-ttu-id="2cc8f-119">2 </span><span class="sxs-lookup"><span data-stu-id="2cc8f-119">2</span></span>|<span data-ttu-id="2cc8f-120">Операционная система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="2cc8f-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="2cc8f-121">хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="2cc8f-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="2cc8f-122">3 </span><span class="sxs-lookup"><span data-stu-id="2cc8f-122">3</span></span>|<span data-ttu-id="2cc8f-123">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="2cc8f-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="2cc8f-124">хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="2cc8f-124">httpWithInternetPeering</span></span>|<span data-ttu-id="2cc8f-125">4 </span><span class="sxs-lookup"><span data-stu-id="2cc8f-125">4</span></span>|<span data-ttu-id="2cc8f-126">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="2cc8f-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="2cc8f-127">симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="2cc8f-127">simpleDownload</span></span>|<span data-ttu-id="2cc8f-128">99</span><span class="sxs-lookup"><span data-stu-id="2cc8f-128">99</span></span>|<span data-ttu-id="2cc8f-129">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="2cc8f-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="2cc8f-130">бипассмоде</span><span class="sxs-lookup"><span data-stu-id="2cc8f-130">bypassMode</span></span>|<span data-ttu-id="2cc8f-131">100</span><span class="sxs-lookup"><span data-stu-id="2cc8f-131">100</span></span>|<span data-ttu-id="2cc8f-132">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="2cc8f-132">Bypass mode.</span></span> <span data-ttu-id="2cc8f-133">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="2cc8f-133">Do not use Delivery Optimization and use BITS instead</span></span>|



