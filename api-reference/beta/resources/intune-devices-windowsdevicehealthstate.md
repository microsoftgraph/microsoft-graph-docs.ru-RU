---
title: тип перечисления Виндовсдевицехеалсстате
description: Состояние Endpoint Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9b37f441a1ded71d3f299d6d38b58543aac130ed
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366456"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="b4682-103">тип перечисления Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="b4682-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="b4682-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4682-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4682-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4682-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4682-106">Состояние Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="b4682-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="b4682-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b4682-107">Members</span></span>
|<span data-ttu-id="b4682-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b4682-108">Member</span></span>|<span data-ttu-id="b4682-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b4682-109">Value</span></span>|<span data-ttu-id="b4682-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b4682-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4682-111">чистить</span><span class="sxs-lookup"><span data-stu-id="b4682-111">clean</span></span>|<span data-ttu-id="b4682-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b4682-112">0</span></span>|<span data-ttu-id="b4682-113">Компьютер чист и никаких действий не требовалось</span><span class="sxs-lookup"><span data-stu-id="b4682-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="b4682-114">фуллсканпендинг</span><span class="sxs-lookup"><span data-stu-id="b4682-114">fullScanPending</span></span>|<span data-ttu-id="b4682-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b4682-115">1</span></span>|<span data-ttu-id="b4682-116">Компьютер находится в состоянии ожидания полного сканирования</span><span class="sxs-lookup"><span data-stu-id="b4682-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="b4682-117">ребутпендинг</span><span class="sxs-lookup"><span data-stu-id="b4682-117">rebootPending</span></span>|<span data-ttu-id="b4682-118">2</span><span class="sxs-lookup"><span data-stu-id="b4682-118">2</span></span>|<span data-ttu-id="b4682-119">Компьютер находится в состоянии ожидания перезагрузки</span><span class="sxs-lookup"><span data-stu-id="b4682-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="b4682-120">мануалстепспендинг</span><span class="sxs-lookup"><span data-stu-id="b4682-120">manualStepsPending</span></span>|<span data-ttu-id="b4682-121">SP4</span><span class="sxs-lookup"><span data-stu-id="b4682-121">4</span></span>|<span data-ttu-id="b4682-122">Компьютер находится в состоянии ожидания действий, выполняемых вручную</span><span class="sxs-lookup"><span data-stu-id="b4682-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="b4682-123">оффлинесканпендинг</span><span class="sxs-lookup"><span data-stu-id="b4682-123">offlineScanPending</span></span>|<span data-ttu-id="b4682-124">8 </span><span class="sxs-lookup"><span data-stu-id="b4682-124">8</span></span>|<span data-ttu-id="b4682-125">Компьютер находится в состоянии ожидания автономной проверки</span><span class="sxs-lookup"><span data-stu-id="b4682-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="b4682-126">наиболее</span><span class="sxs-lookup"><span data-stu-id="b4682-126">critical</span></span>|<span data-ttu-id="b4682-127">столбцов</span><span class="sxs-lookup"><span data-stu-id="b4682-127">16</span></span>|<span data-ttu-id="b4682-128">Компьютер находится в состоянии критической ошибки</span><span class="sxs-lookup"><span data-stu-id="b4682-128">Computer is in critical failure state</span></span>|



