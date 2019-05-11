---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1376927bc76903e10619e7c71fa53ce26d17075
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947297"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="8796a-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="8796a-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="8796a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8796a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8796a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8796a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8796a-106">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="8796a-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="8796a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8796a-107">Members</span></span>
|<span data-ttu-id="8796a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8796a-108">Member</span></span>|<span data-ttu-id="8796a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8796a-109">Value</span></span>|<span data-ttu-id="8796a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8796a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8796a-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="8796a-111">deviceDefault</span></span>|<span data-ttu-id="8796a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="8796a-112">0</span></span>|<span data-ttu-id="8796a-113">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="8796a-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="8796a-114">чистить</span><span class="sxs-lookup"><span data-stu-id="8796a-114">clean</span></span>|<span data-ttu-id="8796a-115">1,1</span><span class="sxs-lookup"><span data-stu-id="8796a-115">1</span></span>|<span data-ttu-id="8796a-116">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="8796a-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="8796a-117">папку</span><span class="sxs-lookup"><span data-stu-id="8796a-117">quarantine</span></span>|<span data-ttu-id="8796a-118">2</span><span class="sxs-lookup"><span data-stu-id="8796a-118">2</span></span>|<span data-ttu-id="8796a-119">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="8796a-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="8796a-120">удалить</span><span class="sxs-lookup"><span data-stu-id="8796a-120">remove</span></span>|<span data-ttu-id="8796a-121">4</span><span class="sxs-lookup"><span data-stu-id="8796a-121">3</span></span>|<span data-ttu-id="8796a-122">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="8796a-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="8796a-123">разрешить</span><span class="sxs-lookup"><span data-stu-id="8796a-123">allow</span></span>|<span data-ttu-id="8796a-124">SP4</span><span class="sxs-lookup"><span data-stu-id="8796a-124">4</span></span>|<span data-ttu-id="8796a-125">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="8796a-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="8796a-126">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="8796a-126">userDefined</span></span>|<span data-ttu-id="8796a-127">17:00</span><span class="sxs-lookup"><span data-stu-id="8796a-127">5</span></span>|<span data-ttu-id="8796a-128">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="8796a-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="8796a-129">блок</span><span class="sxs-lookup"><span data-stu-id="8796a-129">block</span></span>|<span data-ttu-id="8796a-130">6 </span><span class="sxs-lookup"><span data-stu-id="8796a-130">6</span></span>|<span data-ttu-id="8796a-131">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="8796a-131">Block the detected threat.</span></span>|




