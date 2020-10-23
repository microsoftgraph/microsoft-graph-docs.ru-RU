---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bd71ee742ba7d7b5a98c5f3bbf90496bb52392be
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696267"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="84660-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="84660-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="84660-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84660-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84660-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84660-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84660-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84660-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84660-107">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="84660-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="84660-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="84660-108">Members</span></span>
|<span data-ttu-id="84660-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="84660-109">Member</span></span>|<span data-ttu-id="84660-110">Значение</span><span class="sxs-lookup"><span data-stu-id="84660-110">Value</span></span>|<span data-ttu-id="84660-111">Описание</span><span class="sxs-lookup"><span data-stu-id="84660-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84660-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="84660-112">deviceDefault</span></span>|<span data-ttu-id="84660-113">нуль</span><span class="sxs-lookup"><span data-stu-id="84660-113">0</span></span>|<span data-ttu-id="84660-114">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="84660-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="84660-115">чистить</span><span class="sxs-lookup"><span data-stu-id="84660-115">clean</span></span>|<span data-ttu-id="84660-116">1,1</span><span class="sxs-lookup"><span data-stu-id="84660-116">1</span></span>|<span data-ttu-id="84660-117">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="84660-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="84660-118">папку</span><span class="sxs-lookup"><span data-stu-id="84660-118">quarantine</span></span>|<span data-ttu-id="84660-119">2</span><span class="sxs-lookup"><span data-stu-id="84660-119">2</span></span>|<span data-ttu-id="84660-120">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="84660-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="84660-121">удалить</span><span class="sxs-lookup"><span data-stu-id="84660-121">remove</span></span>|<span data-ttu-id="84660-122">4</span><span class="sxs-lookup"><span data-stu-id="84660-122">3</span></span>|<span data-ttu-id="84660-123">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="84660-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="84660-124">разрешить</span><span class="sxs-lookup"><span data-stu-id="84660-124">allow</span></span>|<span data-ttu-id="84660-125">4 </span><span class="sxs-lookup"><span data-stu-id="84660-125">4</span></span>|<span data-ttu-id="84660-126">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="84660-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="84660-127">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="84660-127">userDefined</span></span>|<span data-ttu-id="84660-128">5 </span><span class="sxs-lookup"><span data-stu-id="84660-128">5</span></span>|<span data-ttu-id="84660-129">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="84660-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="84660-130">блок</span><span class="sxs-lookup"><span data-stu-id="84660-130">block</span></span>|<span data-ttu-id="84660-131">6 </span><span class="sxs-lookup"><span data-stu-id="84660-131">6</span></span>|<span data-ttu-id="84660-132">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="84660-132">Block the detected threat.</span></span>|





