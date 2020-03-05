---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e11fc186dcfe16005e3ceaab5c6306f5893a8598
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418169"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="cac0c-103">тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="cac0c-103">actionState enum type</span></span>

<span data-ttu-id="cac0c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cac0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cac0c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cac0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cac0c-106">Состояние действия на устройстве</span><span class="sxs-lookup"><span data-stu-id="cac0c-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="cac0c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="cac0c-107">Members</span></span>
|<span data-ttu-id="cac0c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="cac0c-108">Member</span></span>|<span data-ttu-id="cac0c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="cac0c-109">Value</span></span>|<span data-ttu-id="cac0c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cac0c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cac0c-111">нет</span><span class="sxs-lookup"><span data-stu-id="cac0c-111">none</span></span>|<span data-ttu-id="cac0c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="cac0c-112">0</span></span>|<span data-ttu-id="cac0c-113">Недопустимое состояние действия</span><span class="sxs-lookup"><span data-stu-id="cac0c-113">Not a valid action state</span></span>|
|<span data-ttu-id="cac0c-114">закончен</span><span class="sxs-lookup"><span data-stu-id="cac0c-114">pending</span></span>|<span data-ttu-id="cac0c-115">1 </span><span class="sxs-lookup"><span data-stu-id="cac0c-115">1</span></span>|<span data-ttu-id="cac0c-116">Ожидается действие</span><span class="sxs-lookup"><span data-stu-id="cac0c-116">Action is pending</span></span>|
|<span data-ttu-id="cac0c-117">закрыт</span><span class="sxs-lookup"><span data-stu-id="cac0c-117">canceled</span></span>|<span data-ttu-id="cac0c-118">2 </span><span class="sxs-lookup"><span data-stu-id="cac0c-118">2</span></span>|<span data-ttu-id="cac0c-119">Действие отменено.</span><span class="sxs-lookup"><span data-stu-id="cac0c-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="cac0c-120">ASP</span><span class="sxs-lookup"><span data-stu-id="cac0c-120">active</span></span>|<span data-ttu-id="cac0c-121">3 </span><span class="sxs-lookup"><span data-stu-id="cac0c-121">3</span></span>|<span data-ttu-id="cac0c-122">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="cac0c-122">Action is active.</span></span>|
|<span data-ttu-id="cac0c-123">done</span><span class="sxs-lookup"><span data-stu-id="cac0c-123">done</span></span>|<span data-ttu-id="cac0c-124">4 </span><span class="sxs-lookup"><span data-stu-id="cac0c-124">4</span></span>|<span data-ttu-id="cac0c-125">Действие выполнено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="cac0c-125">Action completed without errors.</span></span>|
|<span data-ttu-id="cac0c-126">сбоев</span><span class="sxs-lookup"><span data-stu-id="cac0c-126">failed</span></span>|<span data-ttu-id="cac0c-127">5 </span><span class="sxs-lookup"><span data-stu-id="cac0c-127">5</span></span>|<span data-ttu-id="cac0c-128">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="cac0c-128">Action failed</span></span>|
|<span data-ttu-id="cac0c-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="cac0c-129">notSupported</span></span>|<span data-ttu-id="cac0c-130">6 </span><span class="sxs-lookup"><span data-stu-id="cac0c-130">6</span></span>|<span data-ttu-id="cac0c-131">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cac0c-131">Action is not supported.</span></span>|




