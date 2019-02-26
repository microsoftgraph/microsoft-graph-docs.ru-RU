---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9034c7c90257a7ca622cd203d4ab84387fd2014
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251505"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="e8ddb-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="e8ddb-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="e8ddb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8ddb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8ddb-105">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="e8ddb-105">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="e8ddb-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="e8ddb-106">Members</span></span>
|<span data-ttu-id="e8ddb-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="e8ddb-107">Member</span></span>|<span data-ttu-id="e8ddb-108">Значение</span><span class="sxs-lookup"><span data-stu-id="e8ddb-108">Value</span></span>|<span data-ttu-id="e8ddb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e8ddb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8ddb-110">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="e8ddb-110">userDefined</span></span>|<span data-ttu-id="e8ddb-111">нуль</span><span class="sxs-lookup"><span data-stu-id="e8ddb-111">0</span></span>|<span data-ttu-id="e8ddb-112">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="e8ddb-112">Allow the user to set.</span></span>|
|<span data-ttu-id="e8ddb-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="e8ddb-113">httpOnly</span></span>|<span data-ttu-id="e8ddb-114">1,1</span><span class="sxs-lookup"><span data-stu-id="e8ddb-114">1</span></span>|<span data-ttu-id="e8ddb-115">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="e8ddb-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="e8ddb-116">Хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="e8ddb-116">httpWithPeeringNat</span></span>|<span data-ttu-id="e8ddb-117">2</span><span class="sxs-lookup"><span data-stu-id="e8ddb-117">2</span></span>|<span data-ttu-id="e8ddb-118">ОПЕРАЦИОННАЯ система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="e8ddb-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="e8ddb-119">Хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="e8ddb-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="e8ddb-120">4</span><span class="sxs-lookup"><span data-stu-id="e8ddb-120">3</span></span>|<span data-ttu-id="e8ddb-121">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="e8ddb-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="e8ddb-122">Хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="e8ddb-122">httpWithInternetPeering</span></span>|<span data-ttu-id="e8ddb-123">4</span><span class="sxs-lookup"><span data-stu-id="e8ddb-123">4</span></span>|<span data-ttu-id="e8ddb-124">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="e8ddb-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="e8ddb-125">Симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="e8ddb-125">simpleDownload</span></span>|<span data-ttu-id="e8ddb-126">99</span><span class="sxs-lookup"><span data-stu-id="e8ddb-126">99</span></span>|<span data-ttu-id="e8ddb-127">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="e8ddb-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="e8ddb-128">Бипассмоде</span><span class="sxs-lookup"><span data-stu-id="e8ddb-128">bypassMode</span></span>|<span data-ttu-id="e8ddb-129">100</span><span class="sxs-lookup"><span data-stu-id="e8ddb-129">100</span></span>|<span data-ttu-id="e8ddb-130">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="e8ddb-130">Bypass mode.</span></span> <span data-ttu-id="e8ddb-131">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="e8ddb-131">Do not use Delivery Optimization and use BITS instead</span></span>|



