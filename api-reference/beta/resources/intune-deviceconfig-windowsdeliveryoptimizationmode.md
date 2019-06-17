---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a41d359f77f0fd2a893236c9a4e952b321d003b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994089"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="ae946-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="ae946-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="ae946-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae946-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae946-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae946-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae946-106">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="ae946-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="ae946-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ae946-107">Members</span></span>
|<span data-ttu-id="ae946-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ae946-108">Member</span></span>|<span data-ttu-id="ae946-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ae946-109">Value</span></span>|<span data-ttu-id="ae946-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ae946-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae946-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="ae946-111">userDefined</span></span>|<span data-ttu-id="ae946-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ae946-112">0</span></span>|<span data-ttu-id="ae946-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="ae946-113">Allow the user to set.</span></span>|
|<span data-ttu-id="ae946-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="ae946-114">httpOnly</span></span>|<span data-ttu-id="ae946-115">1,1</span><span class="sxs-lookup"><span data-stu-id="ae946-115">1</span></span>|<span data-ttu-id="ae946-116">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="ae946-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="ae946-117">Хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="ae946-117">httpWithPeeringNat</span></span>|<span data-ttu-id="ae946-118">2</span><span class="sxs-lookup"><span data-stu-id="ae946-118">2</span></span>|<span data-ttu-id="ae946-119">Операционная система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="ae946-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="ae946-120">Хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="ae946-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="ae946-121">4</span><span class="sxs-lookup"><span data-stu-id="ae946-121">3</span></span>|<span data-ttu-id="ae946-122">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="ae946-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="ae946-123">Хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="ae946-123">httpWithInternetPeering</span></span>|<span data-ttu-id="ae946-124">SP4</span><span class="sxs-lookup"><span data-stu-id="ae946-124">4</span></span>|<span data-ttu-id="ae946-125">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="ae946-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="ae946-126">Симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="ae946-126">simpleDownload</span></span>|<span data-ttu-id="ae946-127">99</span><span class="sxs-lookup"><span data-stu-id="ae946-127">99</span></span>|<span data-ttu-id="ae946-128">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="ae946-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="ae946-129">Бипассмоде</span><span class="sxs-lookup"><span data-stu-id="ae946-129">bypassMode</span></span>|<span data-ttu-id="ae946-130">100</span><span class="sxs-lookup"><span data-stu-id="ae946-130">100</span></span>|<span data-ttu-id="ae946-131">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="ae946-131">Bypass mode.</span></span> <span data-ttu-id="ae946-132">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="ae946-132">Do not use Delivery Optimization and use BITS instead</span></span>|





