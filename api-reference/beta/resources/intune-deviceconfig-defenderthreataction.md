---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6549b16e325fd8830d0b96de7fd234a315319b8a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794412"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="66cb3-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="66cb3-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="66cb3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66cb3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66cb3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66cb3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66cb3-106">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="66cb3-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="66cb3-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="66cb3-107">Members</span></span>
|<span data-ttu-id="66cb3-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="66cb3-108">Member</span></span>|<span data-ttu-id="66cb3-109">Значение</span><span class="sxs-lookup"><span data-stu-id="66cb3-109">Value</span></span>|<span data-ttu-id="66cb3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="66cb3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66cb3-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="66cb3-111">deviceDefault</span></span>|<span data-ttu-id="66cb3-112">нуль</span><span class="sxs-lookup"><span data-stu-id="66cb3-112">0</span></span>|<span data-ttu-id="66cb3-113">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="66cb3-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="66cb3-114">чистить</span><span class="sxs-lookup"><span data-stu-id="66cb3-114">clean</span></span>|<span data-ttu-id="66cb3-115">1,1</span><span class="sxs-lookup"><span data-stu-id="66cb3-115">1</span></span>|<span data-ttu-id="66cb3-116">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="66cb3-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="66cb3-117">папку</span><span class="sxs-lookup"><span data-stu-id="66cb3-117">quarantine</span></span>|<span data-ttu-id="66cb3-118">2</span><span class="sxs-lookup"><span data-stu-id="66cb3-118">2</span></span>|<span data-ttu-id="66cb3-119">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="66cb3-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="66cb3-120">удалить</span><span class="sxs-lookup"><span data-stu-id="66cb3-120">remove</span></span>|<span data-ttu-id="66cb3-121">4</span><span class="sxs-lookup"><span data-stu-id="66cb3-121">3</span></span>|<span data-ttu-id="66cb3-122">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="66cb3-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="66cb3-123">разрешить</span><span class="sxs-lookup"><span data-stu-id="66cb3-123">allow</span></span>|<span data-ttu-id="66cb3-124">4 </span><span class="sxs-lookup"><span data-stu-id="66cb3-124">4</span></span>|<span data-ttu-id="66cb3-125">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="66cb3-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="66cb3-126">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="66cb3-126">userDefined</span></span>|<span data-ttu-id="66cb3-127">5 </span><span class="sxs-lookup"><span data-stu-id="66cb3-127">5</span></span>|<span data-ttu-id="66cb3-128">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="66cb3-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="66cb3-129">блок</span><span class="sxs-lookup"><span data-stu-id="66cb3-129">block</span></span>|<span data-ttu-id="66cb3-130">6 </span><span class="sxs-lookup"><span data-stu-id="66cb3-130">6</span></span>|<span data-ttu-id="66cb3-131">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="66cb3-131">Block the detected threat.</span></span>|



