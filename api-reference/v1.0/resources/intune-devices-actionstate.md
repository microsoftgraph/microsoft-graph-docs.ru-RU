---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e06b492e41ffa5e2f9aa4b64782e96125ea746a2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261490"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="6d8b0-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="6d8b0-103">actionState enum type</span></span>

> <span data-ttu-id="6d8b0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d8b0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d8b0-105">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="6d8b0-105">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="6d8b0-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="6d8b0-106">Members</span></span>
|<span data-ttu-id="6d8b0-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="6d8b0-107">Member</span></span>|<span data-ttu-id="6d8b0-108">Значение</span><span class="sxs-lookup"><span data-stu-id="6d8b0-108">Value</span></span>|<span data-ttu-id="6d8b0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6d8b0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d8b0-110">Нет</span><span class="sxs-lookup"><span data-stu-id="6d8b0-110">none</span></span>|<span data-ttu-id="6d8b0-111">нуль</span><span class="sxs-lookup"><span data-stu-id="6d8b0-111">0</span></span>|<span data-ttu-id="6d8b0-112">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="6d8b0-112">Not a valid action state</span></span>|
|<span data-ttu-id="6d8b0-113">закончен</span><span class="sxs-lookup"><span data-stu-id="6d8b0-113">pending</span></span>|<span data-ttu-id="6d8b0-114">1,1</span><span class="sxs-lookup"><span data-stu-id="6d8b0-114">1</span></span>|<span data-ttu-id="6d8b0-115">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="6d8b0-115">Action is pending</span></span>|
|<span data-ttu-id="6d8b0-116">закрыт</span><span class="sxs-lookup"><span data-stu-id="6d8b0-116">canceled</span></span>|<span data-ttu-id="6d8b0-117">2</span><span class="sxs-lookup"><span data-stu-id="6d8b0-117">2</span></span>|<span data-ttu-id="6d8b0-118">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="6d8b0-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="6d8b0-119">ASP</span><span class="sxs-lookup"><span data-stu-id="6d8b0-119">active</span></span>|<span data-ttu-id="6d8b0-120">4</span><span class="sxs-lookup"><span data-stu-id="6d8b0-120">3</span></span>|<span data-ttu-id="6d8b0-121">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="6d8b0-121">Action is active.</span></span>|
|<span data-ttu-id="6d8b0-122">done</span><span class="sxs-lookup"><span data-stu-id="6d8b0-122">done</span></span>|<span data-ttu-id="6d8b0-123">4</span><span class="sxs-lookup"><span data-stu-id="6d8b0-123">4</span></span>|<span data-ttu-id="6d8b0-124">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="6d8b0-124">Action completed without errors.</span></span>|
|<span data-ttu-id="6d8b0-125">failed</span><span class="sxs-lookup"><span data-stu-id="6d8b0-125">failed</span></span>|<span data-ttu-id="6d8b0-126">17:00</span><span class="sxs-lookup"><span data-stu-id="6d8b0-126">5</span></span>|<span data-ttu-id="6d8b0-127">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="6d8b0-127">Action failed</span></span>|
|<span data-ttu-id="6d8b0-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="6d8b0-128">notSupported</span></span>|<span data-ttu-id="6d8b0-129">6</span><span class="sxs-lookup"><span data-stu-id="6d8b0-129">6</span></span>|<span data-ttu-id="6d8b0-130">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d8b0-130">Action is not supported.</span></span>|



