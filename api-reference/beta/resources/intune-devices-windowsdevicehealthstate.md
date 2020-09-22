---
title: тип перечисления Виндовсдевицехеалсстате
description: Состояние Endpoint Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c24f0b022d60ef6a9b50d881fdaa05b88bd518c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080658"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="19cb9-103">тип перечисления Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="19cb9-103">windowsDeviceHealthState enum type</span></span>

<span data-ttu-id="19cb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19cb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19cb9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19cb9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19cb9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19cb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19cb9-107">Состояние Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="19cb9-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="19cb9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="19cb9-108">Members</span></span>
|<span data-ttu-id="19cb9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="19cb9-109">Member</span></span>|<span data-ttu-id="19cb9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="19cb9-110">Value</span></span>|<span data-ttu-id="19cb9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="19cb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19cb9-112">чистить</span><span class="sxs-lookup"><span data-stu-id="19cb9-112">clean</span></span>|<span data-ttu-id="19cb9-113">нуль</span><span class="sxs-lookup"><span data-stu-id="19cb9-113">0</span></span>|<span data-ttu-id="19cb9-114">Компьютер чист и никаких действий не требовалось</span><span class="sxs-lookup"><span data-stu-id="19cb9-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="19cb9-115">фуллсканпендинг</span><span class="sxs-lookup"><span data-stu-id="19cb9-115">fullScanPending</span></span>|<span data-ttu-id="19cb9-116">1 </span><span class="sxs-lookup"><span data-stu-id="19cb9-116">1</span></span>|<span data-ttu-id="19cb9-117">Компьютер находится в состоянии ожидания полного сканирования</span><span class="sxs-lookup"><span data-stu-id="19cb9-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="19cb9-118">ребутпендинг</span><span class="sxs-lookup"><span data-stu-id="19cb9-118">rebootPending</span></span>|<span data-ttu-id="19cb9-119">2 </span><span class="sxs-lookup"><span data-stu-id="19cb9-119">2</span></span>|<span data-ttu-id="19cb9-120">Компьютер находится в состоянии ожидания перезагрузки</span><span class="sxs-lookup"><span data-stu-id="19cb9-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="19cb9-121">мануалстепспендинг</span><span class="sxs-lookup"><span data-stu-id="19cb9-121">manualStepsPending</span></span>|<span data-ttu-id="19cb9-122">4 </span><span class="sxs-lookup"><span data-stu-id="19cb9-122">4</span></span>|<span data-ttu-id="19cb9-123">Компьютер находится в состоянии ожидания действий, выполняемых вручную</span><span class="sxs-lookup"><span data-stu-id="19cb9-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="19cb9-124">оффлинесканпендинг</span><span class="sxs-lookup"><span data-stu-id="19cb9-124">offlineScanPending</span></span>|<span data-ttu-id="19cb9-125">8 </span><span class="sxs-lookup"><span data-stu-id="19cb9-125">8</span></span>|<span data-ttu-id="19cb9-126">Компьютер находится в состоянии ожидания автономной проверки</span><span class="sxs-lookup"><span data-stu-id="19cb9-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="19cb9-127">наиболее</span><span class="sxs-lookup"><span data-stu-id="19cb9-127">critical</span></span>|<span data-ttu-id="19cb9-128">16 </span><span class="sxs-lookup"><span data-stu-id="19cb9-128">16</span></span>|<span data-ttu-id="19cb9-129">Компьютер находится в состоянии критической ошибки</span><span class="sxs-lookup"><span data-stu-id="19cb9-129">Computer is in critical failure state</span></span>|






