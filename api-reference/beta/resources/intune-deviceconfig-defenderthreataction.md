---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3d93ed616a73c69467a1a77cb27e6fb27a7ea553
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024299"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="fd954-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="fd954-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="fd954-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd954-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd954-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd954-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd954-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd954-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd954-107">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="fd954-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="fd954-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fd954-108">Members</span></span>
|<span data-ttu-id="fd954-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fd954-109">Member</span></span>|<span data-ttu-id="fd954-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fd954-110">Value</span></span>|<span data-ttu-id="fd954-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fd954-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd954-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="fd954-112">deviceDefault</span></span>|<span data-ttu-id="fd954-113">нуль</span><span class="sxs-lookup"><span data-stu-id="fd954-113">0</span></span>|<span data-ttu-id="fd954-114">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="fd954-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="fd954-115">чистить</span><span class="sxs-lookup"><span data-stu-id="fd954-115">clean</span></span>|<span data-ttu-id="fd954-116">1 </span><span class="sxs-lookup"><span data-stu-id="fd954-116">1</span></span>|<span data-ttu-id="fd954-117">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="fd954-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="fd954-118">папку</span><span class="sxs-lookup"><span data-stu-id="fd954-118">quarantine</span></span>|<span data-ttu-id="fd954-119">2 </span><span class="sxs-lookup"><span data-stu-id="fd954-119">2</span></span>|<span data-ttu-id="fd954-120">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="fd954-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="fd954-121">удалить</span><span class="sxs-lookup"><span data-stu-id="fd954-121">remove</span></span>|<span data-ttu-id="fd954-122">4</span><span class="sxs-lookup"><span data-stu-id="fd954-122">3</span></span>|<span data-ttu-id="fd954-123">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="fd954-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="fd954-124">разрешить</span><span class="sxs-lookup"><span data-stu-id="fd954-124">allow</span></span>|<span data-ttu-id="fd954-125">4 </span><span class="sxs-lookup"><span data-stu-id="fd954-125">4</span></span>|<span data-ttu-id="fd954-126">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="fd954-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="fd954-127">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="fd954-127">userDefined</span></span>|<span data-ttu-id="fd954-128">5 </span><span class="sxs-lookup"><span data-stu-id="fd954-128">5</span></span>|<span data-ttu-id="fd954-129">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="fd954-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="fd954-130">блок</span><span class="sxs-lookup"><span data-stu-id="fd954-130">block</span></span>|<span data-ttu-id="fd954-131">6 </span><span class="sxs-lookup"><span data-stu-id="fd954-131">6</span></span>|<span data-ttu-id="fd954-132">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="fd954-132">Block the detected threat.</span></span>|






