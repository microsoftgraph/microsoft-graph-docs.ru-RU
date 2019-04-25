---
title: тип перечисления Дефендерсреатактион
description: Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d3d48415e55ad246f75ca9b32bd169ee102fc67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534320"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="070ab-103">тип перечисления Дефендерсреатактион</span><span class="sxs-lookup"><span data-stu-id="070ab-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="070ab-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="070ab-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="070ab-105">Действие защитника по умолчанию для обнаружения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="070ab-105">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="070ab-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="070ab-106">Members</span></span>
|<span data-ttu-id="070ab-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="070ab-107">Member</span></span>|<span data-ttu-id="070ab-108">Значение</span><span class="sxs-lookup"><span data-stu-id="070ab-108">Value</span></span>|<span data-ttu-id="070ab-109">Описание</span><span class="sxs-lookup"><span data-stu-id="070ab-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="070ab-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="070ab-110">deviceDefault</span></span>|<span data-ttu-id="070ab-111">нуль</span><span class="sxs-lookup"><span data-stu-id="070ab-111">0</span></span>|<span data-ttu-id="070ab-112">Применение действия на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="070ab-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="070ab-113">чистить</span><span class="sxs-lookup"><span data-stu-id="070ab-113">clean</span></span>|<span data-ttu-id="070ab-114">1 </span><span class="sxs-lookup"><span data-stu-id="070ab-114">1</span></span>|<span data-ttu-id="070ab-115">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="070ab-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="070ab-116">папку</span><span class="sxs-lookup"><span data-stu-id="070ab-116">quarantine</span></span>|<span data-ttu-id="070ab-117">2 </span><span class="sxs-lookup"><span data-stu-id="070ab-117">2</span></span>|<span data-ttu-id="070ab-118">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="070ab-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="070ab-119">удалить</span><span class="sxs-lookup"><span data-stu-id="070ab-119">remove</span></span>|<span data-ttu-id="070ab-120">3 </span><span class="sxs-lookup"><span data-stu-id="070ab-120">3</span></span>|<span data-ttu-id="070ab-121">Удаление обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="070ab-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="070ab-122">разрешить</span><span class="sxs-lookup"><span data-stu-id="070ab-122">allow</span></span>|<span data-ttu-id="070ab-123">4 </span><span class="sxs-lookup"><span data-stu-id="070ab-123">4</span></span>|<span data-ttu-id="070ab-124">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="070ab-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="070ab-125">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="070ab-125">userDefined</span></span>|<span data-ttu-id="070ab-126">5 </span><span class="sxs-lookup"><span data-stu-id="070ab-126">5</span></span>|<span data-ttu-id="070ab-127">Разрешить пользователю определять действие, выполняемое с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="070ab-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="070ab-128">блок</span><span class="sxs-lookup"><span data-stu-id="070ab-128">block</span></span>|<span data-ttu-id="070ab-129">6 </span><span class="sxs-lookup"><span data-stu-id="070ab-129">6</span></span>|<span data-ttu-id="070ab-130">Блокировка обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="070ab-130">Block the detected threat.</span></span>|



