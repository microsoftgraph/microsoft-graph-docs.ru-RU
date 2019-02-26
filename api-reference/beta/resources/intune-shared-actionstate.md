---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d55ff0419c6178668bbee921c149c8bc797ebff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143402"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="65d39-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="65d39-103">actionState enum type</span></span>

> <span data-ttu-id="65d39-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65d39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65d39-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65d39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65d39-106">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="65d39-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="65d39-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="65d39-107">Members</span></span>
|<span data-ttu-id="65d39-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="65d39-108">Member</span></span>|<span data-ttu-id="65d39-109">Значение</span><span class="sxs-lookup"><span data-stu-id="65d39-109">Value</span></span>|<span data-ttu-id="65d39-110">Описание</span><span class="sxs-lookup"><span data-stu-id="65d39-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65d39-111">Нет</span><span class="sxs-lookup"><span data-stu-id="65d39-111">none</span></span>|<span data-ttu-id="65d39-112">нуль</span><span class="sxs-lookup"><span data-stu-id="65d39-112">0</span></span>|<span data-ttu-id="65d39-113">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="65d39-113">Not a valid action state</span></span>|
|<span data-ttu-id="65d39-114">закончен</span><span class="sxs-lookup"><span data-stu-id="65d39-114">pending</span></span>|<span data-ttu-id="65d39-115">1,1</span><span class="sxs-lookup"><span data-stu-id="65d39-115">1</span></span>|<span data-ttu-id="65d39-116">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="65d39-116">Action is pending</span></span>|
|<span data-ttu-id="65d39-117">закрыт</span><span class="sxs-lookup"><span data-stu-id="65d39-117">canceled</span></span>|<span data-ttu-id="65d39-118">2</span><span class="sxs-lookup"><span data-stu-id="65d39-118">2</span></span>|<span data-ttu-id="65d39-119">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="65d39-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="65d39-120">ASP</span><span class="sxs-lookup"><span data-stu-id="65d39-120">active</span></span>|<span data-ttu-id="65d39-121">4</span><span class="sxs-lookup"><span data-stu-id="65d39-121">3</span></span>|<span data-ttu-id="65d39-122">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="65d39-122">Action is active.</span></span>|
|<span data-ttu-id="65d39-123">done</span><span class="sxs-lookup"><span data-stu-id="65d39-123">done</span></span>|<span data-ttu-id="65d39-124">4</span><span class="sxs-lookup"><span data-stu-id="65d39-124">4</span></span>|<span data-ttu-id="65d39-125">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="65d39-125">Action completed without errors.</span></span>|
|<span data-ttu-id="65d39-126">failed</span><span class="sxs-lookup"><span data-stu-id="65d39-126">failed</span></span>|<span data-ttu-id="65d39-127">17:00</span><span class="sxs-lookup"><span data-stu-id="65d39-127">5</span></span>|<span data-ttu-id="65d39-128">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="65d39-128">Action failed</span></span>|
|<span data-ttu-id="65d39-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="65d39-129">notSupported</span></span>|<span data-ttu-id="65d39-130">6</span><span class="sxs-lookup"><span data-stu-id="65d39-130">6</span></span>|<span data-ttu-id="65d39-131">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65d39-131">Action is not supported.</span></span>|




