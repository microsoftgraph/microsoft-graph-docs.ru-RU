---
title: тип перечисления Емаилсинкдуратион
description: Возможные значения срока действия синхронизации электронной почты.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4c199f55d78f14ca7e77a24a0e1c62762b51afb3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705962"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="5f17c-103">тип перечисления Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="5f17c-103">emailSyncDuration enum type</span></span>

<span data-ttu-id="5f17c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f17c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f17c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f17c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f17c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f17c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f17c-107">Возможные значения срока действия синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5f17c-107">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="5f17c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="5f17c-108">Members</span></span>
|<span data-ttu-id="5f17c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="5f17c-109">Member</span></span>|<span data-ttu-id="5f17c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="5f17c-110">Value</span></span>|<span data-ttu-id="5f17c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5f17c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f17c-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="5f17c-112">userDefined</span></span>|<span data-ttu-id="5f17c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="5f17c-113">0</span></span>|<span data-ttu-id="5f17c-114">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="5f17c-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="5f17c-115">онедай</span><span class="sxs-lookup"><span data-stu-id="5f17c-115">oneDay</span></span>|<span data-ttu-id="5f17c-116">1,1</span><span class="sxs-lookup"><span data-stu-id="5f17c-116">1</span></span>|<span data-ttu-id="5f17c-117">Синхронизация одного дня электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5f17c-117">Sync one day of email.</span></span>|
|<span data-ttu-id="5f17c-118">сридайс</span><span class="sxs-lookup"><span data-stu-id="5f17c-118">threeDays</span></span>|<span data-ttu-id="5f17c-119">2</span><span class="sxs-lookup"><span data-stu-id="5f17c-119">2</span></span>|<span data-ttu-id="5f17c-120">Синхронизация трех дней электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5f17c-120">Sync three days of email.</span></span>|
|<span data-ttu-id="5f17c-121">оневик</span><span class="sxs-lookup"><span data-stu-id="5f17c-121">oneWeek</span></span>|<span data-ttu-id="5f17c-122">4</span><span class="sxs-lookup"><span data-stu-id="5f17c-122">3</span></span>|<span data-ttu-id="5f17c-123">Синхронизация одной недели с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="5f17c-123">Sync one week of email.</span></span>|
|<span data-ttu-id="5f17c-124">твовикс</span><span class="sxs-lookup"><span data-stu-id="5f17c-124">twoWeeks</span></span>|<span data-ttu-id="5f17c-125">4 </span><span class="sxs-lookup"><span data-stu-id="5f17c-125">4</span></span>|<span data-ttu-id="5f17c-126">Синхронизируйте две недели с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="5f17c-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="5f17c-127">онемонс</span><span class="sxs-lookup"><span data-stu-id="5f17c-127">oneMonth</span></span>|<span data-ttu-id="5f17c-128">5 </span><span class="sxs-lookup"><span data-stu-id="5f17c-128">5</span></span>|<span data-ttu-id="5f17c-129">Синхронизируйте один месяц электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5f17c-129">Sync one month of email.</span></span>|
|<span data-ttu-id="5f17c-130">неограниченно</span><span class="sxs-lookup"><span data-stu-id="5f17c-130">unlimited</span></span>|<span data-ttu-id="5f17c-131">6 </span><span class="sxs-lookup"><span data-stu-id="5f17c-131">6</span></span>|<span data-ttu-id="5f17c-132">Синхронизация неограниченной длительности электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5f17c-132">Sync an unlimited duration of email.</span></span>|





