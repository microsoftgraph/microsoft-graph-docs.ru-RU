---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e16ea7734b61213286d15467701fa3512ebb7d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563821"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="15c84-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="15c84-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="15c84-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15c84-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15c84-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15c84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15c84-106">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="15c84-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="15c84-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="15c84-107">Members</span></span>
|<span data-ttu-id="15c84-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="15c84-108">Member</span></span>|<span data-ttu-id="15c84-109">Значение</span><span class="sxs-lookup"><span data-stu-id="15c84-109">Value</span></span>|<span data-ttu-id="15c84-110">Описание</span><span class="sxs-lookup"><span data-stu-id="15c84-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15c84-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="15c84-111">deviceDefault</span></span>|<span data-ttu-id="15c84-112">нуль</span><span class="sxs-lookup"><span data-stu-id="15c84-112">0</span></span>|<span data-ttu-id="15c84-113">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="15c84-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="15c84-114">чистить</span><span class="sxs-lookup"><span data-stu-id="15c84-114">clean</span></span>|<span data-ttu-id="15c84-115">1 </span><span class="sxs-lookup"><span data-stu-id="15c84-115">1</span></span>|<span data-ttu-id="15c84-116">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="15c84-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="15c84-117">папку</span><span class="sxs-lookup"><span data-stu-id="15c84-117">quarantine</span></span>|<span data-ttu-id="15c84-118">2 </span><span class="sxs-lookup"><span data-stu-id="15c84-118">2</span></span>|<span data-ttu-id="15c84-119">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="15c84-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="15c84-120">удалить</span><span class="sxs-lookup"><span data-stu-id="15c84-120">remove</span></span>|<span data-ttu-id="15c84-121">3 </span><span class="sxs-lookup"><span data-stu-id="15c84-121">3</span></span>|<span data-ttu-id="15c84-122">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="15c84-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="15c84-123">разрешить</span><span class="sxs-lookup"><span data-stu-id="15c84-123">allow</span></span>|<span data-ttu-id="15c84-124">4 </span><span class="sxs-lookup"><span data-stu-id="15c84-124">4</span></span>|<span data-ttu-id="15c84-125">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="15c84-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="15c84-126">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="15c84-126">userDefined</span></span>|<span data-ttu-id="15c84-127">5 </span><span class="sxs-lookup"><span data-stu-id="15c84-127">5</span></span>|<span data-ttu-id="15c84-128">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="15c84-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="15c84-129">блок</span><span class="sxs-lookup"><span data-stu-id="15c84-129">block</span></span>|<span data-ttu-id="15c84-130">6 </span><span class="sxs-lookup"><span data-stu-id="15c84-130">6</span></span>|<span data-ttu-id="15c84-131">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="15c84-131">Block the detected threat.</span></span>|





