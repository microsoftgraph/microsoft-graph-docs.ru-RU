---
title: Тип перечисления windowsUpdateType
description: Какие устройства филиала будет получать обновления из
author: tfitzmac
ms.openlocfilehash: b41fea0254cbbb6a590d240c2db9e4fb7aa0e6eb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309627"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="99c09-103">Тип перечисления windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="99c09-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="99c09-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="99c09-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99c09-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99c09-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99c09-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="99c09-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99c09-107">Какие устройства филиала будет получать обновления из</span><span class="sxs-lookup"><span data-stu-id="99c09-107">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="99c09-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="99c09-108">Members</span></span>
|<span data-ttu-id="99c09-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="99c09-109">Member</span></span>|<span data-ttu-id="99c09-110">Значение</span><span class="sxs-lookup"><span data-stu-id="99c09-110">Value</span></span>|<span data-ttu-id="99c09-111">Описание</span><span class="sxs-lookup"><span data-stu-id="99c09-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99c09-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="99c09-112">userDefined</span></span>|<span data-ttu-id="99c09-113">0</span><span class="sxs-lookup"><span data-stu-id="99c09-113">0</span></span>|<span data-ttu-id="99c09-114">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="99c09-114">Allow the user to set.</span></span>|
|<span data-ttu-id="99c09-115">all</span><span class="sxs-lookup"><span data-stu-id="99c09-115">all</span></span>|<span data-ttu-id="99c09-116">1</span><span class="sxs-lookup"><span data-stu-id="99c09-116">1</span></span>|<span data-ttu-id="99c09-117">Разделитель годовая канала (целевой).</span><span class="sxs-lookup"><span data-stu-id="99c09-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="99c09-118">Устройства получает все обновления компонента, которые применяются с точками годовая канала (требуемой).</span><span class="sxs-lookup"><span data-stu-id="99c09-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="99c09-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="99c09-119">businessReadyOnly</span></span>|<span data-ttu-id="99c09-120">2</span><span class="sxs-lookup"><span data-stu-id="99c09-120">2</span></span>|<span data-ttu-id="99c09-121">Разделитель годовая канала.</span><span class="sxs-lookup"><span data-stu-id="99c09-121">Semi-annual Channel.</span></span> <span data-ttu-id="99c09-122">Устройства получает обновления компонента точками годовая канала.</span><span class="sxs-lookup"><span data-stu-id="99c09-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="99c09-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="99c09-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="99c09-124">3</span><span class="sxs-lookup"><span data-stu-id="99c09-124">3</span></span>|<span data-ttu-id="99c09-125">Построение изнутри Windows - Fast</span><span class="sxs-lookup"><span data-stu-id="99c09-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="99c09-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="99c09-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="99c09-127">4</span><span class="sxs-lookup"><span data-stu-id="99c09-127">4</span></span>|<span data-ttu-id="99c09-128">Построение изнутри Windows - снижение производительности</span><span class="sxs-lookup"><span data-stu-id="99c09-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="99c09-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="99c09-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="99c09-130">5</span><span class="sxs-lookup"><span data-stu-id="99c09-130">5</span></span>|<span data-ttu-id="99c09-131">Построение выпуска Windows изнутри</span><span class="sxs-lookup"><span data-stu-id="99c09-131">Release Windows Insider build</span></span>|





