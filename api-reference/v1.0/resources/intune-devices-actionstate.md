---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d0544d0783109ca5f3616981c06ee330bfddea06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091329"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="e30a0-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="e30a0-103">actionState enum type</span></span>

<span data-ttu-id="e30a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e30a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e30a0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e30a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e30a0-106">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="e30a0-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="e30a0-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e30a0-107">Members</span></span>
|<span data-ttu-id="e30a0-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e30a0-108">Member</span></span>|<span data-ttu-id="e30a0-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e30a0-109">Value</span></span>|<span data-ttu-id="e30a0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e30a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e30a0-111">Нет</span><span class="sxs-lookup"><span data-stu-id="e30a0-111">none</span></span>|<span data-ttu-id="e30a0-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e30a0-112">0</span></span>|<span data-ttu-id="e30a0-113">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="e30a0-113">Not a valid action state</span></span>|
|<span data-ttu-id="e30a0-114">закончен</span><span class="sxs-lookup"><span data-stu-id="e30a0-114">pending</span></span>|<span data-ttu-id="e30a0-115">1 </span><span class="sxs-lookup"><span data-stu-id="e30a0-115">1</span></span>|<span data-ttu-id="e30a0-116">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="e30a0-116">Action is pending</span></span>|
|<span data-ttu-id="e30a0-117">закрыт</span><span class="sxs-lookup"><span data-stu-id="e30a0-117">canceled</span></span>|<span data-ttu-id="e30a0-118">2 </span><span class="sxs-lookup"><span data-stu-id="e30a0-118">2</span></span>|<span data-ttu-id="e30a0-119">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="e30a0-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="e30a0-120">ASP</span><span class="sxs-lookup"><span data-stu-id="e30a0-120">active</span></span>|<span data-ttu-id="e30a0-121">4</span><span class="sxs-lookup"><span data-stu-id="e30a0-121">3</span></span>|<span data-ttu-id="e30a0-122">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="e30a0-122">Action is active.</span></span>|
|<span data-ttu-id="e30a0-123">done</span><span class="sxs-lookup"><span data-stu-id="e30a0-123">done</span></span>|<span data-ttu-id="e30a0-124">4 </span><span class="sxs-lookup"><span data-stu-id="e30a0-124">4</span></span>|<span data-ttu-id="e30a0-125">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="e30a0-125">Action completed without errors.</span></span>|
|<span data-ttu-id="e30a0-126">сбоев</span><span class="sxs-lookup"><span data-stu-id="e30a0-126">failed</span></span>|<span data-ttu-id="e30a0-127">5 </span><span class="sxs-lookup"><span data-stu-id="e30a0-127">5</span></span>|<span data-ttu-id="e30a0-128">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="e30a0-128">Action failed</span></span>|
|<span data-ttu-id="e30a0-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="e30a0-129">notSupported</span></span>|<span data-ttu-id="e30a0-130">6 </span><span class="sxs-lookup"><span data-stu-id="e30a0-130">6</span></span>|<span data-ttu-id="e30a0-131">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e30a0-131">Action is not supported.</span></span>|









