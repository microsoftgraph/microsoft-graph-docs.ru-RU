---
title: Тип перечисления windowsUpdateType
description: Какие устройства филиала будет получать обновления из
author: tfitzmac
ms.openlocfilehash: 415dde619529ffa9bb40ab2cea36665558bb0ee9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340840"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="9275e-103">Тип перечисления windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="9275e-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="9275e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9275e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9275e-105">Какие устройства филиала будет получать обновления из</span><span class="sxs-lookup"><span data-stu-id="9275e-105">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="9275e-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="9275e-106">Members</span></span>
|<span data-ttu-id="9275e-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="9275e-107">Member</span></span>|<span data-ttu-id="9275e-108">Значение</span><span class="sxs-lookup"><span data-stu-id="9275e-108">Value</span></span>|<span data-ttu-id="9275e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9275e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9275e-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="9275e-110">userDefined</span></span>|<span data-ttu-id="9275e-111">0</span><span class="sxs-lookup"><span data-stu-id="9275e-111">0</span></span>|<span data-ttu-id="9275e-112">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="9275e-112">Allow the user to set.</span></span>|
|<span data-ttu-id="9275e-113">all</span><span class="sxs-lookup"><span data-stu-id="9275e-113">all</span></span>|<span data-ttu-id="9275e-114">1</span><span class="sxs-lookup"><span data-stu-id="9275e-114">1</span></span>|<span data-ttu-id="9275e-115">Разделитель годовая канала (целевой).</span><span class="sxs-lookup"><span data-stu-id="9275e-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="9275e-116">Устройства получает все обновления компонента, которые применяются с точками годовая канала (требуемой).</span><span class="sxs-lookup"><span data-stu-id="9275e-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="9275e-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="9275e-117">businessReadyOnly</span></span>|<span data-ttu-id="9275e-118">2</span><span class="sxs-lookup"><span data-stu-id="9275e-118">2</span></span>|<span data-ttu-id="9275e-119">Разделитель годовая канала.</span><span class="sxs-lookup"><span data-stu-id="9275e-119">Semi-annual Channel.</span></span> <span data-ttu-id="9275e-120">Устройства получает обновления компонента точками годовая канала.</span><span class="sxs-lookup"><span data-stu-id="9275e-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="9275e-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="9275e-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="9275e-122">3</span><span class="sxs-lookup"><span data-stu-id="9275e-122">3</span></span>|<span data-ttu-id="9275e-123">Построение изнутри Windows - Fast</span><span class="sxs-lookup"><span data-stu-id="9275e-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="9275e-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="9275e-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="9275e-125">4</span><span class="sxs-lookup"><span data-stu-id="9275e-125">4</span></span>|<span data-ttu-id="9275e-126">Построение изнутри Windows - снижение производительности</span><span class="sxs-lookup"><span data-stu-id="9275e-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="9275e-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="9275e-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="9275e-128">5</span><span class="sxs-lookup"><span data-stu-id="9275e-128">5</span></span>|<span data-ttu-id="9275e-129">Построение выпуска Windows изнутри</span><span class="sxs-lookup"><span data-stu-id="9275e-129">Release Windows Insider build</span></span>|



