---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f75622021616ac0d65dd305c75d73af738f3446c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733170"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="6b3ab-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="6b3ab-103">actionState enum type</span></span>

<span data-ttu-id="6b3ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b3ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b3ab-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b3ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b3ab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b3ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b3ab-107">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="6b3ab-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="6b3ab-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="6b3ab-108">Members</span></span>
|<span data-ttu-id="6b3ab-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="6b3ab-109">Member</span></span>|<span data-ttu-id="6b3ab-110">Значение</span><span class="sxs-lookup"><span data-stu-id="6b3ab-110">Value</span></span>|<span data-ttu-id="6b3ab-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6b3ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b3ab-112">none</span><span class="sxs-lookup"><span data-stu-id="6b3ab-112">none</span></span>|<span data-ttu-id="6b3ab-113">нуль</span><span class="sxs-lookup"><span data-stu-id="6b3ab-113">0</span></span>|<span data-ttu-id="6b3ab-114">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="6b3ab-114">Not a valid action state</span></span>|
|<span data-ttu-id="6b3ab-115">закончен</span><span class="sxs-lookup"><span data-stu-id="6b3ab-115">pending</span></span>|<span data-ttu-id="6b3ab-116">1,1</span><span class="sxs-lookup"><span data-stu-id="6b3ab-116">1</span></span>|<span data-ttu-id="6b3ab-117">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="6b3ab-117">Action is pending</span></span>|
|<span data-ttu-id="6b3ab-118">закрыт</span><span class="sxs-lookup"><span data-stu-id="6b3ab-118">canceled</span></span>|<span data-ttu-id="6b3ab-119">2</span><span class="sxs-lookup"><span data-stu-id="6b3ab-119">2</span></span>|<span data-ttu-id="6b3ab-120">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="6b3ab-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="6b3ab-121">ASP</span><span class="sxs-lookup"><span data-stu-id="6b3ab-121">active</span></span>|<span data-ttu-id="6b3ab-122">4</span><span class="sxs-lookup"><span data-stu-id="6b3ab-122">3</span></span>|<span data-ttu-id="6b3ab-123">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="6b3ab-123">Action is active.</span></span>|
|<span data-ttu-id="6b3ab-124">done</span><span class="sxs-lookup"><span data-stu-id="6b3ab-124">done</span></span>|<span data-ttu-id="6b3ab-125">4 </span><span class="sxs-lookup"><span data-stu-id="6b3ab-125">4</span></span>|<span data-ttu-id="6b3ab-126">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="6b3ab-126">Action completed without errors.</span></span>|
|<span data-ttu-id="6b3ab-127">сбоев</span><span class="sxs-lookup"><span data-stu-id="6b3ab-127">failed</span></span>|<span data-ttu-id="6b3ab-128">5 </span><span class="sxs-lookup"><span data-stu-id="6b3ab-128">5</span></span>|<span data-ttu-id="6b3ab-129">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="6b3ab-129">Action failed</span></span>|
|<span data-ttu-id="6b3ab-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="6b3ab-130">notSupported</span></span>|<span data-ttu-id="6b3ab-131">6 </span><span class="sxs-lookup"><span data-stu-id="6b3ab-131">6</span></span>|<span data-ttu-id="6b3ab-132">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b3ab-132">Action is not supported.</span></span>|





