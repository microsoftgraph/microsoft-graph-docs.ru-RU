---
title: Тип перечисления windowsUpdateType
description: Какие устройства филиала будет получать обновления из
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d3dd0f6d8ba46d7f1cc803b217a98a862602149
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400139"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="01ce5-103">Тип перечисления windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="01ce5-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="01ce5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01ce5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="01ce5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01ce5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01ce5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01ce5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01ce5-107">Какие устройства филиала будет получать обновления из</span><span class="sxs-lookup"><span data-stu-id="01ce5-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="01ce5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="01ce5-108">Members</span></span>
|<span data-ttu-id="01ce5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="01ce5-109">Member</span></span>|<span data-ttu-id="01ce5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="01ce5-110">Value</span></span>|<span data-ttu-id="01ce5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="01ce5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01ce5-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="01ce5-112">userDefined</span></span>|<span data-ttu-id="01ce5-113">0</span><span class="sxs-lookup"><span data-stu-id="01ce5-113">0</span></span>|<span data-ttu-id="01ce5-114">Пользователь может задать.</span><span class="sxs-lookup"><span data-stu-id="01ce5-114">Allow the user to set.</span></span>|
|<span data-ttu-id="01ce5-115">all</span><span class="sxs-lookup"><span data-stu-id="01ce5-115">all</span></span>|<span data-ttu-id="01ce5-116">1</span><span class="sxs-lookup"><span data-stu-id="01ce5-116">1</span></span>|<span data-ttu-id="01ce5-117">Разделитель годовая канала (целевой).</span><span class="sxs-lookup"><span data-stu-id="01ce5-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="01ce5-118">Устройства получает все обновления компонента, которые применяются с точками годовая канала (требуемой).</span><span class="sxs-lookup"><span data-stu-id="01ce5-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="01ce5-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="01ce5-119">businessReadyOnly</span></span>|<span data-ttu-id="01ce5-120">2</span><span class="sxs-lookup"><span data-stu-id="01ce5-120">2</span></span>|<span data-ttu-id="01ce5-121">Разделитель годовая канала.</span><span class="sxs-lookup"><span data-stu-id="01ce5-121">Semi-annual Channel.</span></span> <span data-ttu-id="01ce5-122">Устройства получает обновления компонента точками годовая канала.</span><span class="sxs-lookup"><span data-stu-id="01ce5-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="01ce5-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="01ce5-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="01ce5-124">3</span><span class="sxs-lookup"><span data-stu-id="01ce5-124">3</span></span>|<span data-ttu-id="01ce5-125">Построение изнутри Windows - Fast</span><span class="sxs-lookup"><span data-stu-id="01ce5-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="01ce5-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="01ce5-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="01ce5-127">4</span><span class="sxs-lookup"><span data-stu-id="01ce5-127">4</span></span>|<span data-ttu-id="01ce5-128">Построение изнутри Windows - снижение производительности</span><span class="sxs-lookup"><span data-stu-id="01ce5-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="01ce5-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="01ce5-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="01ce5-130">5</span><span class="sxs-lookup"><span data-stu-id="01ce5-130">5</span></span>|<span data-ttu-id="01ce5-131">Построение выпуска Windows изнутри</span><span class="sxs-lookup"><span data-stu-id="01ce5-131">Release Windows Insider build</span></span>|




