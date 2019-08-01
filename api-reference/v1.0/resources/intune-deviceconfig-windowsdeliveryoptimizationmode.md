---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9154a78af87dbef125e5d211aba284d7a0023e84
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027652"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="b50f5-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="b50f5-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="b50f5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b50f5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b50f5-105">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="b50f5-105">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="b50f5-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="b50f5-106">Members</span></span>
|<span data-ttu-id="b50f5-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="b50f5-107">Member</span></span>|<span data-ttu-id="b50f5-108">Значение</span><span class="sxs-lookup"><span data-stu-id="b50f5-108">Value</span></span>|<span data-ttu-id="b50f5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b50f5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b50f5-110">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="b50f5-110">userDefined</span></span>|<span data-ttu-id="b50f5-111">нуль</span><span class="sxs-lookup"><span data-stu-id="b50f5-111">0</span></span>|<span data-ttu-id="b50f5-112">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="b50f5-112">Allow the user to set.</span></span>|
|<span data-ttu-id="b50f5-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="b50f5-113">httpOnly</span></span>|<span data-ttu-id="b50f5-114">1,1</span><span class="sxs-lookup"><span data-stu-id="b50f5-114">1</span></span>|<span data-ttu-id="b50f5-115">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="b50f5-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="b50f5-116">Хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="b50f5-116">httpWithPeeringNat</span></span>|<span data-ttu-id="b50f5-117">2</span><span class="sxs-lookup"><span data-stu-id="b50f5-117">2</span></span>|<span data-ttu-id="b50f5-118">Операционная система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="b50f5-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="b50f5-119">Хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="b50f5-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="b50f5-120">4</span><span class="sxs-lookup"><span data-stu-id="b50f5-120">3</span></span>|<span data-ttu-id="b50f5-121">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="b50f5-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="b50f5-122">Хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="b50f5-122">httpWithInternetPeering</span></span>|<span data-ttu-id="b50f5-123">SP4</span><span class="sxs-lookup"><span data-stu-id="b50f5-123">4</span></span>|<span data-ttu-id="b50f5-124">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="b50f5-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="b50f5-125">Симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="b50f5-125">simpleDownload</span></span>|<span data-ttu-id="b50f5-126">99</span><span class="sxs-lookup"><span data-stu-id="b50f5-126">99</span></span>|<span data-ttu-id="b50f5-127">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="b50f5-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="b50f5-128">Бипассмоде</span><span class="sxs-lookup"><span data-stu-id="b50f5-128">bypassMode</span></span>|<span data-ttu-id="b50f5-129">100</span><span class="sxs-lookup"><span data-stu-id="b50f5-129">100</span></span>|<span data-ttu-id="b50f5-130">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="b50f5-130">Bypass mode.</span></span> <span data-ttu-id="b50f5-131">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="b50f5-131">Do not use Delivery Optimization and use BITS instead</span></span>|



