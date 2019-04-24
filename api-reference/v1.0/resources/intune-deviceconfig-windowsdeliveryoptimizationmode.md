---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9034c7c90257a7ca622cd203d4ab84387fd2014
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463896"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="12308-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="12308-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="12308-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12308-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12308-105">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="12308-105">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="12308-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="12308-106">Members</span></span>
|<span data-ttu-id="12308-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="12308-107">Member</span></span>|<span data-ttu-id="12308-108">Значение</span><span class="sxs-lookup"><span data-stu-id="12308-108">Value</span></span>|<span data-ttu-id="12308-109">Описание</span><span class="sxs-lookup"><span data-stu-id="12308-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12308-110">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="12308-110">userDefined</span></span>|<span data-ttu-id="12308-111">нуль</span><span class="sxs-lookup"><span data-stu-id="12308-111">0</span></span>|<span data-ttu-id="12308-112">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="12308-112">Allow the user to set.</span></span>|
|<span data-ttu-id="12308-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="12308-113">httpOnly</span></span>|<span data-ttu-id="12308-114">1,1</span><span class="sxs-lookup"><span data-stu-id="12308-114">1</span></span>|<span data-ttu-id="12308-115">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="12308-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="12308-116">Хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="12308-116">httpWithPeeringNat</span></span>|<span data-ttu-id="12308-117">2</span><span class="sxs-lookup"><span data-stu-id="12308-117">2</span></span>|<span data-ttu-id="12308-118">ОПЕРАЦИОННАЯ система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="12308-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="12308-119">Хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="12308-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="12308-120">4</span><span class="sxs-lookup"><span data-stu-id="12308-120">3</span></span>|<span data-ttu-id="12308-121">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="12308-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="12308-122">Хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="12308-122">httpWithInternetPeering</span></span>|<span data-ttu-id="12308-123">SP4</span><span class="sxs-lookup"><span data-stu-id="12308-123">4</span></span>|<span data-ttu-id="12308-124">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="12308-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="12308-125">Симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="12308-125">simpleDownload</span></span>|<span data-ttu-id="12308-126">99</span><span class="sxs-lookup"><span data-stu-id="12308-126">99</span></span>|<span data-ttu-id="12308-127">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="12308-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="12308-128">Бипассмоде</span><span class="sxs-lookup"><span data-stu-id="12308-128">bypassMode</span></span>|<span data-ttu-id="12308-129">100</span><span class="sxs-lookup"><span data-stu-id="12308-129">100</span></span>|<span data-ttu-id="12308-130">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="12308-130">Bypass mode.</span></span> <span data-ttu-id="12308-131">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="12308-131">Do not use Delivery Optimization and use BITS instead</span></span>|



