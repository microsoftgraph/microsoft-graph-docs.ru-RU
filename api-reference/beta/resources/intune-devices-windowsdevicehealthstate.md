---
title: тип перечисления Виндовсдевицехеалсстате
description: Состояние Endpoint Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7da8a7cc01cef7ff410611e819739e226a4baee1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549480"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="0838b-103">тип перечисления Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="0838b-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="0838b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0838b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0838b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0838b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0838b-106">Состояние Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="0838b-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="0838b-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="0838b-107">Members</span></span>
|<span data-ttu-id="0838b-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="0838b-108">Member</span></span>|<span data-ttu-id="0838b-109">Значение</span><span class="sxs-lookup"><span data-stu-id="0838b-109">Value</span></span>|<span data-ttu-id="0838b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0838b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0838b-111">чистить</span><span class="sxs-lookup"><span data-stu-id="0838b-111">clean</span></span>|<span data-ttu-id="0838b-112">нуль</span><span class="sxs-lookup"><span data-stu-id="0838b-112">0</span></span>|<span data-ttu-id="0838b-113">Компьютер чист и никаких действий не требовалось</span><span class="sxs-lookup"><span data-stu-id="0838b-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="0838b-114">Фуллсканпендинг</span><span class="sxs-lookup"><span data-stu-id="0838b-114">fullScanPending</span></span>|<span data-ttu-id="0838b-115">1 </span><span class="sxs-lookup"><span data-stu-id="0838b-115">1</span></span>|<span data-ttu-id="0838b-116">Компьютер находится в состоянии ожидания полного сканирования</span><span class="sxs-lookup"><span data-stu-id="0838b-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="0838b-117">Ребутпендинг</span><span class="sxs-lookup"><span data-stu-id="0838b-117">rebootPending</span></span>|<span data-ttu-id="0838b-118">2 </span><span class="sxs-lookup"><span data-stu-id="0838b-118">2</span></span>|<span data-ttu-id="0838b-119">Компьютер находится в состоянии ожидания перезагрузки</span><span class="sxs-lookup"><span data-stu-id="0838b-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="0838b-120">Мануалстепспендинг</span><span class="sxs-lookup"><span data-stu-id="0838b-120">manualStepsPending</span></span>|<span data-ttu-id="0838b-121">4 </span><span class="sxs-lookup"><span data-stu-id="0838b-121">4</span></span>|<span data-ttu-id="0838b-122">Компьютер находится в состоянии ожидания действий, выполняемых вручную</span><span class="sxs-lookup"><span data-stu-id="0838b-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="0838b-123">Оффлинесканпендинг</span><span class="sxs-lookup"><span data-stu-id="0838b-123">offlineScanPending</span></span>|<span data-ttu-id="0838b-124">8 </span><span class="sxs-lookup"><span data-stu-id="0838b-124">8</span></span>|<span data-ttu-id="0838b-125">Компьютер находится в состоянии ожидания автономной проверки</span><span class="sxs-lookup"><span data-stu-id="0838b-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="0838b-126">наиболее</span><span class="sxs-lookup"><span data-stu-id="0838b-126">critical</span></span>|<span data-ttu-id="0838b-127">16 </span><span class="sxs-lookup"><span data-stu-id="0838b-127">16</span></span>|<span data-ttu-id="0838b-128">Компьютер находится в состоянии критической ошибки</span><span class="sxs-lookup"><span data-stu-id="0838b-128">Computer is in critical failure state</span></span>|





