---
title: тип перечисления Емаилсинкдуратион
description: Возможные значения срока действия синхронизации электронной почты.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 64dbd2e5321affeacc45eeccc63ad76b862f70db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003733"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="30a6f-103">тип перечисления Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="30a6f-103">emailSyncDuration enum type</span></span>

<span data-ttu-id="30a6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30a6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30a6f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30a6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30a6f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30a6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30a6f-107">Возможные значения срока действия синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="30a6f-107">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="30a6f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="30a6f-108">Members</span></span>
|<span data-ttu-id="30a6f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="30a6f-109">Member</span></span>|<span data-ttu-id="30a6f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="30a6f-110">Value</span></span>|<span data-ttu-id="30a6f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="30a6f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30a6f-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="30a6f-112">userDefined</span></span>|<span data-ttu-id="30a6f-113">нуль</span><span class="sxs-lookup"><span data-stu-id="30a6f-113">0</span></span>|<span data-ttu-id="30a6f-114">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="30a6f-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="30a6f-115">онедай</span><span class="sxs-lookup"><span data-stu-id="30a6f-115">oneDay</span></span>|<span data-ttu-id="30a6f-116">1 </span><span class="sxs-lookup"><span data-stu-id="30a6f-116">1</span></span>|<span data-ttu-id="30a6f-117">Синхронизация одного дня электронной почты.</span><span class="sxs-lookup"><span data-stu-id="30a6f-117">Sync one day of email.</span></span>|
|<span data-ttu-id="30a6f-118">сридайс</span><span class="sxs-lookup"><span data-stu-id="30a6f-118">threeDays</span></span>|<span data-ttu-id="30a6f-119">2 </span><span class="sxs-lookup"><span data-stu-id="30a6f-119">2</span></span>|<span data-ttu-id="30a6f-120">Синхронизация трех дней электронной почты.</span><span class="sxs-lookup"><span data-stu-id="30a6f-120">Sync three days of email.</span></span>|
|<span data-ttu-id="30a6f-121">оневик</span><span class="sxs-lookup"><span data-stu-id="30a6f-121">oneWeek</span></span>|<span data-ttu-id="30a6f-122">4</span><span class="sxs-lookup"><span data-stu-id="30a6f-122">3</span></span>|<span data-ttu-id="30a6f-123">Синхронизация одной недели с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="30a6f-123">Sync one week of email.</span></span>|
|<span data-ttu-id="30a6f-124">твовикс</span><span class="sxs-lookup"><span data-stu-id="30a6f-124">twoWeeks</span></span>|<span data-ttu-id="30a6f-125">4 </span><span class="sxs-lookup"><span data-stu-id="30a6f-125">4</span></span>|<span data-ttu-id="30a6f-126">Синхронизируйте две недели с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="30a6f-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="30a6f-127">онемонс</span><span class="sxs-lookup"><span data-stu-id="30a6f-127">oneMonth</span></span>|<span data-ttu-id="30a6f-128">5 </span><span class="sxs-lookup"><span data-stu-id="30a6f-128">5</span></span>|<span data-ttu-id="30a6f-129">Синхронизируйте один месяц электронной почты.</span><span class="sxs-lookup"><span data-stu-id="30a6f-129">Sync one month of email.</span></span>|
|<span data-ttu-id="30a6f-130">неограниченно</span><span class="sxs-lookup"><span data-stu-id="30a6f-130">unlimited</span></span>|<span data-ttu-id="30a6f-131">6 </span><span class="sxs-lookup"><span data-stu-id="30a6f-131">6</span></span>|<span data-ttu-id="30a6f-132">Синхронизация неограниченной длительности электронной почты.</span><span class="sxs-lookup"><span data-stu-id="30a6f-132">Sync an unlimited duration of email.</span></span>|






