---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f38e2b1e99fb3d31064f1be63b1d9ae1618ee373
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451327"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="ee62b-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="ee62b-103">actionState enum type</span></span>

<span data-ttu-id="ee62b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee62b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee62b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee62b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee62b-106">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="ee62b-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="ee62b-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ee62b-107">Members</span></span>
|<span data-ttu-id="ee62b-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ee62b-108">Member</span></span>|<span data-ttu-id="ee62b-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ee62b-109">Value</span></span>|<span data-ttu-id="ee62b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ee62b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee62b-111">Нет</span><span class="sxs-lookup"><span data-stu-id="ee62b-111">none</span></span>|<span data-ttu-id="ee62b-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ee62b-112">0</span></span>|<span data-ttu-id="ee62b-113">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="ee62b-113">Not a valid action state</span></span>|
|<span data-ttu-id="ee62b-114">закончен</span><span class="sxs-lookup"><span data-stu-id="ee62b-114">pending</span></span>|<span data-ttu-id="ee62b-115">1,1</span><span class="sxs-lookup"><span data-stu-id="ee62b-115">1</span></span>|<span data-ttu-id="ee62b-116">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="ee62b-116">Action is pending</span></span>|
|<span data-ttu-id="ee62b-117">закрыт</span><span class="sxs-lookup"><span data-stu-id="ee62b-117">canceled</span></span>|<span data-ttu-id="ee62b-118">2</span><span class="sxs-lookup"><span data-stu-id="ee62b-118">2</span></span>|<span data-ttu-id="ee62b-119">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="ee62b-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="ee62b-120">ASP</span><span class="sxs-lookup"><span data-stu-id="ee62b-120">active</span></span>|<span data-ttu-id="ee62b-121">4</span><span class="sxs-lookup"><span data-stu-id="ee62b-121">3</span></span>|<span data-ttu-id="ee62b-122">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="ee62b-122">Action is active.</span></span>|
|<span data-ttu-id="ee62b-123">done</span><span class="sxs-lookup"><span data-stu-id="ee62b-123">done</span></span>|<span data-ttu-id="ee62b-124">4 </span><span class="sxs-lookup"><span data-stu-id="ee62b-124">4</span></span>|<span data-ttu-id="ee62b-125">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="ee62b-125">Action completed without errors.</span></span>|
|<span data-ttu-id="ee62b-126">сбоев</span><span class="sxs-lookup"><span data-stu-id="ee62b-126">failed</span></span>|<span data-ttu-id="ee62b-127">5 </span><span class="sxs-lookup"><span data-stu-id="ee62b-127">5</span></span>|<span data-ttu-id="ee62b-128">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="ee62b-128">Action failed</span></span>|
|<span data-ttu-id="ee62b-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="ee62b-129">notSupported</span></span>|<span data-ttu-id="ee62b-130">6 </span><span class="sxs-lookup"><span data-stu-id="ee62b-130">6</span></span>|<span data-ttu-id="ee62b-131">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee62b-131">Action is not supported.</span></span>|







