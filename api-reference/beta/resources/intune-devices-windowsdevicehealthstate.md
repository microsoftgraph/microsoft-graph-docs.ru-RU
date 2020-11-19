---
title: тип перечисления Виндовсдевицехеалсстате
description: Состояние Endpoint Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ebe11f91b90074839a1a03dab2ce79788f259358
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208060"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="19567-103">тип перечисления Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="19567-103">windowsDeviceHealthState enum type</span></span>

<span data-ttu-id="19567-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19567-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19567-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19567-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19567-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19567-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19567-107">Состояние Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="19567-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="19567-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="19567-108">Members</span></span>
|<span data-ttu-id="19567-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="19567-109">Member</span></span>|<span data-ttu-id="19567-110">Значение</span><span class="sxs-lookup"><span data-stu-id="19567-110">Value</span></span>|<span data-ttu-id="19567-111">Описание</span><span class="sxs-lookup"><span data-stu-id="19567-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19567-112">чистить</span><span class="sxs-lookup"><span data-stu-id="19567-112">clean</span></span>|<span data-ttu-id="19567-113">нуль</span><span class="sxs-lookup"><span data-stu-id="19567-113">0</span></span>|<span data-ttu-id="19567-114">Компьютер чист и никаких действий не требовалось</span><span class="sxs-lookup"><span data-stu-id="19567-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="19567-115">фуллсканпендинг</span><span class="sxs-lookup"><span data-stu-id="19567-115">fullScanPending</span></span>|<span data-ttu-id="19567-116">1,1</span><span class="sxs-lookup"><span data-stu-id="19567-116">1</span></span>|<span data-ttu-id="19567-117">Компьютер находится в состоянии ожидания полного сканирования</span><span class="sxs-lookup"><span data-stu-id="19567-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="19567-118">ребутпендинг</span><span class="sxs-lookup"><span data-stu-id="19567-118">rebootPending</span></span>|<span data-ttu-id="19567-119">2</span><span class="sxs-lookup"><span data-stu-id="19567-119">2</span></span>|<span data-ttu-id="19567-120">Компьютер находится в состоянии ожидания перезагрузки</span><span class="sxs-lookup"><span data-stu-id="19567-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="19567-121">мануалстепспендинг</span><span class="sxs-lookup"><span data-stu-id="19567-121">manualStepsPending</span></span>|<span data-ttu-id="19567-122">4 </span><span class="sxs-lookup"><span data-stu-id="19567-122">4</span></span>|<span data-ttu-id="19567-123">Компьютер находится в состоянии ожидания действий, выполняемых вручную</span><span class="sxs-lookup"><span data-stu-id="19567-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="19567-124">оффлинесканпендинг</span><span class="sxs-lookup"><span data-stu-id="19567-124">offlineScanPending</span></span>|<span data-ttu-id="19567-125">8 </span><span class="sxs-lookup"><span data-stu-id="19567-125">8</span></span>|<span data-ttu-id="19567-126">Компьютер находится в состоянии ожидания автономной проверки</span><span class="sxs-lookup"><span data-stu-id="19567-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="19567-127">наиболее</span><span class="sxs-lookup"><span data-stu-id="19567-127">critical</span></span>|<span data-ttu-id="19567-128">16 </span><span class="sxs-lookup"><span data-stu-id="19567-128">16</span></span>|<span data-ttu-id="19567-129">Компьютер находится в состоянии критической ошибки</span><span class="sxs-lookup"><span data-stu-id="19567-129">Computer is in critical failure state</span></span>|




