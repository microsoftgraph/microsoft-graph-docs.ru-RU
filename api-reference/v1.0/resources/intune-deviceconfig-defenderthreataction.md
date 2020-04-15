---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 24c2b0c60f0451b58e624558fd44f3628c92e3cc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448990"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="5c8ce-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="5c8ce-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="5c8ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c8ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c8ce-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c8ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c8ce-106">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="5c8ce-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="5c8ce-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5c8ce-107">Members</span></span>
|<span data-ttu-id="5c8ce-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5c8ce-108">Member</span></span>|<span data-ttu-id="5c8ce-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5c8ce-109">Value</span></span>|<span data-ttu-id="5c8ce-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5c8ce-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c8ce-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="5c8ce-111">deviceDefault</span></span>|<span data-ttu-id="5c8ce-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5c8ce-112">0</span></span>|<span data-ttu-id="5c8ce-113">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="5c8ce-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="5c8ce-114">чистить</span><span class="sxs-lookup"><span data-stu-id="5c8ce-114">clean</span></span>|<span data-ttu-id="5c8ce-115">1,1</span><span class="sxs-lookup"><span data-stu-id="5c8ce-115">1</span></span>|<span data-ttu-id="5c8ce-116">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="5c8ce-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="5c8ce-117">папку</span><span class="sxs-lookup"><span data-stu-id="5c8ce-117">quarantine</span></span>|<span data-ttu-id="5c8ce-118">2</span><span class="sxs-lookup"><span data-stu-id="5c8ce-118">2</span></span>|<span data-ttu-id="5c8ce-119">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="5c8ce-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="5c8ce-120">удалить</span><span class="sxs-lookup"><span data-stu-id="5c8ce-120">remove</span></span>|<span data-ttu-id="5c8ce-121">4</span><span class="sxs-lookup"><span data-stu-id="5c8ce-121">3</span></span>|<span data-ttu-id="5c8ce-122">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="5c8ce-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="5c8ce-123">разрешить</span><span class="sxs-lookup"><span data-stu-id="5c8ce-123">allow</span></span>|<span data-ttu-id="5c8ce-124">4 </span><span class="sxs-lookup"><span data-stu-id="5c8ce-124">4</span></span>|<span data-ttu-id="5c8ce-125">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="5c8ce-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="5c8ce-126">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="5c8ce-126">userDefined</span></span>|<span data-ttu-id="5c8ce-127">5 </span><span class="sxs-lookup"><span data-stu-id="5c8ce-127">5</span></span>|<span data-ttu-id="5c8ce-128">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="5c8ce-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="5c8ce-129">блок</span><span class="sxs-lookup"><span data-stu-id="5c8ce-129">block</span></span>|<span data-ttu-id="5c8ce-130">6 </span><span class="sxs-lookup"><span data-stu-id="5c8ce-130">6</span></span>|<span data-ttu-id="5c8ce-131">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="5c8ce-131">Block the detected threat.</span></span>|







