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
# <a name="actionstate-enum-type"></a><span data-ttu-id="73182-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="73182-103">actionState enum type</span></span>

<span data-ttu-id="73182-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73182-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73182-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73182-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73182-106">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="73182-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="73182-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="73182-107">Members</span></span>
|<span data-ttu-id="73182-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="73182-108">Member</span></span>|<span data-ttu-id="73182-109">Значение</span><span class="sxs-lookup"><span data-stu-id="73182-109">Value</span></span>|<span data-ttu-id="73182-110">Описание</span><span class="sxs-lookup"><span data-stu-id="73182-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73182-111">нет</span><span class="sxs-lookup"><span data-stu-id="73182-111">none</span></span>|<span data-ttu-id="73182-112">нуль</span><span class="sxs-lookup"><span data-stu-id="73182-112">0</span></span>|<span data-ttu-id="73182-113">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="73182-113">Not a valid action state</span></span>|
|<span data-ttu-id="73182-114">закончен</span><span class="sxs-lookup"><span data-stu-id="73182-114">pending</span></span>|<span data-ttu-id="73182-115">1,1</span><span class="sxs-lookup"><span data-stu-id="73182-115">1</span></span>|<span data-ttu-id="73182-116">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="73182-116">Action is pending</span></span>|
|<span data-ttu-id="73182-117">закрыт</span><span class="sxs-lookup"><span data-stu-id="73182-117">canceled</span></span>|<span data-ttu-id="73182-118">2</span><span class="sxs-lookup"><span data-stu-id="73182-118">2</span></span>|<span data-ttu-id="73182-119">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="73182-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="73182-120">ASP</span><span class="sxs-lookup"><span data-stu-id="73182-120">active</span></span>|<span data-ttu-id="73182-121">4</span><span class="sxs-lookup"><span data-stu-id="73182-121">3</span></span>|<span data-ttu-id="73182-122">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="73182-122">Action is active.</span></span>|
|<span data-ttu-id="73182-123">done</span><span class="sxs-lookup"><span data-stu-id="73182-123">done</span></span>|<span data-ttu-id="73182-124">4 </span><span class="sxs-lookup"><span data-stu-id="73182-124">4</span></span>|<span data-ttu-id="73182-125">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="73182-125">Action completed without errors.</span></span>|
|<span data-ttu-id="73182-126">сбоев</span><span class="sxs-lookup"><span data-stu-id="73182-126">failed</span></span>|<span data-ttu-id="73182-127">5 </span><span class="sxs-lookup"><span data-stu-id="73182-127">5</span></span>|<span data-ttu-id="73182-128">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="73182-128">Action failed</span></span>|
|<span data-ttu-id="73182-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="73182-129">notSupported</span></span>|<span data-ttu-id="73182-130">6 </span><span class="sxs-lookup"><span data-stu-id="73182-130">6</span></span>|<span data-ttu-id="73182-131">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73182-131">Action is not supported.</span></span>|







