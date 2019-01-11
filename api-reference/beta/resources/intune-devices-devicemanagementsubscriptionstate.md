---
title: Тип перечисления deviceManagementSubscriptionState
description: Состояние подписки на управление мобильными устройствами для клиента.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a063252dcd3b65d85728550dd9ab616435a73472
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848372"
---
# <a name="devicemanagementsubscriptionstate-enum-type"></a><span data-ttu-id="9f2aa-103">Тип перечисления deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="9f2aa-103">deviceManagementSubscriptionState enum type</span></span>

> <span data-ttu-id="9f2aa-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9f2aa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f2aa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f2aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f2aa-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9f2aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f2aa-107">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f2aa-107">Tenant mobile device management subscription state.</span></span>
## <a name="members"></a><span data-ttu-id="9f2aa-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9f2aa-108">Members</span></span>
|<span data-ttu-id="9f2aa-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9f2aa-109">Member</span></span>|<span data-ttu-id="9f2aa-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9f2aa-110">Value</span></span>|<span data-ttu-id="9f2aa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9f2aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f2aa-112">Ожидание</span><span class="sxs-lookup"><span data-stu-id="9f2aa-112">pending</span></span>|<span data-ttu-id="9f2aa-113">0</span><span class="sxs-lookup"><span data-stu-id="9f2aa-113">0</span></span>|<span data-ttu-id="9f2aa-114">Pending</span><span class="sxs-lookup"><span data-stu-id="9f2aa-114">Pending</span></span>|
|<span data-ttu-id="9f2aa-115">активных</span><span class="sxs-lookup"><span data-stu-id="9f2aa-115">active</span></span>|<span data-ttu-id="9f2aa-116">1</span><span class="sxs-lookup"><span data-stu-id="9f2aa-116">1</span></span>|<span data-ttu-id="9f2aa-117">Active</span><span class="sxs-lookup"><span data-stu-id="9f2aa-117">Active</span></span>|
|<span data-ttu-id="9f2aa-118">warning</span><span class="sxs-lookup"><span data-stu-id="9f2aa-118">warning</span></span>|<span data-ttu-id="9f2aa-119">2</span><span class="sxs-lookup"><span data-stu-id="9f2aa-119">2</span></span>|<span data-ttu-id="9f2aa-120">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="9f2aa-120">Warning</span></span>|
|<span data-ttu-id="9f2aa-121">Этот параметр отключен</span><span class="sxs-lookup"><span data-stu-id="9f2aa-121">disabled</span></span>|<span data-ttu-id="9f2aa-122">3</span><span class="sxs-lookup"><span data-stu-id="9f2aa-122">3</span></span>|<span data-ttu-id="9f2aa-123">Отключена</span><span class="sxs-lookup"><span data-stu-id="9f2aa-123">Disabled</span></span>|
|<span data-ttu-id="9f2aa-124">deleted</span><span class="sxs-lookup"><span data-stu-id="9f2aa-124">deleted</span></span>|<span data-ttu-id="9f2aa-125">4</span><span class="sxs-lookup"><span data-stu-id="9f2aa-125">4</span></span>|<span data-ttu-id="9f2aa-126">Deleted</span><span class="sxs-lookup"><span data-stu-id="9f2aa-126">Deleted</span></span>|
|<span data-ttu-id="9f2aa-127">заблокировано</span><span class="sxs-lookup"><span data-stu-id="9f2aa-127">blocked</span></span>|<span data-ttu-id="9f2aa-128">5</span><span class="sxs-lookup"><span data-stu-id="9f2aa-128">5</span></span>|<span data-ttu-id="9f2aa-129">Blocked</span><span class="sxs-lookup"><span data-stu-id="9f2aa-129">Blocked</span></span>|
|<span data-ttu-id="9f2aa-130">lockedOut</span><span class="sxs-lookup"><span data-stu-id="9f2aa-130">lockedOut</span></span>|<span data-ttu-id="9f2aa-131">8</span><span class="sxs-lookup"><span data-stu-id="9f2aa-131">8</span></span>|<span data-ttu-id="9f2aa-132">LockedOut</span><span class="sxs-lookup"><span data-stu-id="9f2aa-132">LockedOut</span></span>|





