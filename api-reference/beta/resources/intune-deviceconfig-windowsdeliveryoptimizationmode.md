---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b2a66292ec6fb5db3fead93cbda7d24f5e505514
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371171"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="aba1d-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="aba1d-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="aba1d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aba1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aba1d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aba1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aba1d-106">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="aba1d-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="aba1d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="aba1d-107">Members</span></span>
|<span data-ttu-id="aba1d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="aba1d-108">Member</span></span>|<span data-ttu-id="aba1d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="aba1d-109">Value</span></span>|<span data-ttu-id="aba1d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aba1d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aba1d-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="aba1d-111">userDefined</span></span>|<span data-ttu-id="aba1d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="aba1d-112">0</span></span>|<span data-ttu-id="aba1d-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="aba1d-113">Allow the user to set.</span></span>|
|<span data-ttu-id="aba1d-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="aba1d-114">httpOnly</span></span>|<span data-ttu-id="aba1d-115">1,1</span><span class="sxs-lookup"><span data-stu-id="aba1d-115">1</span></span>|<span data-ttu-id="aba1d-116">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="aba1d-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="aba1d-117">хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="aba1d-117">httpWithPeeringNat</span></span>|<span data-ttu-id="aba1d-118">2</span><span class="sxs-lookup"><span data-stu-id="aba1d-118">2</span></span>|<span data-ttu-id="aba1d-119">Операционная система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="aba1d-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="aba1d-120">хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="aba1d-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="aba1d-121">4</span><span class="sxs-lookup"><span data-stu-id="aba1d-121">3</span></span>|<span data-ttu-id="aba1d-122">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="aba1d-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="aba1d-123">хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="aba1d-123">httpWithInternetPeering</span></span>|<span data-ttu-id="aba1d-124">SP4</span><span class="sxs-lookup"><span data-stu-id="aba1d-124">4</span></span>|<span data-ttu-id="aba1d-125">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="aba1d-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="aba1d-126">симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="aba1d-126">simpleDownload</span></span>|<span data-ttu-id="aba1d-127">99</span><span class="sxs-lookup"><span data-stu-id="aba1d-127">99</span></span>|<span data-ttu-id="aba1d-128">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="aba1d-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="aba1d-129">бипассмоде</span><span class="sxs-lookup"><span data-stu-id="aba1d-129">bypassMode</span></span>|<span data-ttu-id="aba1d-130">100</span><span class="sxs-lookup"><span data-stu-id="aba1d-130">100</span></span>|<span data-ttu-id="aba1d-131">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="aba1d-131">Bypass mode.</span></span> <span data-ttu-id="aba1d-132">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="aba1d-132">Do not use Delivery Optimization and use BITS instead</span></span>|



