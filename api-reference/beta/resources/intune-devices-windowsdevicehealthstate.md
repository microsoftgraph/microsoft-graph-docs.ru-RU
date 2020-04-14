---
title: тип перечисления Виндовсдевицехеалсстате
description: Состояние Endpoint Protection
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1ce06c1b6c52266bb7d052a4524c6f4439973bde
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401752"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="1ffc7-103">тип перечисления Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="1ffc7-103">windowsDeviceHealthState enum type</span></span>

<span data-ttu-id="1ffc7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ffc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ffc7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ffc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ffc7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ffc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ffc7-107">Состояние Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="1ffc7-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="1ffc7-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1ffc7-108">Members</span></span>
|<span data-ttu-id="1ffc7-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1ffc7-109">Member</span></span>|<span data-ttu-id="1ffc7-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1ffc7-110">Value</span></span>|<span data-ttu-id="1ffc7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1ffc7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ffc7-112">чистить</span><span class="sxs-lookup"><span data-stu-id="1ffc7-112">clean</span></span>|<span data-ttu-id="1ffc7-113">нуль</span><span class="sxs-lookup"><span data-stu-id="1ffc7-113">0</span></span>|<span data-ttu-id="1ffc7-114">Компьютер чист и никаких действий не требовалось</span><span class="sxs-lookup"><span data-stu-id="1ffc7-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="1ffc7-115">фуллсканпендинг</span><span class="sxs-lookup"><span data-stu-id="1ffc7-115">fullScanPending</span></span>|<span data-ttu-id="1ffc7-116">1,1</span><span class="sxs-lookup"><span data-stu-id="1ffc7-116">1</span></span>|<span data-ttu-id="1ffc7-117">Компьютер находится в состоянии ожидания полного сканирования</span><span class="sxs-lookup"><span data-stu-id="1ffc7-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="1ffc7-118">ребутпендинг</span><span class="sxs-lookup"><span data-stu-id="1ffc7-118">rebootPending</span></span>|<span data-ttu-id="1ffc7-119">2</span><span class="sxs-lookup"><span data-stu-id="1ffc7-119">2</span></span>|<span data-ttu-id="1ffc7-120">Компьютер находится в состоянии ожидания перезагрузки</span><span class="sxs-lookup"><span data-stu-id="1ffc7-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="1ffc7-121">мануалстепспендинг</span><span class="sxs-lookup"><span data-stu-id="1ffc7-121">manualStepsPending</span></span>|<span data-ttu-id="1ffc7-122">4 </span><span class="sxs-lookup"><span data-stu-id="1ffc7-122">4</span></span>|<span data-ttu-id="1ffc7-123">Компьютер находится в состоянии ожидания действий, выполняемых вручную</span><span class="sxs-lookup"><span data-stu-id="1ffc7-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="1ffc7-124">оффлинесканпендинг</span><span class="sxs-lookup"><span data-stu-id="1ffc7-124">offlineScanPending</span></span>|<span data-ttu-id="1ffc7-125">8 </span><span class="sxs-lookup"><span data-stu-id="1ffc7-125">8</span></span>|<span data-ttu-id="1ffc7-126">Компьютер находится в состоянии ожидания автономной проверки</span><span class="sxs-lookup"><span data-stu-id="1ffc7-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="1ffc7-127">наиболее</span><span class="sxs-lookup"><span data-stu-id="1ffc7-127">critical</span></span>|<span data-ttu-id="1ffc7-128">16 </span><span class="sxs-lookup"><span data-stu-id="1ffc7-128">16</span></span>|<span data-ttu-id="1ffc7-129">Компьютер находится в состоянии критической ошибки</span><span class="sxs-lookup"><span data-stu-id="1ffc7-129">Computer is in critical failure state</span></span>|



