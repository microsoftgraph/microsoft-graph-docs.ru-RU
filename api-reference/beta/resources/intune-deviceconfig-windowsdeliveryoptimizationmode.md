---
title: тип перечисления Виндовсделиверйоптимизатионмоде
description: Режим оптимизации доставки для распределения одноранговой сети
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 719e315f8cccf52f98dfddb979d9f0fd5490dff8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692431"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="38944-103">тип перечисления Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="38944-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="38944-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38944-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38944-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38944-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38944-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38944-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38944-107">Режим оптимизации доставки для распределения одноранговой сети</span><span class="sxs-lookup"><span data-stu-id="38944-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="38944-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="38944-108">Members</span></span>
|<span data-ttu-id="38944-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="38944-109">Member</span></span>|<span data-ttu-id="38944-110">Значение</span><span class="sxs-lookup"><span data-stu-id="38944-110">Value</span></span>|<span data-ttu-id="38944-111">Описание</span><span class="sxs-lookup"><span data-stu-id="38944-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38944-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="38944-112">userDefined</span></span>|<span data-ttu-id="38944-113">нуль</span><span class="sxs-lookup"><span data-stu-id="38944-113">0</span></span>|<span data-ttu-id="38944-114">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="38944-114">Allow the user to set.</span></span>|
|<span data-ttu-id="38944-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="38944-115">httpOnly</span></span>|<span data-ttu-id="38944-116">1,1</span><span class="sxs-lookup"><span data-stu-id="38944-116">1</span></span>|<span data-ttu-id="38944-117">Только HTTP, без пиринга</span><span class="sxs-lookup"><span data-stu-id="38944-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="38944-118">хттпвиспирингнат</span><span class="sxs-lookup"><span data-stu-id="38944-118">httpWithPeeringNat</span></span>|<span data-ttu-id="38944-119">2</span><span class="sxs-lookup"><span data-stu-id="38944-119">2</span></span>|<span data-ttu-id="38944-120">Операционная система по умолчанию — HTTP, смешанная с одноранговым устройством с одним транслятором сетевых адресов</span><span class="sxs-lookup"><span data-stu-id="38944-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="38944-121">хттпвиспирингприватеграуп</span><span class="sxs-lookup"><span data-stu-id="38944-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="38944-122">4</span><span class="sxs-lookup"><span data-stu-id="38944-122">3</span></span>|<span data-ttu-id="38944-123">HTTP-смешение с одноранговым элементом в частной группе</span><span class="sxs-lookup"><span data-stu-id="38944-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="38944-124">хттпвисинтернетпиринг</span><span class="sxs-lookup"><span data-stu-id="38944-124">httpWithInternetPeering</span></span>|<span data-ttu-id="38944-125">4 </span><span class="sxs-lookup"><span data-stu-id="38944-125">4</span></span>|<span data-ttu-id="38944-126">HTTP-смешение с подключением к Интернету</span><span class="sxs-lookup"><span data-stu-id="38944-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="38944-127">симпледовнлоад</span><span class="sxs-lookup"><span data-stu-id="38944-127">simpleDownload</span></span>|<span data-ttu-id="38944-128">99</span><span class="sxs-lookup"><span data-stu-id="38944-128">99</span></span>|<span data-ttu-id="38944-129">Простой режим загрузки без пиринга</span><span class="sxs-lookup"><span data-stu-id="38944-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="38944-130">бипассмоде</span><span class="sxs-lookup"><span data-stu-id="38944-130">bypassMode</span></span>|<span data-ttu-id="38944-131">100</span><span class="sxs-lookup"><span data-stu-id="38944-131">100</span></span>|<span data-ttu-id="38944-132">Режим обхода.</span><span class="sxs-lookup"><span data-stu-id="38944-132">Bypass mode.</span></span> <span data-ttu-id="38944-133">Не используйте оптимизацию доставки и не используйте BITS</span><span class="sxs-lookup"><span data-stu-id="38944-133">Do not use Delivery Optimization and use BITS instead</span></span>|





