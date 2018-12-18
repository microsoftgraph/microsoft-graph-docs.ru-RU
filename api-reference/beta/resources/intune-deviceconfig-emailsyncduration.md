---
title: Тип перечисления emailSyncDuration
description: Возможные значения для продолжительность синхронизации электронной почты.
author: tfitzmac
ms.openlocfilehash: 512e20ad13c13fdf92e45cfe0a37792d97e17fbb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361168"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="7b802-103">Тип перечисления emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="7b802-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="7b802-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b802-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b802-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b802-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b802-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7b802-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b802-107">Возможные значения для продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7b802-107">Possible values for email sync duration.</span></span>
## <a name="members"></a><span data-ttu-id="7b802-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="7b802-108">Members</span></span>
|<span data-ttu-id="7b802-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="7b802-109">Member</span></span>|<span data-ttu-id="7b802-110">Значение</span><span class="sxs-lookup"><span data-stu-id="7b802-110">Value</span></span>|<span data-ttu-id="7b802-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7b802-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b802-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="7b802-112">userDefined</span></span>|<span data-ttu-id="7b802-113">0</span><span class="sxs-lookup"><span data-stu-id="7b802-113">0</span></span>|<span data-ttu-id="7b802-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="7b802-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="7b802-115">oneDay</span><span class="sxs-lookup"><span data-stu-id="7b802-115">oneDay</span></span>|<span data-ttu-id="7b802-116">1</span><span class="sxs-lookup"><span data-stu-id="7b802-116">1</span></span>|<span data-ttu-id="7b802-117">Синхронизация электронной почты на один день.</span><span class="sxs-lookup"><span data-stu-id="7b802-117">Sync one day of email.</span></span>|
|<span data-ttu-id="7b802-118">threeDays</span><span class="sxs-lookup"><span data-stu-id="7b802-118">threeDays</span></span>|<span data-ttu-id="7b802-119">2</span><span class="sxs-lookup"><span data-stu-id="7b802-119">2</span></span>|<span data-ttu-id="7b802-120">Синхронизация электронной почты на три дня.</span><span class="sxs-lookup"><span data-stu-id="7b802-120">Sync three days of email.</span></span>|
|<span data-ttu-id="7b802-121">oneWeek</span><span class="sxs-lookup"><span data-stu-id="7b802-121">oneWeek</span></span>|<span data-ttu-id="7b802-122">3</span><span class="sxs-lookup"><span data-stu-id="7b802-122">3</span></span>|<span data-ttu-id="7b802-123">Синхронизация неделю сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7b802-123">Sync one week of email.</span></span>|
|<span data-ttu-id="7b802-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="7b802-124">twoWeeks</span></span>|<span data-ttu-id="7b802-125">4</span><span class="sxs-lookup"><span data-stu-id="7b802-125">4</span></span>|<span data-ttu-id="7b802-126">Синхронизация две недели по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="7b802-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="7b802-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="7b802-127">oneMonth</span></span>|<span data-ttu-id="7b802-128">5</span><span class="sxs-lookup"><span data-stu-id="7b802-128">5</span></span>|<span data-ttu-id="7b802-129">Синхронизация месяц сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7b802-129">Sync one month of email.</span></span>|
|<span data-ttu-id="7b802-130">без ограничений</span><span class="sxs-lookup"><span data-stu-id="7b802-130">unlimited</span></span>|<span data-ttu-id="7b802-131">6</span><span class="sxs-lookup"><span data-stu-id="7b802-131">6</span></span>|<span data-ttu-id="7b802-132">Синхронизируйте неограниченное время сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7b802-132">Sync an unlimited duration of email.</span></span>|





