---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fda734d6d582f8b838e0dca26ae57c118f3438b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526834"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="c26ec-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="c26ec-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="c26ec-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c26ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c26ec-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c26ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c26ec-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c26ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c26ec-107">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="c26ec-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="c26ec-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c26ec-108">Members</span></span>
|<span data-ttu-id="c26ec-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c26ec-109">Member</span></span>|<span data-ttu-id="c26ec-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c26ec-110">Value</span></span>|<span data-ttu-id="c26ec-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c26ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c26ec-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="c26ec-112">deviceDefault</span></span>|<span data-ttu-id="c26ec-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c26ec-113">0</span></span>|<span data-ttu-id="c26ec-114">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="c26ec-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="c26ec-115">чистить</span><span class="sxs-lookup"><span data-stu-id="c26ec-115">clean</span></span>|<span data-ttu-id="c26ec-116">1 </span><span class="sxs-lookup"><span data-stu-id="c26ec-116">1</span></span>|<span data-ttu-id="c26ec-117">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="c26ec-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="c26ec-118">папку</span><span class="sxs-lookup"><span data-stu-id="c26ec-118">quarantine</span></span>|<span data-ttu-id="c26ec-119">2 </span><span class="sxs-lookup"><span data-stu-id="c26ec-119">2</span></span>|<span data-ttu-id="c26ec-120">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="c26ec-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="c26ec-121">удалить</span><span class="sxs-lookup"><span data-stu-id="c26ec-121">remove</span></span>|<span data-ttu-id="c26ec-122">3 </span><span class="sxs-lookup"><span data-stu-id="c26ec-122">3</span></span>|<span data-ttu-id="c26ec-123">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="c26ec-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="c26ec-124">разрешить</span><span class="sxs-lookup"><span data-stu-id="c26ec-124">allow</span></span>|<span data-ttu-id="c26ec-125">4 </span><span class="sxs-lookup"><span data-stu-id="c26ec-125">4</span></span>|<span data-ttu-id="c26ec-126">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="c26ec-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="c26ec-127">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="c26ec-127">userDefined</span></span>|<span data-ttu-id="c26ec-128">5 </span><span class="sxs-lookup"><span data-stu-id="c26ec-128">5</span></span>|<span data-ttu-id="c26ec-129">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="c26ec-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="c26ec-130">блок</span><span class="sxs-lookup"><span data-stu-id="c26ec-130">block</span></span>|<span data-ttu-id="c26ec-131">6 </span><span class="sxs-lookup"><span data-stu-id="c26ec-131">6</span></span>|<span data-ttu-id="c26ec-132">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="c26ec-132">Block the detected threat.</span></span>|



