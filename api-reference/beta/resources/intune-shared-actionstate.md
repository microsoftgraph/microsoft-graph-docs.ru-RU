---
title: Тип перечисления состояние действия
description: Состояние действие на устройстве
ms.openlocfilehash: e0169bd690cdc8a26cc771948ebcf311f6fd6aa5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078056"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="8afe6-103">Тип перечисления состояние действия</span><span class="sxs-lookup"><span data-stu-id="8afe6-103">actionState enum type</span></span>

> <span data-ttu-id="8afe6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8afe6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8afe6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8afe6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8afe6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8afe6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8afe6-107">Состояние действие на устройстве</span><span class="sxs-lookup"><span data-stu-id="8afe6-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="8afe6-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8afe6-108">Members</span></span>
|<span data-ttu-id="8afe6-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8afe6-109">Member</span></span>|<span data-ttu-id="8afe6-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8afe6-110">Value</span></span>|<span data-ttu-id="8afe6-111">Description</span><span class="sxs-lookup"><span data-stu-id="8afe6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8afe6-112">Нет</span><span class="sxs-lookup"><span data-stu-id="8afe6-112">none</span></span>|<span data-ttu-id="8afe6-113">0</span><span class="sxs-lookup"><span data-stu-id="8afe6-113">0</span></span>|<span data-ttu-id="8afe6-114">Не имеет состояние допустимое действие</span><span class="sxs-lookup"><span data-stu-id="8afe6-114">Not a valid action state</span></span>|
|<span data-ttu-id="8afe6-115">Ожидание</span><span class="sxs-lookup"><span data-stu-id="8afe6-115">pending</span></span>|<span data-ttu-id="8afe6-116">1</span><span class="sxs-lookup"><span data-stu-id="8afe6-116">1</span></span>|<span data-ttu-id="8afe6-117">Действие находится в состоянии ожидания</span><span class="sxs-lookup"><span data-stu-id="8afe6-117">Action is pending</span></span>|
|<span data-ttu-id="8afe6-118">отменено</span><span class="sxs-lookup"><span data-stu-id="8afe6-118">canceled</span></span>|<span data-ttu-id="8afe6-119">2</span><span class="sxs-lookup"><span data-stu-id="8afe6-119">2</span></span>|<span data-ttu-id="8afe6-120">Действие было отменено.</span><span class="sxs-lookup"><span data-stu-id="8afe6-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="8afe6-121">активных</span><span class="sxs-lookup"><span data-stu-id="8afe6-121">active</span></span>|<span data-ttu-id="8afe6-122">3</span><span class="sxs-lookup"><span data-stu-id="8afe6-122">3</span></span>|<span data-ttu-id="8afe6-123">Действие — active.</span><span class="sxs-lookup"><span data-stu-id="8afe6-123">Action is active.</span></span>|
|<span data-ttu-id="8afe6-124">done</span><span class="sxs-lookup"><span data-stu-id="8afe6-124">done</span></span>|<span data-ttu-id="8afe6-125">4</span><span class="sxs-lookup"><span data-stu-id="8afe6-125">4</span></span>|<span data-ttu-id="8afe6-126">Действие завершается без ошибок.</span><span class="sxs-lookup"><span data-stu-id="8afe6-126">Action completed without errors.</span></span>|
|<span data-ttu-id="8afe6-127">failed</span><span class="sxs-lookup"><span data-stu-id="8afe6-127">failed</span></span>|<span data-ttu-id="8afe6-128">5</span><span class="sxs-lookup"><span data-stu-id="8afe6-128">5</span></span>|<span data-ttu-id="8afe6-129">Не удалось выполнить действие</span><span class="sxs-lookup"><span data-stu-id="8afe6-129">Action failed</span></span>|
|<span data-ttu-id="8afe6-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="8afe6-130">notSupported</span></span>|<span data-ttu-id="8afe6-131">6</span><span class="sxs-lookup"><span data-stu-id="8afe6-131">6</span></span>|<span data-ttu-id="8afe6-132">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8afe6-132">Action is not supported.</span></span>|





