---
title: тип перечисления Виндовсдевицехеалсстате
description: Состояние Endpoint Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6086dc05d204e4c9cb23c77f79f98c3a207de35c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941893"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="3b8c1-103">тип перечисления Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="3b8c1-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="3b8c1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b8c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b8c1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b8c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b8c1-106">Состояние Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="3b8c1-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="3b8c1-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3b8c1-107">Members</span></span>
|<span data-ttu-id="3b8c1-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3b8c1-108">Member</span></span>|<span data-ttu-id="3b8c1-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3b8c1-109">Value</span></span>|<span data-ttu-id="3b8c1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3b8c1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b8c1-111">чистить</span><span class="sxs-lookup"><span data-stu-id="3b8c1-111">clean</span></span>|<span data-ttu-id="3b8c1-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3b8c1-112">0</span></span>|<span data-ttu-id="3b8c1-113">Компьютер чист и никаких действий не требовалось</span><span class="sxs-lookup"><span data-stu-id="3b8c1-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="3b8c1-114">Фуллсканпендинг</span><span class="sxs-lookup"><span data-stu-id="3b8c1-114">fullScanPending</span></span>|<span data-ttu-id="3b8c1-115">1,1</span><span class="sxs-lookup"><span data-stu-id="3b8c1-115">1</span></span>|<span data-ttu-id="3b8c1-116">Компьютер находится в состоянии ожидания полного сканирования</span><span class="sxs-lookup"><span data-stu-id="3b8c1-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="3b8c1-117">Ребутпендинг</span><span class="sxs-lookup"><span data-stu-id="3b8c1-117">rebootPending</span></span>|<span data-ttu-id="3b8c1-118">2</span><span class="sxs-lookup"><span data-stu-id="3b8c1-118">2</span></span>|<span data-ttu-id="3b8c1-119">Компьютер находится в состоянии ожидания перезагрузки</span><span class="sxs-lookup"><span data-stu-id="3b8c1-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="3b8c1-120">Мануалстепспендинг</span><span class="sxs-lookup"><span data-stu-id="3b8c1-120">manualStepsPending</span></span>|<span data-ttu-id="3b8c1-121">SP4</span><span class="sxs-lookup"><span data-stu-id="3b8c1-121">4</span></span>|<span data-ttu-id="3b8c1-122">Компьютер находится в состоянии ожидания действий, выполняемых вручную</span><span class="sxs-lookup"><span data-stu-id="3b8c1-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="3b8c1-123">Оффлинесканпендинг</span><span class="sxs-lookup"><span data-stu-id="3b8c1-123">offlineScanPending</span></span>|<span data-ttu-id="3b8c1-124">8 </span><span class="sxs-lookup"><span data-stu-id="3b8c1-124">8</span></span>|<span data-ttu-id="3b8c1-125">Компьютер находится в состоянии ожидания автономной проверки</span><span class="sxs-lookup"><span data-stu-id="3b8c1-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="3b8c1-126">наиболее</span><span class="sxs-lookup"><span data-stu-id="3b8c1-126">critical</span></span>|<span data-ttu-id="3b8c1-127">столбцов</span><span class="sxs-lookup"><span data-stu-id="3b8c1-127">16</span></span>|<span data-ttu-id="3b8c1-128">Компьютер находится в состоянии критической ошибки</span><span class="sxs-lookup"><span data-stu-id="3b8c1-128">Computer is in critical failure state</span></span>|




