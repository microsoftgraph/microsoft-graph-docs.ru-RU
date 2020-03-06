---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e4c9edcd596d6dcd40b2cfe873b660651f74bb3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530858"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="be589-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="be589-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="be589-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be589-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be589-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be589-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be589-106">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="be589-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="be589-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="be589-107">Members</span></span>
|<span data-ttu-id="be589-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="be589-108">Member</span></span>|<span data-ttu-id="be589-109">Значение</span><span class="sxs-lookup"><span data-stu-id="be589-109">Value</span></span>|<span data-ttu-id="be589-110">Описание</span><span class="sxs-lookup"><span data-stu-id="be589-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be589-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="be589-111">deviceDefault</span></span>|<span data-ttu-id="be589-112">нуль</span><span class="sxs-lookup"><span data-stu-id="be589-112">0</span></span>|<span data-ttu-id="be589-113">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="be589-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="be589-114">чистить</span><span class="sxs-lookup"><span data-stu-id="be589-114">clean</span></span>|<span data-ttu-id="be589-115">1 </span><span class="sxs-lookup"><span data-stu-id="be589-115">1</span></span>|<span data-ttu-id="be589-116">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="be589-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="be589-117">папку</span><span class="sxs-lookup"><span data-stu-id="be589-117">quarantine</span></span>|<span data-ttu-id="be589-118">2 </span><span class="sxs-lookup"><span data-stu-id="be589-118">2</span></span>|<span data-ttu-id="be589-119">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="be589-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="be589-120">удалить</span><span class="sxs-lookup"><span data-stu-id="be589-120">remove</span></span>|<span data-ttu-id="be589-121">3 </span><span class="sxs-lookup"><span data-stu-id="be589-121">3</span></span>|<span data-ttu-id="be589-122">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="be589-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="be589-123">разрешить</span><span class="sxs-lookup"><span data-stu-id="be589-123">allow</span></span>|<span data-ttu-id="be589-124">4 </span><span class="sxs-lookup"><span data-stu-id="be589-124">4</span></span>|<span data-ttu-id="be589-125">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="be589-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="be589-126">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="be589-126">userDefined</span></span>|<span data-ttu-id="be589-127">5 </span><span class="sxs-lookup"><span data-stu-id="be589-127">5</span></span>|<span data-ttu-id="be589-128">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="be589-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="be589-129">блок</span><span class="sxs-lookup"><span data-stu-id="be589-129">block</span></span>|<span data-ttu-id="be589-130">6 </span><span class="sxs-lookup"><span data-stu-id="be589-130">6</span></span>|<span data-ttu-id="be589-131">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="be589-131">Block the detected threat.</span></span>|




