---
title: Тип перечисления windowsUpdateType
description: Какие устройства филиала будет получать обновления из
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 198b5f8db5698d309199964e4cb69f8981ceeb1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838971"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="58eb2-103">Тип перечисления windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="58eb2-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="58eb2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="58eb2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58eb2-105">Какие устройства филиала будет получать обновления из</span><span class="sxs-lookup"><span data-stu-id="58eb2-105">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="58eb2-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="58eb2-106">Members</span></span>
|<span data-ttu-id="58eb2-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="58eb2-107">Member</span></span>|<span data-ttu-id="58eb2-108">Значение</span><span class="sxs-lookup"><span data-stu-id="58eb2-108">Value</span></span>|<span data-ttu-id="58eb2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="58eb2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58eb2-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="58eb2-110">userDefined</span></span>|<span data-ttu-id="58eb2-111">0</span><span class="sxs-lookup"><span data-stu-id="58eb2-111">0</span></span>|<span data-ttu-id="58eb2-112">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="58eb2-112">Allow the user to set.</span></span>|
|<span data-ttu-id="58eb2-113">all</span><span class="sxs-lookup"><span data-stu-id="58eb2-113">all</span></span>|<span data-ttu-id="58eb2-114">1</span><span class="sxs-lookup"><span data-stu-id="58eb2-114">1</span></span>|<span data-ttu-id="58eb2-115">Разделитель годовая канала (целевой).</span><span class="sxs-lookup"><span data-stu-id="58eb2-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="58eb2-116">Устройства получает все обновления компонента, которые применяются с точками годовая канала (требуемой).</span><span class="sxs-lookup"><span data-stu-id="58eb2-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="58eb2-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="58eb2-117">businessReadyOnly</span></span>|<span data-ttu-id="58eb2-118">2</span><span class="sxs-lookup"><span data-stu-id="58eb2-118">2</span></span>|<span data-ttu-id="58eb2-119">Разделитель годовая канала.</span><span class="sxs-lookup"><span data-stu-id="58eb2-119">Semi-annual Channel.</span></span> <span data-ttu-id="58eb2-120">Устройства получает обновления компонента точками годовая канала.</span><span class="sxs-lookup"><span data-stu-id="58eb2-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="58eb2-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="58eb2-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="58eb2-122">3</span><span class="sxs-lookup"><span data-stu-id="58eb2-122">3</span></span>|<span data-ttu-id="58eb2-123">Построение изнутри Windows - Fast</span><span class="sxs-lookup"><span data-stu-id="58eb2-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="58eb2-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="58eb2-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="58eb2-125">4</span><span class="sxs-lookup"><span data-stu-id="58eb2-125">4</span></span>|<span data-ttu-id="58eb2-126">Построение изнутри Windows - снижение производительности</span><span class="sxs-lookup"><span data-stu-id="58eb2-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="58eb2-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="58eb2-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="58eb2-128">5</span><span class="sxs-lookup"><span data-stu-id="58eb2-128">5</span></span>|<span data-ttu-id="58eb2-129">Построение выпуска Windows изнутри</span><span class="sxs-lookup"><span data-stu-id="58eb2-129">Release Windows Insider build</span></span>|



