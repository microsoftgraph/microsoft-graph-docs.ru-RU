---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 734fa5b7920c64ed2f649f78a2e81de068e3e0db
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772260"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="dd212-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="dd212-103">actionState enum type</span></span>

> <span data-ttu-id="dd212-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd212-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd212-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd212-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd212-106">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="dd212-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="dd212-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="dd212-107">Members</span></span>
|<span data-ttu-id="dd212-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="dd212-108">Member</span></span>|<span data-ttu-id="dd212-109">Значение</span><span class="sxs-lookup"><span data-stu-id="dd212-109">Value</span></span>|<span data-ttu-id="dd212-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dd212-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd212-111">none</span><span class="sxs-lookup"><span data-stu-id="dd212-111">none</span></span>|<span data-ttu-id="dd212-112">нуль</span><span class="sxs-lookup"><span data-stu-id="dd212-112">0</span></span>|<span data-ttu-id="dd212-113">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="dd212-113">Not a valid action state</span></span>|
|<span data-ttu-id="dd212-114">закончен</span><span class="sxs-lookup"><span data-stu-id="dd212-114">pending</span></span>|<span data-ttu-id="dd212-115">1,1</span><span class="sxs-lookup"><span data-stu-id="dd212-115">1</span></span>|<span data-ttu-id="dd212-116">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="dd212-116">Action is pending</span></span>|
|<span data-ttu-id="dd212-117">закрыт</span><span class="sxs-lookup"><span data-stu-id="dd212-117">canceled</span></span>|<span data-ttu-id="dd212-118">2</span><span class="sxs-lookup"><span data-stu-id="dd212-118">2</span></span>|<span data-ttu-id="dd212-119">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="dd212-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="dd212-120">ASP</span><span class="sxs-lookup"><span data-stu-id="dd212-120">active</span></span>|<span data-ttu-id="dd212-121">4</span><span class="sxs-lookup"><span data-stu-id="dd212-121">3</span></span>|<span data-ttu-id="dd212-122">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="dd212-122">Action is active.</span></span>|
|<span data-ttu-id="dd212-123">done</span><span class="sxs-lookup"><span data-stu-id="dd212-123">done</span></span>|<span data-ttu-id="dd212-124">4 </span><span class="sxs-lookup"><span data-stu-id="dd212-124">4</span></span>|<span data-ttu-id="dd212-125">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="dd212-125">Action completed without errors.</span></span>|
|<span data-ttu-id="dd212-126">сбоев</span><span class="sxs-lookup"><span data-stu-id="dd212-126">failed</span></span>|<span data-ttu-id="dd212-127">5 </span><span class="sxs-lookup"><span data-stu-id="dd212-127">5</span></span>|<span data-ttu-id="dd212-128">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="dd212-128">Action failed</span></span>|
|<span data-ttu-id="dd212-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="dd212-129">notSupported</span></span>|<span data-ttu-id="dd212-130">6 </span><span class="sxs-lookup"><span data-stu-id="dd212-130">6</span></span>|<span data-ttu-id="dd212-131">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd212-131">Action is not supported.</span></span>|



