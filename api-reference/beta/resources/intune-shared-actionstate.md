---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1188670476e911b01375598a2361aae326a98425
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793464"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="767af-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="767af-103">actionState enum type</span></span>

> <span data-ttu-id="767af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="767af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="767af-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="767af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="767af-106">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="767af-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="767af-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="767af-107">Members</span></span>
|<span data-ttu-id="767af-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="767af-108">Member</span></span>|<span data-ttu-id="767af-109">Значение</span><span class="sxs-lookup"><span data-stu-id="767af-109">Value</span></span>|<span data-ttu-id="767af-110">Описание</span><span class="sxs-lookup"><span data-stu-id="767af-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="767af-111">нет</span><span class="sxs-lookup"><span data-stu-id="767af-111">none</span></span>|<span data-ttu-id="767af-112">нуль</span><span class="sxs-lookup"><span data-stu-id="767af-112">0</span></span>|<span data-ttu-id="767af-113">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="767af-113">Not a valid action state</span></span>|
|<span data-ttu-id="767af-114">закончен</span><span class="sxs-lookup"><span data-stu-id="767af-114">pending</span></span>|<span data-ttu-id="767af-115">1,1</span><span class="sxs-lookup"><span data-stu-id="767af-115">1</span></span>|<span data-ttu-id="767af-116">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="767af-116">Action is pending</span></span>|
|<span data-ttu-id="767af-117">закрыт</span><span class="sxs-lookup"><span data-stu-id="767af-117">canceled</span></span>|<span data-ttu-id="767af-118">2</span><span class="sxs-lookup"><span data-stu-id="767af-118">2</span></span>|<span data-ttu-id="767af-119">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="767af-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="767af-120">ASP</span><span class="sxs-lookup"><span data-stu-id="767af-120">active</span></span>|<span data-ttu-id="767af-121">4</span><span class="sxs-lookup"><span data-stu-id="767af-121">3</span></span>|<span data-ttu-id="767af-122">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="767af-122">Action is active.</span></span>|
|<span data-ttu-id="767af-123">done</span><span class="sxs-lookup"><span data-stu-id="767af-123">done</span></span>|<span data-ttu-id="767af-124">SP4</span><span class="sxs-lookup"><span data-stu-id="767af-124">4</span></span>|<span data-ttu-id="767af-125">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="767af-125">Action completed without errors.</span></span>|
|<span data-ttu-id="767af-126">сбоев</span><span class="sxs-lookup"><span data-stu-id="767af-126">failed</span></span>|<span data-ttu-id="767af-127">17:00</span><span class="sxs-lookup"><span data-stu-id="767af-127">5</span></span>|<span data-ttu-id="767af-128">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="767af-128">Action failed</span></span>|
|<span data-ttu-id="767af-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="767af-129">notSupported</span></span>|<span data-ttu-id="767af-130">ICMPv6</span><span class="sxs-lookup"><span data-stu-id="767af-130">6</span></span>|<span data-ttu-id="767af-131">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="767af-131">Action is not supported.</span></span>|





