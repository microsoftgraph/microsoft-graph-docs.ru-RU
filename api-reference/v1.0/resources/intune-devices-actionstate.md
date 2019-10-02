---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4cd21f0ac93e59d551400e87886e5bc871fd55c9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357089"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="b92cc-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="b92cc-103">actionState enum type</span></span>

> <span data-ttu-id="b92cc-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b92cc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b92cc-105">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="b92cc-105">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="b92cc-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="b92cc-106">Members</span></span>
|<span data-ttu-id="b92cc-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="b92cc-107">Member</span></span>|<span data-ttu-id="b92cc-108">Значение</span><span class="sxs-lookup"><span data-stu-id="b92cc-108">Value</span></span>|<span data-ttu-id="b92cc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b92cc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b92cc-110">none</span><span class="sxs-lookup"><span data-stu-id="b92cc-110">none</span></span>|<span data-ttu-id="b92cc-111">нуль</span><span class="sxs-lookup"><span data-stu-id="b92cc-111">0</span></span>|<span data-ttu-id="b92cc-112">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="b92cc-112">Not a valid action state</span></span>|
|<span data-ttu-id="b92cc-113">закончен</span><span class="sxs-lookup"><span data-stu-id="b92cc-113">pending</span></span>|<span data-ttu-id="b92cc-114">1,1</span><span class="sxs-lookup"><span data-stu-id="b92cc-114">1</span></span>|<span data-ttu-id="b92cc-115">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="b92cc-115">Action is pending</span></span>|
|<span data-ttu-id="b92cc-116">закрыт</span><span class="sxs-lookup"><span data-stu-id="b92cc-116">canceled</span></span>|<span data-ttu-id="b92cc-117">2</span><span class="sxs-lookup"><span data-stu-id="b92cc-117">2</span></span>|<span data-ttu-id="b92cc-118">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="b92cc-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="b92cc-119">ASP</span><span class="sxs-lookup"><span data-stu-id="b92cc-119">active</span></span>|<span data-ttu-id="b92cc-120">4</span><span class="sxs-lookup"><span data-stu-id="b92cc-120">3</span></span>|<span data-ttu-id="b92cc-121">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="b92cc-121">Action is active.</span></span>|
|<span data-ttu-id="b92cc-122">done</span><span class="sxs-lookup"><span data-stu-id="b92cc-122">done</span></span>|<span data-ttu-id="b92cc-123">SP4</span><span class="sxs-lookup"><span data-stu-id="b92cc-123">4</span></span>|<span data-ttu-id="b92cc-124">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="b92cc-124">Action completed without errors.</span></span>|
|<span data-ttu-id="b92cc-125">сбоев</span><span class="sxs-lookup"><span data-stu-id="b92cc-125">failed</span></span>|<span data-ttu-id="b92cc-126">17:00</span><span class="sxs-lookup"><span data-stu-id="b92cc-126">5</span></span>|<span data-ttu-id="b92cc-127">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="b92cc-127">Action failed</span></span>|
|<span data-ttu-id="b92cc-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="b92cc-128">notSupported</span></span>|<span data-ttu-id="b92cc-129">6 </span><span class="sxs-lookup"><span data-stu-id="b92cc-129">6</span></span>|<span data-ttu-id="b92cc-130">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b92cc-130">Action is not supported.</span></span>|




