---
title: тип перечисления Виндовсдевицехеалсстате
description: Состояние Endpoint Protection
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 69d20e06ba23390ff912251bb99980c4a945704c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783713"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="16865-103">тип перечисления Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="16865-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="16865-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16865-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16865-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16865-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16865-106">Состояние Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="16865-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="16865-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="16865-107">Members</span></span>
|<span data-ttu-id="16865-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="16865-108">Member</span></span>|<span data-ttu-id="16865-109">Значение</span><span class="sxs-lookup"><span data-stu-id="16865-109">Value</span></span>|<span data-ttu-id="16865-110">Описание</span><span class="sxs-lookup"><span data-stu-id="16865-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16865-111">чистить</span><span class="sxs-lookup"><span data-stu-id="16865-111">clean</span></span>|<span data-ttu-id="16865-112">нуль</span><span class="sxs-lookup"><span data-stu-id="16865-112">0</span></span>|<span data-ttu-id="16865-113">Компьютер чист и никаких действий не требовалось</span><span class="sxs-lookup"><span data-stu-id="16865-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="16865-114">фуллсканпендинг</span><span class="sxs-lookup"><span data-stu-id="16865-114">fullScanPending</span></span>|<span data-ttu-id="16865-115">1,1</span><span class="sxs-lookup"><span data-stu-id="16865-115">1</span></span>|<span data-ttu-id="16865-116">Компьютер находится в состоянии ожидания полного сканирования</span><span class="sxs-lookup"><span data-stu-id="16865-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="16865-117">ребутпендинг</span><span class="sxs-lookup"><span data-stu-id="16865-117">rebootPending</span></span>|<span data-ttu-id="16865-118">2</span><span class="sxs-lookup"><span data-stu-id="16865-118">2</span></span>|<span data-ttu-id="16865-119">Компьютер находится в состоянии ожидания перезагрузки</span><span class="sxs-lookup"><span data-stu-id="16865-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="16865-120">мануалстепспендинг</span><span class="sxs-lookup"><span data-stu-id="16865-120">manualStepsPending</span></span>|<span data-ttu-id="16865-121">4 </span><span class="sxs-lookup"><span data-stu-id="16865-121">4</span></span>|<span data-ttu-id="16865-122">Компьютер находится в состоянии ожидания действий, выполняемых вручную</span><span class="sxs-lookup"><span data-stu-id="16865-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="16865-123">оффлинесканпендинг</span><span class="sxs-lookup"><span data-stu-id="16865-123">offlineScanPending</span></span>|<span data-ttu-id="16865-124">8 </span><span class="sxs-lookup"><span data-stu-id="16865-124">8</span></span>|<span data-ttu-id="16865-125">Компьютер находится в состоянии ожидания автономной проверки</span><span class="sxs-lookup"><span data-stu-id="16865-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="16865-126">наиболее</span><span class="sxs-lookup"><span data-stu-id="16865-126">critical</span></span>|<span data-ttu-id="16865-127">16 </span><span class="sxs-lookup"><span data-stu-id="16865-127">16</span></span>|<span data-ttu-id="16865-128">Компьютер находится в состоянии критической ошибки</span><span class="sxs-lookup"><span data-stu-id="16865-128">Computer is in critical failure state</span></span>|



