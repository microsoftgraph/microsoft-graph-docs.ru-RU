---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa3e3dcd9b563301fb87b9bae0f3c2957631334b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939919"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="58804-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="58804-103">actionState enum type</span></span>

> <span data-ttu-id="58804-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58804-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58804-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58804-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58804-106">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="58804-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="58804-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="58804-107">Members</span></span>
|<span data-ttu-id="58804-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="58804-108">Member</span></span>|<span data-ttu-id="58804-109">Значение</span><span class="sxs-lookup"><span data-stu-id="58804-109">Value</span></span>|<span data-ttu-id="58804-110">Описание</span><span class="sxs-lookup"><span data-stu-id="58804-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58804-111">none</span><span class="sxs-lookup"><span data-stu-id="58804-111">none</span></span>|<span data-ttu-id="58804-112">нуль</span><span class="sxs-lookup"><span data-stu-id="58804-112">0</span></span>|<span data-ttu-id="58804-113">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="58804-113">Not a valid action state</span></span>|
|<span data-ttu-id="58804-114">закончен</span><span class="sxs-lookup"><span data-stu-id="58804-114">pending</span></span>|<span data-ttu-id="58804-115">1,1</span><span class="sxs-lookup"><span data-stu-id="58804-115">1</span></span>|<span data-ttu-id="58804-116">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="58804-116">Action is pending</span></span>|
|<span data-ttu-id="58804-117">закрыт</span><span class="sxs-lookup"><span data-stu-id="58804-117">canceled</span></span>|<span data-ttu-id="58804-118">2</span><span class="sxs-lookup"><span data-stu-id="58804-118">2</span></span>|<span data-ttu-id="58804-119">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="58804-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="58804-120">ASP</span><span class="sxs-lookup"><span data-stu-id="58804-120">active</span></span>|<span data-ttu-id="58804-121">4</span><span class="sxs-lookup"><span data-stu-id="58804-121">3</span></span>|<span data-ttu-id="58804-122">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="58804-122">Action is active.</span></span>|
|<span data-ttu-id="58804-123">done</span><span class="sxs-lookup"><span data-stu-id="58804-123">done</span></span>|<span data-ttu-id="58804-124">SP4</span><span class="sxs-lookup"><span data-stu-id="58804-124">4</span></span>|<span data-ttu-id="58804-125">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="58804-125">Action completed without errors.</span></span>|
|<span data-ttu-id="58804-126">сбоев</span><span class="sxs-lookup"><span data-stu-id="58804-126">failed</span></span>|<span data-ttu-id="58804-127">17:00</span><span class="sxs-lookup"><span data-stu-id="58804-127">5</span></span>|<span data-ttu-id="58804-128">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="58804-128">Action failed</span></span>|
|<span data-ttu-id="58804-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="58804-129">notSupported</span></span>|<span data-ttu-id="58804-130">6 </span><span class="sxs-lookup"><span data-stu-id="58804-130">6</span></span>|<span data-ttu-id="58804-131">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58804-131">Action is not supported.</span></span>|




