---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4f4716f65c5405cf324d758ffd3c8bcf38d61b5e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523774"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="22c28-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="22c28-103">actionState enum type</span></span>

<span data-ttu-id="22c28-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="22c28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22c28-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22c28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22c28-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22c28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22c28-107">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="22c28-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="22c28-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="22c28-108">Members</span></span>
|<span data-ttu-id="22c28-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="22c28-109">Member</span></span>|<span data-ttu-id="22c28-110">Значение</span><span class="sxs-lookup"><span data-stu-id="22c28-110">Value</span></span>|<span data-ttu-id="22c28-111">Описание</span><span class="sxs-lookup"><span data-stu-id="22c28-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22c28-112">нет</span><span class="sxs-lookup"><span data-stu-id="22c28-112">none</span></span>|<span data-ttu-id="22c28-113">нуль</span><span class="sxs-lookup"><span data-stu-id="22c28-113">0</span></span>|<span data-ttu-id="22c28-114">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="22c28-114">Not a valid action state</span></span>|
|<span data-ttu-id="22c28-115">закончен</span><span class="sxs-lookup"><span data-stu-id="22c28-115">pending</span></span>|<span data-ttu-id="22c28-116">1 </span><span class="sxs-lookup"><span data-stu-id="22c28-116">1</span></span>|<span data-ttu-id="22c28-117">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="22c28-117">Action is pending</span></span>|
|<span data-ttu-id="22c28-118">закрыт</span><span class="sxs-lookup"><span data-stu-id="22c28-118">canceled</span></span>|<span data-ttu-id="22c28-119">2 </span><span class="sxs-lookup"><span data-stu-id="22c28-119">2</span></span>|<span data-ttu-id="22c28-120">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="22c28-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="22c28-121">ASP</span><span class="sxs-lookup"><span data-stu-id="22c28-121">active</span></span>|<span data-ttu-id="22c28-122">3 </span><span class="sxs-lookup"><span data-stu-id="22c28-122">3</span></span>|<span data-ttu-id="22c28-123">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="22c28-123">Action is active.</span></span>|
|<span data-ttu-id="22c28-124">done</span><span class="sxs-lookup"><span data-stu-id="22c28-124">done</span></span>|<span data-ttu-id="22c28-125">4 </span><span class="sxs-lookup"><span data-stu-id="22c28-125">4</span></span>|<span data-ttu-id="22c28-126">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="22c28-126">Action completed without errors.</span></span>|
|<span data-ttu-id="22c28-127">сбоев</span><span class="sxs-lookup"><span data-stu-id="22c28-127">failed</span></span>|<span data-ttu-id="22c28-128">5 </span><span class="sxs-lookup"><span data-stu-id="22c28-128">5</span></span>|<span data-ttu-id="22c28-129">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="22c28-129">Action failed</span></span>|
|<span data-ttu-id="22c28-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="22c28-130">notSupported</span></span>|<span data-ttu-id="22c28-131">6 </span><span class="sxs-lookup"><span data-stu-id="22c28-131">6</span></span>|<span data-ttu-id="22c28-132">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22c28-132">Action is not supported.</span></span>|



