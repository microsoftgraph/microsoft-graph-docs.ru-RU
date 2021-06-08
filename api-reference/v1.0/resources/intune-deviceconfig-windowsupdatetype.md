---
title: тип enum windowsUpdateType
description: Какие устройства филиала будут получать обновления от
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f49158686884d55825751a9314a50a9ab9a16d57
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759947"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="304d2-103">тип enum windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="304d2-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="304d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="304d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="304d2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="304d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="304d2-106">Какие устройства филиала будут получать обновления от</span><span class="sxs-lookup"><span data-stu-id="304d2-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="304d2-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="304d2-107">Members</span></span>
|<span data-ttu-id="304d2-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="304d2-108">Member</span></span>|<span data-ttu-id="304d2-109">Значение</span><span class="sxs-lookup"><span data-stu-id="304d2-109">Value</span></span>|<span data-ttu-id="304d2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="304d2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="304d2-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="304d2-111">userDefined</span></span>|<span data-ttu-id="304d2-112">0</span><span class="sxs-lookup"><span data-stu-id="304d2-112">0</span></span>|<span data-ttu-id="304d2-113">Разрешить пользователю установить.</span><span class="sxs-lookup"><span data-stu-id="304d2-113">Allow the user to set.</span></span>|
|<span data-ttu-id="304d2-114">все</span><span class="sxs-lookup"><span data-stu-id="304d2-114">all</span></span>|<span data-ttu-id="304d2-115">1</span><span class="sxs-lookup"><span data-stu-id="304d2-115">1</span></span>|<span data-ttu-id="304d2-116">Semi-annual Channel (Targeted).</span><span class="sxs-lookup"><span data-stu-id="304d2-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="304d2-117">Устройство получает все применимые обновления функций из Semi-annual Channel (Targeted).</span><span class="sxs-lookup"><span data-stu-id="304d2-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="304d2-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="304d2-118">businessReadyOnly</span></span>|<span data-ttu-id="304d2-119">2</span><span class="sxs-lookup"><span data-stu-id="304d2-119">2</span></span>|<span data-ttu-id="304d2-120">Полугодовой канал.</span><span class="sxs-lookup"><span data-stu-id="304d2-120">Semi-annual Channel.</span></span> <span data-ttu-id="304d2-121">Устройство получает обновления функций из Semi-annual Channel.</span><span class="sxs-lookup"><span data-stu-id="304d2-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="304d2-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="304d2-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="304d2-123">3</span><span class="sxs-lookup"><span data-stu-id="304d2-123">3</span></span>|<span data-ttu-id="304d2-124">Windows Сборка инсайдеров — быстрая</span><span class="sxs-lookup"><span data-stu-id="304d2-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="304d2-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="304d2-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="304d2-126">4 </span><span class="sxs-lookup"><span data-stu-id="304d2-126">4</span></span>|<span data-ttu-id="304d2-127">Windows Сборка инсайдеров - Slow</span><span class="sxs-lookup"><span data-stu-id="304d2-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="304d2-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="304d2-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="304d2-129">5 </span><span class="sxs-lookup"><span data-stu-id="304d2-129">5</span></span>|<span data-ttu-id="304d2-130">Сборка Windows insider</span><span class="sxs-lookup"><span data-stu-id="304d2-130">Release Windows Insider build</span></span>|




