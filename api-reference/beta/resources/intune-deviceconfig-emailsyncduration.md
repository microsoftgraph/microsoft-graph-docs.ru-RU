---
title: Тип перечисления emailSyncDuration
description: Возможные значения для продолжительность синхронизации электронной почты.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d83a1ceb82820ddc44d8753e8ed05e00de09e36e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819385"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="50a61-103">Тип перечисления emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="50a61-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="50a61-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="50a61-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50a61-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50a61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50a61-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="50a61-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50a61-107">Возможные значения для продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="50a61-107">Possible values for email sync duration.</span></span>
## <a name="members"></a><span data-ttu-id="50a61-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="50a61-108">Members</span></span>
|<span data-ttu-id="50a61-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="50a61-109">Member</span></span>|<span data-ttu-id="50a61-110">Значение</span><span class="sxs-lookup"><span data-stu-id="50a61-110">Value</span></span>|<span data-ttu-id="50a61-111">Описание</span><span class="sxs-lookup"><span data-stu-id="50a61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50a61-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="50a61-112">userDefined</span></span>|<span data-ttu-id="50a61-113">0</span><span class="sxs-lookup"><span data-stu-id="50a61-113">0</span></span>|<span data-ttu-id="50a61-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="50a61-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="50a61-115">oneDay</span><span class="sxs-lookup"><span data-stu-id="50a61-115">oneDay</span></span>|<span data-ttu-id="50a61-116">1</span><span class="sxs-lookup"><span data-stu-id="50a61-116">1</span></span>|<span data-ttu-id="50a61-117">Синхронизация электронной почты на один день.</span><span class="sxs-lookup"><span data-stu-id="50a61-117">Sync one day of email.</span></span>|
|<span data-ttu-id="50a61-118">threeDays</span><span class="sxs-lookup"><span data-stu-id="50a61-118">threeDays</span></span>|<span data-ttu-id="50a61-119">2</span><span class="sxs-lookup"><span data-stu-id="50a61-119">2</span></span>|<span data-ttu-id="50a61-120">Синхронизация электронной почты на три дня.</span><span class="sxs-lookup"><span data-stu-id="50a61-120">Sync three days of email.</span></span>|
|<span data-ttu-id="50a61-121">oneWeek</span><span class="sxs-lookup"><span data-stu-id="50a61-121">oneWeek</span></span>|<span data-ttu-id="50a61-122">3</span><span class="sxs-lookup"><span data-stu-id="50a61-122">3</span></span>|<span data-ttu-id="50a61-123">Синхронизация неделю сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="50a61-123">Sync one week of email.</span></span>|
|<span data-ttu-id="50a61-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="50a61-124">twoWeeks</span></span>|<span data-ttu-id="50a61-125">4</span><span class="sxs-lookup"><span data-stu-id="50a61-125">4</span></span>|<span data-ttu-id="50a61-126">Синхронизация две недели по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="50a61-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="50a61-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="50a61-127">oneMonth</span></span>|<span data-ttu-id="50a61-128">5</span><span class="sxs-lookup"><span data-stu-id="50a61-128">5</span></span>|<span data-ttu-id="50a61-129">Синхронизация месяц сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="50a61-129">Sync one month of email.</span></span>|
|<span data-ttu-id="50a61-130">без ограничений</span><span class="sxs-lookup"><span data-stu-id="50a61-130">unlimited</span></span>|<span data-ttu-id="50a61-131">6</span><span class="sxs-lookup"><span data-stu-id="50a61-131">6</span></span>|<span data-ttu-id="50a61-132">Синхронизируйте неограниченное время сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="50a61-132">Sync an unlimited duration of email.</span></span>|





