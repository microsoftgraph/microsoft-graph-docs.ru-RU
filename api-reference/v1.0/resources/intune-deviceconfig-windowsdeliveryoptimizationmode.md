---
title: тип enum windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для одноранговой рассылки
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5c483f00817858e7061bacf1b1e2b6ec6c00a02b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742750"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="e337d-103">тип enum windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="e337d-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="e337d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e337d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e337d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e337d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e337d-106">Режим оптимизации доставки для одноранговой рассылки</span><span class="sxs-lookup"><span data-stu-id="e337d-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="e337d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e337d-107">Members</span></span>
|<span data-ttu-id="e337d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e337d-108">Member</span></span>|<span data-ttu-id="e337d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e337d-109">Value</span></span>|<span data-ttu-id="e337d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e337d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e337d-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="e337d-111">userDefined</span></span>|<span data-ttu-id="e337d-112">0</span><span class="sxs-lookup"><span data-stu-id="e337d-112">0</span></span>|<span data-ttu-id="e337d-113">Разрешить пользователю установить.</span><span class="sxs-lookup"><span data-stu-id="e337d-113">Allow the user to set.</span></span>|
|<span data-ttu-id="e337d-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="e337d-114">httpOnly</span></span>|<span data-ttu-id="e337d-115">1</span><span class="sxs-lookup"><span data-stu-id="e337d-115">1</span></span>|<span data-ttu-id="e337d-116">ТОЛЬКО HTTP, без одноранговых</span><span class="sxs-lookup"><span data-stu-id="e337d-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="e337d-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="e337d-117">httpWithPeeringNat</span></span>|<span data-ttu-id="e337d-118">2</span><span class="sxs-lookup"><span data-stu-id="e337d-118">2</span></span>|<span data-ttu-id="e337d-119">По умолчанию ОС — http blended with peering behind the same network address translator</span><span class="sxs-lookup"><span data-stu-id="e337d-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="e337d-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="e337d-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="e337d-121">3</span><span class="sxs-lookup"><span data-stu-id="e337d-121">3</span></span>|<span data-ttu-id="e337d-122">HTTP, смешанный с вглядывом в частную группу</span><span class="sxs-lookup"><span data-stu-id="e337d-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="e337d-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="e337d-123">httpWithInternetPeering</span></span>|<span data-ttu-id="e337d-124">4 </span><span class="sxs-lookup"><span data-stu-id="e337d-124">4</span></span>|<span data-ttu-id="e337d-125">HTTP, смешанный с интернет-пирингом</span><span class="sxs-lookup"><span data-stu-id="e337d-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="e337d-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="e337d-126">simpleDownload</span></span>|<span data-ttu-id="e337d-127">99</span><span class="sxs-lookup"><span data-stu-id="e337d-127">99</span></span>|<span data-ttu-id="e337d-128">Простой режим загрузки без вглядывок</span><span class="sxs-lookup"><span data-stu-id="e337d-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="e337d-129">bypassMode</span><span class="sxs-lookup"><span data-stu-id="e337d-129">bypassMode</span></span>|<span data-ttu-id="e337d-130">100</span><span class="sxs-lookup"><span data-stu-id="e337d-130">100</span></span>|<span data-ttu-id="e337d-131">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="e337d-131">Bypass mode.</span></span> <span data-ttu-id="e337d-132">Не используйте оптимизацию доставки и вместо этого используйте BITS</span><span class="sxs-lookup"><span data-stu-id="e337d-132">Do not use Delivery Optimization and use BITS instead</span></span>|




