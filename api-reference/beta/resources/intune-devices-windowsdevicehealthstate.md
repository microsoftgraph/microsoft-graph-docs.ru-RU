---
title: Тип перечисления windowsDeviceHealthState
description: Состояние защиты компьютера конечной точки
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 91869502d0d61c25c6eb8dd67ba4e8e32d28fbb2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885927"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="b3d8b-103">Тип перечисления windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="b3d8b-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="b3d8b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b3d8b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3d8b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3d8b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3d8b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b3d8b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3d8b-107">Состояние защиты компьютера конечной точки</span><span class="sxs-lookup"><span data-stu-id="b3d8b-107">Computer endpoint protection state</span></span>
## <a name="members"></a><span data-ttu-id="b3d8b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b3d8b-108">Members</span></span>
|<span data-ttu-id="b3d8b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b3d8b-109">Member</span></span>|<span data-ttu-id="b3d8b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b3d8b-110">Value</span></span>|<span data-ttu-id="b3d8b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b3d8b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3d8b-112">clean</span><span class="sxs-lookup"><span data-stu-id="b3d8b-112">clean</span></span>|<span data-ttu-id="b3d8b-113">0</span><span class="sxs-lookup"><span data-stu-id="b3d8b-113">0</span></span>|<span data-ttu-id="b3d8b-114">Компьютер чистой и никаких действий не требуется</span><span class="sxs-lookup"><span data-stu-id="b3d8b-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="b3d8b-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="b3d8b-115">fullScanPending</span></span>|<span data-ttu-id="b3d8b-116">1</span><span class="sxs-lookup"><span data-stu-id="b3d8b-116">1</span></span>|<span data-ttu-id="b3d8b-117">Компьютер находится в состоянии полную проверку ожидания</span><span class="sxs-lookup"><span data-stu-id="b3d8b-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="b3d8b-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="b3d8b-118">rebootPending</span></span>|<span data-ttu-id="b3d8b-119">2</span><span class="sxs-lookup"><span data-stu-id="b3d8b-119">2</span></span>|<span data-ttu-id="b3d8b-120">Компьютер находится в состоянии перезагрузки ожидания</span><span class="sxs-lookup"><span data-stu-id="b3d8b-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="b3d8b-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="b3d8b-121">manualStepsPending</span></span>|<span data-ttu-id="b3d8b-122">4</span><span class="sxs-lookup"><span data-stu-id="b3d8b-122">4</span></span>|<span data-ttu-id="b3d8b-123">Компьютер находится в состоянии ручные операции ожидания</span><span class="sxs-lookup"><span data-stu-id="b3d8b-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="b3d8b-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="b3d8b-124">offlineScanPending</span></span>|<span data-ttu-id="b3d8b-125">8</span><span class="sxs-lookup"><span data-stu-id="b3d8b-125">8</span></span>|<span data-ttu-id="b3d8b-126">Компьютер находится в состоянии автономной проверки ожидания</span><span class="sxs-lookup"><span data-stu-id="b3d8b-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="b3d8b-127">critical</span><span class="sxs-lookup"><span data-stu-id="b3d8b-127">critical</span></span>|<span data-ttu-id="b3d8b-128">16</span><span class="sxs-lookup"><span data-stu-id="b3d8b-128">16</span></span>|<span data-ttu-id="b3d8b-129">Компьютер находится в состоянии критическая ошибка</span><span class="sxs-lookup"><span data-stu-id="b3d8b-129">Computer is in critical failure state</span></span>|





