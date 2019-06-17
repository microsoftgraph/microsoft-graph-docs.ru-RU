---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35fccdc65eec7781f38d366e31ddb1a626005169
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996227"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="1d0ea-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="1d0ea-103">actionState enum type</span></span>

> <span data-ttu-id="1d0ea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d0ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d0ea-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d0ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d0ea-106">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="1d0ea-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="1d0ea-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="1d0ea-107">Members</span></span>
|<span data-ttu-id="1d0ea-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="1d0ea-108">Member</span></span>|<span data-ttu-id="1d0ea-109">Значение</span><span class="sxs-lookup"><span data-stu-id="1d0ea-109">Value</span></span>|<span data-ttu-id="1d0ea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1d0ea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d0ea-111">none</span><span class="sxs-lookup"><span data-stu-id="1d0ea-111">none</span></span>|<span data-ttu-id="1d0ea-112">нуль</span><span class="sxs-lookup"><span data-stu-id="1d0ea-112">0</span></span>|<span data-ttu-id="1d0ea-113">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="1d0ea-113">Not a valid action state</span></span>|
|<span data-ttu-id="1d0ea-114">закончен</span><span class="sxs-lookup"><span data-stu-id="1d0ea-114">pending</span></span>|<span data-ttu-id="1d0ea-115">1,1</span><span class="sxs-lookup"><span data-stu-id="1d0ea-115">1</span></span>|<span data-ttu-id="1d0ea-116">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="1d0ea-116">Action is pending</span></span>|
|<span data-ttu-id="1d0ea-117">закрыт</span><span class="sxs-lookup"><span data-stu-id="1d0ea-117">canceled</span></span>|<span data-ttu-id="1d0ea-118">2</span><span class="sxs-lookup"><span data-stu-id="1d0ea-118">2</span></span>|<span data-ttu-id="1d0ea-119">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="1d0ea-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="1d0ea-120">ASP</span><span class="sxs-lookup"><span data-stu-id="1d0ea-120">active</span></span>|<span data-ttu-id="1d0ea-121">4</span><span class="sxs-lookup"><span data-stu-id="1d0ea-121">3</span></span>|<span data-ttu-id="1d0ea-122">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="1d0ea-122">Action is active.</span></span>|
|<span data-ttu-id="1d0ea-123">done</span><span class="sxs-lookup"><span data-stu-id="1d0ea-123">done</span></span>|<span data-ttu-id="1d0ea-124">SP4</span><span class="sxs-lookup"><span data-stu-id="1d0ea-124">4</span></span>|<span data-ttu-id="1d0ea-125">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="1d0ea-125">Action completed without errors.</span></span>|
|<span data-ttu-id="1d0ea-126">сбоев</span><span class="sxs-lookup"><span data-stu-id="1d0ea-126">failed</span></span>|<span data-ttu-id="1d0ea-127">17:00</span><span class="sxs-lookup"><span data-stu-id="1d0ea-127">5</span></span>|<span data-ttu-id="1d0ea-128">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="1d0ea-128">Action failed</span></span>|
|<span data-ttu-id="1d0ea-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="1d0ea-129">notSupported</span></span>|<span data-ttu-id="1d0ea-130">6 </span><span class="sxs-lookup"><span data-stu-id="1d0ea-130">6</span></span>|<span data-ttu-id="1d0ea-131">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d0ea-131">Action is not supported.</span></span>|





