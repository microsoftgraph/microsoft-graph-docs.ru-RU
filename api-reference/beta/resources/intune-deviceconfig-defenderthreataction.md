---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bd72afa1d49e39486454304ce27517e9433a137a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420803"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="693e5-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="693e5-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="693e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="693e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="693e5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="693e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="693e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="693e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="693e5-107">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="693e5-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="693e5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="693e5-108">Members</span></span>
|<span data-ttu-id="693e5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="693e5-109">Member</span></span>|<span data-ttu-id="693e5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="693e5-110">Value</span></span>|<span data-ttu-id="693e5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="693e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="693e5-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="693e5-112">deviceDefault</span></span>|<span data-ttu-id="693e5-113">нуль</span><span class="sxs-lookup"><span data-stu-id="693e5-113">0</span></span>|<span data-ttu-id="693e5-114">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="693e5-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="693e5-115">чистить</span><span class="sxs-lookup"><span data-stu-id="693e5-115">clean</span></span>|<span data-ttu-id="693e5-116">1,1</span><span class="sxs-lookup"><span data-stu-id="693e5-116">1</span></span>|<span data-ttu-id="693e5-117">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="693e5-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="693e5-118">папку</span><span class="sxs-lookup"><span data-stu-id="693e5-118">quarantine</span></span>|<span data-ttu-id="693e5-119">2</span><span class="sxs-lookup"><span data-stu-id="693e5-119">2</span></span>|<span data-ttu-id="693e5-120">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="693e5-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="693e5-121">удалить</span><span class="sxs-lookup"><span data-stu-id="693e5-121">remove</span></span>|<span data-ttu-id="693e5-122">4</span><span class="sxs-lookup"><span data-stu-id="693e5-122">3</span></span>|<span data-ttu-id="693e5-123">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="693e5-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="693e5-124">разрешить</span><span class="sxs-lookup"><span data-stu-id="693e5-124">allow</span></span>|<span data-ttu-id="693e5-125">4 </span><span class="sxs-lookup"><span data-stu-id="693e5-125">4</span></span>|<span data-ttu-id="693e5-126">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="693e5-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="693e5-127">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="693e5-127">userDefined</span></span>|<span data-ttu-id="693e5-128">5 </span><span class="sxs-lookup"><span data-stu-id="693e5-128">5</span></span>|<span data-ttu-id="693e5-129">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="693e5-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="693e5-130">блок</span><span class="sxs-lookup"><span data-stu-id="693e5-130">block</span></span>|<span data-ttu-id="693e5-131">6 </span><span class="sxs-lookup"><span data-stu-id="693e5-131">6</span></span>|<span data-ttu-id="693e5-132">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="693e5-132">Block the detected threat.</span></span>|



