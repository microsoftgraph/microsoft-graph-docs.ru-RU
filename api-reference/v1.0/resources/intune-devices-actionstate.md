---
title: Тип перечисления состояние действия
description: Состояние действие на устройстве
author: tfitzmac
ms.openlocfilehash: 53ee72430ac646bf978a3167b87feaf398c8ac37
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333385"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="2d256-103">Тип перечисления состояние действия</span><span class="sxs-lookup"><span data-stu-id="2d256-103">actionState enum type</span></span>

> <span data-ttu-id="2d256-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2d256-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d256-105">Состояние действие на устройстве</span><span class="sxs-lookup"><span data-stu-id="2d256-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="2d256-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="2d256-106">Members</span></span>
|<span data-ttu-id="2d256-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="2d256-107">Member</span></span>|<span data-ttu-id="2d256-108">Значение</span><span class="sxs-lookup"><span data-stu-id="2d256-108">Value</span></span>|<span data-ttu-id="2d256-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2d256-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d256-110">none</span><span class="sxs-lookup"><span data-stu-id="2d256-110">none</span></span>|<span data-ttu-id="2d256-111">0</span><span class="sxs-lookup"><span data-stu-id="2d256-111">0</span></span>|<span data-ttu-id="2d256-112">Не имеет состояние допустимое действие</span><span class="sxs-lookup"><span data-stu-id="2d256-112">Not a valid action state</span></span>|
|<span data-ttu-id="2d256-113">Ожидание</span><span class="sxs-lookup"><span data-stu-id="2d256-113">pending</span></span>|<span data-ttu-id="2d256-114">1</span><span class="sxs-lookup"><span data-stu-id="2d256-114">1</span></span>|<span data-ttu-id="2d256-115">Действие находится в состоянии ожидания</span><span class="sxs-lookup"><span data-stu-id="2d256-115">Action is pending</span></span>|
|<span data-ttu-id="2d256-116">отменено</span><span class="sxs-lookup"><span data-stu-id="2d256-116">canceled</span></span>|<span data-ttu-id="2d256-117">2</span><span class="sxs-lookup"><span data-stu-id="2d256-117">2</span></span>|<span data-ttu-id="2d256-118">Действие было отменено.</span><span class="sxs-lookup"><span data-stu-id="2d256-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="2d256-119">активных</span><span class="sxs-lookup"><span data-stu-id="2d256-119">active</span></span>|<span data-ttu-id="2d256-120">3</span><span class="sxs-lookup"><span data-stu-id="2d256-120">3</span></span>|<span data-ttu-id="2d256-121">Действие — active.</span><span class="sxs-lookup"><span data-stu-id="2d256-121">Action is active.</span></span>|
|<span data-ttu-id="2d256-122">done</span><span class="sxs-lookup"><span data-stu-id="2d256-122">done</span></span>|<span data-ttu-id="2d256-123">4</span><span class="sxs-lookup"><span data-stu-id="2d256-123">4</span></span>|<span data-ttu-id="2d256-124">Действие завершается без ошибок.</span><span class="sxs-lookup"><span data-stu-id="2d256-124">Action completed without errors.</span></span>|
|<span data-ttu-id="2d256-125">failed</span><span class="sxs-lookup"><span data-stu-id="2d256-125">failed</span></span>|<span data-ttu-id="2d256-126">5</span><span class="sxs-lookup"><span data-stu-id="2d256-126">5</span></span>|<span data-ttu-id="2d256-127">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="2d256-127">Action failed</span></span>|
|<span data-ttu-id="2d256-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="2d256-128">notSupported</span></span>|<span data-ttu-id="2d256-129">6</span><span class="sxs-lookup"><span data-stu-id="2d256-129">6</span></span>|<span data-ttu-id="2d256-130">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d256-130">Action is not supported.</span></span>|



