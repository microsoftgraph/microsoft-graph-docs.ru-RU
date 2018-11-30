---
title: Тип перечисления windowsUpdateType
description: Какие устройства филиала будет получать обновления из
ms.openlocfilehash: b489f17da5dc02dd7f7e72350eef282e56643dd0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028068"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="b5703-103">Тип перечисления windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="b5703-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="b5703-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b5703-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5703-105">Какие устройства филиала будет получать обновления из</span><span class="sxs-lookup"><span data-stu-id="b5703-105">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="b5703-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="b5703-106">Members</span></span>
|<span data-ttu-id="b5703-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="b5703-107">Member</span></span>|<span data-ttu-id="b5703-108">Значение</span><span class="sxs-lookup"><span data-stu-id="b5703-108">Value</span></span>|<span data-ttu-id="b5703-109">Description</span><span class="sxs-lookup"><span data-stu-id="b5703-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5703-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="b5703-110">userDefined</span></span>|<span data-ttu-id="b5703-111">0</span><span class="sxs-lookup"><span data-stu-id="b5703-111">0</span></span>|<span data-ttu-id="b5703-112">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="b5703-112">Allow the user to set.</span></span>|
|<span data-ttu-id="b5703-113">all</span><span class="sxs-lookup"><span data-stu-id="b5703-113">all</span></span>|<span data-ttu-id="b5703-114">1</span><span class="sxs-lookup"><span data-stu-id="b5703-114">1</span></span>|<span data-ttu-id="b5703-115">Разделитель годовая канала (целевой).</span><span class="sxs-lookup"><span data-stu-id="b5703-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="b5703-116">Устройства получает все обновления компонента, которые применяются с точками годовая канала (требуемой).</span><span class="sxs-lookup"><span data-stu-id="b5703-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="b5703-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="b5703-117">businessReadyOnly</span></span>|<span data-ttu-id="b5703-118">2</span><span class="sxs-lookup"><span data-stu-id="b5703-118">2</span></span>|<span data-ttu-id="b5703-119">Разделитель годовая канала.</span><span class="sxs-lookup"><span data-stu-id="b5703-119">Semi-annual Channel.</span></span> <span data-ttu-id="b5703-120">Устройства получает обновления компонента точками годовая канала.</span><span class="sxs-lookup"><span data-stu-id="b5703-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="b5703-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="b5703-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="b5703-122">3</span><span class="sxs-lookup"><span data-stu-id="b5703-122">3</span></span>|<span data-ttu-id="b5703-123">Построение изнутри Windows - Fast</span><span class="sxs-lookup"><span data-stu-id="b5703-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="b5703-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="b5703-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="b5703-125">4</span><span class="sxs-lookup"><span data-stu-id="b5703-125">4</span></span>|<span data-ttu-id="b5703-126">Построение изнутри Windows - снижение производительности</span><span class="sxs-lookup"><span data-stu-id="b5703-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="b5703-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="b5703-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="b5703-128">5</span><span class="sxs-lookup"><span data-stu-id="b5703-128">5</span></span>|<span data-ttu-id="b5703-129">Построение выпуска Windows изнутри</span><span class="sxs-lookup"><span data-stu-id="b5703-129">Release Windows Insider build</span></span>|



