---
title: Тип перечисления windowsUpdateType
description: Какие устройства филиала будет получать обновления из
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 15d2d46684d38b57690cc9c12d9c49eccd652e6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887040"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="bf94c-103">Тип перечисления windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="bf94c-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="bf94c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf94c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf94c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf94c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf94c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bf94c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf94c-107">Какие устройства филиала будет получать обновления из</span><span class="sxs-lookup"><span data-stu-id="bf94c-107">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="bf94c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="bf94c-108">Members</span></span>
|<span data-ttu-id="bf94c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="bf94c-109">Member</span></span>|<span data-ttu-id="bf94c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="bf94c-110">Value</span></span>|<span data-ttu-id="bf94c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bf94c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf94c-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="bf94c-112">userDefined</span></span>|<span data-ttu-id="bf94c-113">0</span><span class="sxs-lookup"><span data-stu-id="bf94c-113">0</span></span>|<span data-ttu-id="bf94c-114">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="bf94c-114">Allow the user to set.</span></span>|
|<span data-ttu-id="bf94c-115">all</span><span class="sxs-lookup"><span data-stu-id="bf94c-115">all</span></span>|<span data-ttu-id="bf94c-116">1</span><span class="sxs-lookup"><span data-stu-id="bf94c-116">1</span></span>|<span data-ttu-id="bf94c-117">Разделитель годовая канала (целевой).</span><span class="sxs-lookup"><span data-stu-id="bf94c-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="bf94c-118">Устройства получает все обновления компонента, которые применяются с точками годовая канала (требуемой).</span><span class="sxs-lookup"><span data-stu-id="bf94c-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="bf94c-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="bf94c-119">businessReadyOnly</span></span>|<span data-ttu-id="bf94c-120">2</span><span class="sxs-lookup"><span data-stu-id="bf94c-120">2</span></span>|<span data-ttu-id="bf94c-121">Разделитель годовая канала.</span><span class="sxs-lookup"><span data-stu-id="bf94c-121">Semi-annual Channel.</span></span> <span data-ttu-id="bf94c-122">Устройства получает обновления компонента точками годовая канала.</span><span class="sxs-lookup"><span data-stu-id="bf94c-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="bf94c-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="bf94c-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="bf94c-124">3</span><span class="sxs-lookup"><span data-stu-id="bf94c-124">3</span></span>|<span data-ttu-id="bf94c-125">Построение изнутри Windows - Fast</span><span class="sxs-lookup"><span data-stu-id="bf94c-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="bf94c-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="bf94c-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="bf94c-127">4</span><span class="sxs-lookup"><span data-stu-id="bf94c-127">4</span></span>|<span data-ttu-id="bf94c-128">Построение изнутри Windows - снижение производительности</span><span class="sxs-lookup"><span data-stu-id="bf94c-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="bf94c-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="bf94c-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="bf94c-130">5</span><span class="sxs-lookup"><span data-stu-id="bf94c-130">5</span></span>|<span data-ttu-id="bf94c-131">Построение выпуска Windows изнутри</span><span class="sxs-lookup"><span data-stu-id="bf94c-131">Release Windows Insider build</span></span>|





