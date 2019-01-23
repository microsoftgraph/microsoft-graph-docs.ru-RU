---
title: Тип перечисления emailSyncDuration
description: Возможные значения для продолжительность синхронизации электронной почты.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8bf62aea1904c0fd25867aef308ca5a269e3ea20
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399411"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="cda51-103">Тип перечисления emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="cda51-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="cda51-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cda51-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cda51-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cda51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cda51-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cda51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cda51-107">Возможные значения для продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cda51-107">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="cda51-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="cda51-108">Members</span></span>
|<span data-ttu-id="cda51-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="cda51-109">Member</span></span>|<span data-ttu-id="cda51-110">Значение</span><span class="sxs-lookup"><span data-stu-id="cda51-110">Value</span></span>|<span data-ttu-id="cda51-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cda51-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cda51-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="cda51-112">userDefined</span></span>|<span data-ttu-id="cda51-113">0</span><span class="sxs-lookup"><span data-stu-id="cda51-113">0</span></span>|<span data-ttu-id="cda51-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="cda51-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="cda51-115">oneDay</span><span class="sxs-lookup"><span data-stu-id="cda51-115">oneDay</span></span>|<span data-ttu-id="cda51-116">1</span><span class="sxs-lookup"><span data-stu-id="cda51-116">1</span></span>|<span data-ttu-id="cda51-117">Синхронизация электронной почты на один день.</span><span class="sxs-lookup"><span data-stu-id="cda51-117">Sync one day of email.</span></span>|
|<span data-ttu-id="cda51-118">threeDays</span><span class="sxs-lookup"><span data-stu-id="cda51-118">threeDays</span></span>|<span data-ttu-id="cda51-119">2</span><span class="sxs-lookup"><span data-stu-id="cda51-119">2</span></span>|<span data-ttu-id="cda51-120">Синхронизация электронной почты на три дня.</span><span class="sxs-lookup"><span data-stu-id="cda51-120">Sync three days of email.</span></span>|
|<span data-ttu-id="cda51-121">oneWeek</span><span class="sxs-lookup"><span data-stu-id="cda51-121">oneWeek</span></span>|<span data-ttu-id="cda51-122">3</span><span class="sxs-lookup"><span data-stu-id="cda51-122">3</span></span>|<span data-ttu-id="cda51-123">Синхронизация неделю сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cda51-123">Sync one week of email.</span></span>|
|<span data-ttu-id="cda51-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="cda51-124">twoWeeks</span></span>|<span data-ttu-id="cda51-125">4</span><span class="sxs-lookup"><span data-stu-id="cda51-125">4</span></span>|<span data-ttu-id="cda51-126">Синхронизация две недели по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="cda51-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="cda51-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="cda51-127">oneMonth</span></span>|<span data-ttu-id="cda51-128">5</span><span class="sxs-lookup"><span data-stu-id="cda51-128">5</span></span>|<span data-ttu-id="cda51-129">Синхронизация месяц сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cda51-129">Sync one month of email.</span></span>|
|<span data-ttu-id="cda51-130">без ограничений</span><span class="sxs-lookup"><span data-stu-id="cda51-130">unlimited</span></span>|<span data-ttu-id="cda51-131">6</span><span class="sxs-lookup"><span data-stu-id="cda51-131">6</span></span>|<span data-ttu-id="cda51-132">Синхронизируйте неограниченное время сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cda51-132">Sync an unlimited duration of email.</span></span>|




