---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 57b5ecf73548bf67bcb1fbfb75ed0730cb308424
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333417"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="607af-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="607af-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="607af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="607af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="607af-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="607af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="607af-106">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="607af-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="607af-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="607af-107">Members</span></span>
|<span data-ttu-id="607af-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="607af-108">Member</span></span>|<span data-ttu-id="607af-109">Значение</span><span class="sxs-lookup"><span data-stu-id="607af-109">Value</span></span>|<span data-ttu-id="607af-110">Описание</span><span class="sxs-lookup"><span data-stu-id="607af-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="607af-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="607af-111">deviceDefault</span></span>|<span data-ttu-id="607af-112">нуль</span><span class="sxs-lookup"><span data-stu-id="607af-112">0</span></span>|<span data-ttu-id="607af-113">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="607af-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="607af-114">чистить</span><span class="sxs-lookup"><span data-stu-id="607af-114">clean</span></span>|<span data-ttu-id="607af-115">1,1</span><span class="sxs-lookup"><span data-stu-id="607af-115">1</span></span>|<span data-ttu-id="607af-116">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="607af-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="607af-117">папку</span><span class="sxs-lookup"><span data-stu-id="607af-117">quarantine</span></span>|<span data-ttu-id="607af-118">2</span><span class="sxs-lookup"><span data-stu-id="607af-118">2</span></span>|<span data-ttu-id="607af-119">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="607af-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="607af-120">удалить</span><span class="sxs-lookup"><span data-stu-id="607af-120">remove</span></span>|<span data-ttu-id="607af-121">4</span><span class="sxs-lookup"><span data-stu-id="607af-121">3</span></span>|<span data-ttu-id="607af-122">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="607af-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="607af-123">разрешить</span><span class="sxs-lookup"><span data-stu-id="607af-123">allow</span></span>|<span data-ttu-id="607af-124">SP4</span><span class="sxs-lookup"><span data-stu-id="607af-124">4</span></span>|<span data-ttu-id="607af-125">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="607af-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="607af-126">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="607af-126">userDefined</span></span>|<span data-ttu-id="607af-127">17:00</span><span class="sxs-lookup"><span data-stu-id="607af-127">5</span></span>|<span data-ttu-id="607af-128">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="607af-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="607af-129">блок</span><span class="sxs-lookup"><span data-stu-id="607af-129">block</span></span>|<span data-ttu-id="607af-130">6 </span><span class="sxs-lookup"><span data-stu-id="607af-130">6</span></span>|<span data-ttu-id="607af-131">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="607af-131">Block the detected threat.</span></span>|



