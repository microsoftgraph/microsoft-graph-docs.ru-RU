---
title: тип перечисления Виндовсдевицехеалсстате
description: Состояние Endpoint Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb335cd39e6cbcd00f754faae8f7784001c424b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156170"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="256fb-103">тип перечисления Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="256fb-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="256fb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="256fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="256fb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="256fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="256fb-106">Состояние Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="256fb-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="256fb-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="256fb-107">Members</span></span>
|<span data-ttu-id="256fb-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="256fb-108">Member</span></span>|<span data-ttu-id="256fb-109">Значение</span><span class="sxs-lookup"><span data-stu-id="256fb-109">Value</span></span>|<span data-ttu-id="256fb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="256fb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="256fb-111">clean</span><span class="sxs-lookup"><span data-stu-id="256fb-111">clean</span></span>|<span data-ttu-id="256fb-112">нуль</span><span class="sxs-lookup"><span data-stu-id="256fb-112">0</span></span>|<span data-ttu-id="256fb-113">Компьютер чист и никаких действий не требовалось</span><span class="sxs-lookup"><span data-stu-id="256fb-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="256fb-114">Фуллсканпендинг</span><span class="sxs-lookup"><span data-stu-id="256fb-114">fullScanPending</span></span>|<span data-ttu-id="256fb-115">1,1</span><span class="sxs-lookup"><span data-stu-id="256fb-115">1</span></span>|<span data-ttu-id="256fb-116">Компьютер находится в состоянии ожидания полного сканирования</span><span class="sxs-lookup"><span data-stu-id="256fb-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="256fb-117">Ребутпендинг</span><span class="sxs-lookup"><span data-stu-id="256fb-117">rebootPending</span></span>|<span data-ttu-id="256fb-118">2</span><span class="sxs-lookup"><span data-stu-id="256fb-118">2</span></span>|<span data-ttu-id="256fb-119">Компьютер находится в состоянии ожидания перезагрузки</span><span class="sxs-lookup"><span data-stu-id="256fb-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="256fb-120">Мануалстепспендинг</span><span class="sxs-lookup"><span data-stu-id="256fb-120">manualStepsPending</span></span>|<span data-ttu-id="256fb-121">4</span><span class="sxs-lookup"><span data-stu-id="256fb-121">4</span></span>|<span data-ttu-id="256fb-122">Компьютер находится в состоянии ожидания действий, выполняемых вручную</span><span class="sxs-lookup"><span data-stu-id="256fb-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="256fb-123">Оффлинесканпендинг</span><span class="sxs-lookup"><span data-stu-id="256fb-123">offlineScanPending</span></span>|<span data-ttu-id="256fb-124">8,5</span><span class="sxs-lookup"><span data-stu-id="256fb-124">8</span></span>|<span data-ttu-id="256fb-125">Компьютер находится в состоянии ожидания автономной проверки</span><span class="sxs-lookup"><span data-stu-id="256fb-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="256fb-126">critical</span><span class="sxs-lookup"><span data-stu-id="256fb-126">critical</span></span>|<span data-ttu-id="256fb-127">столбцов</span><span class="sxs-lookup"><span data-stu-id="256fb-127">16</span></span>|<span data-ttu-id="256fb-128">Компьютер находится в состоянии критической ошибки</span><span class="sxs-lookup"><span data-stu-id="256fb-128">Computer is in critical failure state</span></span>|




