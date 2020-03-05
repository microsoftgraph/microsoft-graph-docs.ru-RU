---
title: тип перечисления Виндовсдевицехеалсстате
description: Состояние Endpoint Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c5b4c042b93271632df933892ff8296c19c0585b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528424"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="b9d8d-103">тип перечисления Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="b9d8d-103">windowsDeviceHealthState enum type</span></span>

<span data-ttu-id="b9d8d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b9d8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9d8d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9d8d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9d8d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9d8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9d8d-107">Состояние Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="b9d8d-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="b9d8d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b9d8d-108">Members</span></span>
|<span data-ttu-id="b9d8d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b9d8d-109">Member</span></span>|<span data-ttu-id="b9d8d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b9d8d-110">Value</span></span>|<span data-ttu-id="b9d8d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b9d8d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9d8d-112">чистить</span><span class="sxs-lookup"><span data-stu-id="b9d8d-112">clean</span></span>|<span data-ttu-id="b9d8d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="b9d8d-113">0</span></span>|<span data-ttu-id="b9d8d-114">Компьютер чист и никаких действий не требовалось</span><span class="sxs-lookup"><span data-stu-id="b9d8d-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="b9d8d-115">фуллсканпендинг</span><span class="sxs-lookup"><span data-stu-id="b9d8d-115">fullScanPending</span></span>|<span data-ttu-id="b9d8d-116">1 </span><span class="sxs-lookup"><span data-stu-id="b9d8d-116">1</span></span>|<span data-ttu-id="b9d8d-117">Компьютер находится в состоянии ожидания полного сканирования</span><span class="sxs-lookup"><span data-stu-id="b9d8d-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="b9d8d-118">ребутпендинг</span><span class="sxs-lookup"><span data-stu-id="b9d8d-118">rebootPending</span></span>|<span data-ttu-id="b9d8d-119">2 </span><span class="sxs-lookup"><span data-stu-id="b9d8d-119">2</span></span>|<span data-ttu-id="b9d8d-120">Компьютер находится в состоянии ожидания перезагрузки</span><span class="sxs-lookup"><span data-stu-id="b9d8d-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="b9d8d-121">мануалстепспендинг</span><span class="sxs-lookup"><span data-stu-id="b9d8d-121">manualStepsPending</span></span>|<span data-ttu-id="b9d8d-122">4 </span><span class="sxs-lookup"><span data-stu-id="b9d8d-122">4</span></span>|<span data-ttu-id="b9d8d-123">Компьютер находится в состоянии ожидания действий, выполняемых вручную</span><span class="sxs-lookup"><span data-stu-id="b9d8d-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="b9d8d-124">оффлинесканпендинг</span><span class="sxs-lookup"><span data-stu-id="b9d8d-124">offlineScanPending</span></span>|<span data-ttu-id="b9d8d-125">8 </span><span class="sxs-lookup"><span data-stu-id="b9d8d-125">8</span></span>|<span data-ttu-id="b9d8d-126">Компьютер находится в состоянии ожидания автономной проверки</span><span class="sxs-lookup"><span data-stu-id="b9d8d-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="b9d8d-127">наиболее</span><span class="sxs-lookup"><span data-stu-id="b9d8d-127">critical</span></span>|<span data-ttu-id="b9d8d-128">16 </span><span class="sxs-lookup"><span data-stu-id="b9d8d-128">16</span></span>|<span data-ttu-id="b9d8d-129">Компьютер находится в состоянии критической ошибки</span><span class="sxs-lookup"><span data-stu-id="b9d8d-129">Computer is in critical failure state</span></span>|



