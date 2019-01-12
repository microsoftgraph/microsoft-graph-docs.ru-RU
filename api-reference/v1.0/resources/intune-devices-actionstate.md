---
title: Тип перечисления состояние действия
description: Состояние действие на устройстве
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5579d8de986a764cd96e42dff30c007449130b0b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922447"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="01eed-103">Тип перечисления состояние действия</span><span class="sxs-lookup"><span data-stu-id="01eed-103">actionState enum type</span></span>

> <span data-ttu-id="01eed-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="01eed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01eed-105">Состояние действие на устройстве</span><span class="sxs-lookup"><span data-stu-id="01eed-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="01eed-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="01eed-106">Members</span></span>
|<span data-ttu-id="01eed-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="01eed-107">Member</span></span>|<span data-ttu-id="01eed-108">Значение</span><span class="sxs-lookup"><span data-stu-id="01eed-108">Value</span></span>|<span data-ttu-id="01eed-109">Описание</span><span class="sxs-lookup"><span data-stu-id="01eed-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01eed-110">Нет</span><span class="sxs-lookup"><span data-stu-id="01eed-110">none</span></span>|<span data-ttu-id="01eed-111">0</span><span class="sxs-lookup"><span data-stu-id="01eed-111">0</span></span>|<span data-ttu-id="01eed-112">Не имеет состояние допустимое действие</span><span class="sxs-lookup"><span data-stu-id="01eed-112">Not a valid action state</span></span>|
|<span data-ttu-id="01eed-113">Ожидание</span><span class="sxs-lookup"><span data-stu-id="01eed-113">pending</span></span>|<span data-ttu-id="01eed-114">1</span><span class="sxs-lookup"><span data-stu-id="01eed-114">1</span></span>|<span data-ttu-id="01eed-115">Действие находится в состоянии ожидания</span><span class="sxs-lookup"><span data-stu-id="01eed-115">Action is pending</span></span>|
|<span data-ttu-id="01eed-116">отменено</span><span class="sxs-lookup"><span data-stu-id="01eed-116">canceled</span></span>|<span data-ttu-id="01eed-117">2</span><span class="sxs-lookup"><span data-stu-id="01eed-117">2</span></span>|<span data-ttu-id="01eed-118">Действие было отменено.</span><span class="sxs-lookup"><span data-stu-id="01eed-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="01eed-119">активных</span><span class="sxs-lookup"><span data-stu-id="01eed-119">active</span></span>|<span data-ttu-id="01eed-120">3</span><span class="sxs-lookup"><span data-stu-id="01eed-120">3</span></span>|<span data-ttu-id="01eed-121">Действие — active.</span><span class="sxs-lookup"><span data-stu-id="01eed-121">Action is active.</span></span>|
|<span data-ttu-id="01eed-122">done</span><span class="sxs-lookup"><span data-stu-id="01eed-122">done</span></span>|<span data-ttu-id="01eed-123">4</span><span class="sxs-lookup"><span data-stu-id="01eed-123">4</span></span>|<span data-ttu-id="01eed-124">Действие завершается без ошибок.</span><span class="sxs-lookup"><span data-stu-id="01eed-124">Action completed without errors.</span></span>|
|<span data-ttu-id="01eed-125">failed</span><span class="sxs-lookup"><span data-stu-id="01eed-125">failed</span></span>|<span data-ttu-id="01eed-126">5</span><span class="sxs-lookup"><span data-stu-id="01eed-126">5</span></span>|<span data-ttu-id="01eed-127">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="01eed-127">Action failed</span></span>|
|<span data-ttu-id="01eed-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="01eed-128">notSupported</span></span>|<span data-ttu-id="01eed-129">6</span><span class="sxs-lookup"><span data-stu-id="01eed-129">6</span></span>|<span data-ttu-id="01eed-130">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01eed-130">Action is not supported.</span></span>|



