---
title: Тип перечисления windowsDeviceHealthState
description: Состояние защиты компьютера конечной точки
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2d971de9b20780bb51a19c3417384a0ca0563452
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416351"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="8f037-103">Тип перечисления windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="8f037-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="8f037-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8f037-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8f037-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f037-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f037-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f037-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f037-107">Состояние защиты компьютера конечной точки</span><span class="sxs-lookup"><span data-stu-id="8f037-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="8f037-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8f037-108">Members</span></span>
|<span data-ttu-id="8f037-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8f037-109">Member</span></span>|<span data-ttu-id="8f037-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8f037-110">Value</span></span>|<span data-ttu-id="8f037-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8f037-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f037-112">clean</span><span class="sxs-lookup"><span data-stu-id="8f037-112">clean</span></span>|<span data-ttu-id="8f037-113">0</span><span class="sxs-lookup"><span data-stu-id="8f037-113">0</span></span>|<span data-ttu-id="8f037-114">Компьютер чистой и никаких действий не требуется</span><span class="sxs-lookup"><span data-stu-id="8f037-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="8f037-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="8f037-115">fullScanPending</span></span>|<span data-ttu-id="8f037-116">1</span><span class="sxs-lookup"><span data-stu-id="8f037-116">1</span></span>|<span data-ttu-id="8f037-117">Компьютер находится в состоянии полную проверку ожидания</span><span class="sxs-lookup"><span data-stu-id="8f037-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="8f037-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="8f037-118">rebootPending</span></span>|<span data-ttu-id="8f037-119">2</span><span class="sxs-lookup"><span data-stu-id="8f037-119">2</span></span>|<span data-ttu-id="8f037-120">Компьютер находится в состоянии перезагрузки ожидания</span><span class="sxs-lookup"><span data-stu-id="8f037-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="8f037-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="8f037-121">manualStepsPending</span></span>|<span data-ttu-id="8f037-122">4</span><span class="sxs-lookup"><span data-stu-id="8f037-122">4</span></span>|<span data-ttu-id="8f037-123">Компьютер находится в состоянии ручные операции ожидания</span><span class="sxs-lookup"><span data-stu-id="8f037-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="8f037-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="8f037-124">offlineScanPending</span></span>|<span data-ttu-id="8f037-125">8</span><span class="sxs-lookup"><span data-stu-id="8f037-125">8</span></span>|<span data-ttu-id="8f037-126">Компьютер находится в состоянии автономной проверки ожидания</span><span class="sxs-lookup"><span data-stu-id="8f037-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="8f037-127">critical</span><span class="sxs-lookup"><span data-stu-id="8f037-127">critical</span></span>|<span data-ttu-id="8f037-128">16</span><span class="sxs-lookup"><span data-stu-id="8f037-128">16</span></span>|<span data-ttu-id="8f037-129">Компьютер находится в состоянии критическая ошибка</span><span class="sxs-lookup"><span data-stu-id="8f037-129">Computer is in critical failure state</span></span>|




