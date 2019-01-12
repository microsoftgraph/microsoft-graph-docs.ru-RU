---
title: Тип перечисления windowsUpdateType
description: Какие устройства филиала будет получать обновления из
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1444af64043ac38685ca022b56b8856be77a0b70
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944350"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="e4dd1-103">Тип перечисления windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="e4dd1-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="e4dd1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e4dd1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4dd1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4dd1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4dd1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e4dd1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4dd1-107">Какие устройства филиала будет получать обновления из</span><span class="sxs-lookup"><span data-stu-id="e4dd1-107">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="e4dd1-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e4dd1-108">Members</span></span>
|<span data-ttu-id="e4dd1-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e4dd1-109">Member</span></span>|<span data-ttu-id="e4dd1-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e4dd1-110">Value</span></span>|<span data-ttu-id="e4dd1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e4dd1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4dd1-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="e4dd1-112">userDefined</span></span>|<span data-ttu-id="e4dd1-113">0</span><span class="sxs-lookup"><span data-stu-id="e4dd1-113">0</span></span>|<span data-ttu-id="e4dd1-114">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="e4dd1-114">Allow the user to set.</span></span>|
|<span data-ttu-id="e4dd1-115">all</span><span class="sxs-lookup"><span data-stu-id="e4dd1-115">all</span></span>|<span data-ttu-id="e4dd1-116">1</span><span class="sxs-lookup"><span data-stu-id="e4dd1-116">1</span></span>|<span data-ttu-id="e4dd1-117">Разделитель годовая канала (целевой).</span><span class="sxs-lookup"><span data-stu-id="e4dd1-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="e4dd1-118">Устройства получает все обновления компонента, которые применяются с точками годовая канала (требуемой).</span><span class="sxs-lookup"><span data-stu-id="e4dd1-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="e4dd1-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="e4dd1-119">businessReadyOnly</span></span>|<span data-ttu-id="e4dd1-120">2</span><span class="sxs-lookup"><span data-stu-id="e4dd1-120">2</span></span>|<span data-ttu-id="e4dd1-121">Разделитель годовая канала.</span><span class="sxs-lookup"><span data-stu-id="e4dd1-121">Semi-annual Channel.</span></span> <span data-ttu-id="e4dd1-122">Устройства получает обновления компонента точками годовая канала.</span><span class="sxs-lookup"><span data-stu-id="e4dd1-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="e4dd1-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="e4dd1-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="e4dd1-124">3</span><span class="sxs-lookup"><span data-stu-id="e4dd1-124">3</span></span>|<span data-ttu-id="e4dd1-125">Построение изнутри Windows - Fast</span><span class="sxs-lookup"><span data-stu-id="e4dd1-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="e4dd1-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="e4dd1-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="e4dd1-127">4</span><span class="sxs-lookup"><span data-stu-id="e4dd1-127">4</span></span>|<span data-ttu-id="e4dd1-128">Построение изнутри Windows - снижение производительности</span><span class="sxs-lookup"><span data-stu-id="e4dd1-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="e4dd1-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="e4dd1-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="e4dd1-130">5</span><span class="sxs-lookup"><span data-stu-id="e4dd1-130">5</span></span>|<span data-ttu-id="e4dd1-131">Построение выпуска Windows изнутри</span><span class="sxs-lookup"><span data-stu-id="e4dd1-131">Release Windows Insider build</span></span>|





