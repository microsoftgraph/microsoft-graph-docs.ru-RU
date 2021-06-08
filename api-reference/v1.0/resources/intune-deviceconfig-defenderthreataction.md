---
title: тип enum defenderThreatAction
description: Действие защитника по умолчанию для решения обнаруженных угроз вредоносных программ.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 636d20b3c71b62157946e77230cd8945dd9957cd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758892"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="b8bc6-103">тип enum defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="b8bc6-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="b8bc6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8bc6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8bc6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8bc6-106">Действие защитника по умолчанию для решения обнаруженных угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="b8bc6-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b8bc6-107">Members</span></span>
|<span data-ttu-id="b8bc6-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b8bc6-108">Member</span></span>|<span data-ttu-id="b8bc6-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b8bc6-109">Value</span></span>|<span data-ttu-id="b8bc6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8bc6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8bc6-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b8bc6-111">deviceDefault</span></span>|<span data-ttu-id="b8bc6-112">0</span><span class="sxs-lookup"><span data-stu-id="b8bc6-112">0</span></span>|<span data-ttu-id="b8bc6-113">Применение действий на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="b8bc6-114">очистка</span><span class="sxs-lookup"><span data-stu-id="b8bc6-114">clean</span></span>|<span data-ttu-id="b8bc6-115">1</span><span class="sxs-lookup"><span data-stu-id="b8bc6-115">1</span></span>|<span data-ttu-id="b8bc6-116">Очистите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="b8bc6-117">карантин</span><span class="sxs-lookup"><span data-stu-id="b8bc6-117">quarantine</span></span>|<span data-ttu-id="b8bc6-118">2</span><span class="sxs-lookup"><span data-stu-id="b8bc6-118">2</span></span>|<span data-ttu-id="b8bc6-119">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="b8bc6-120">удаление</span><span class="sxs-lookup"><span data-stu-id="b8bc6-120">remove</span></span>|<span data-ttu-id="b8bc6-121">3</span><span class="sxs-lookup"><span data-stu-id="b8bc6-121">3</span></span>|<span data-ttu-id="b8bc6-122">Удалите обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="b8bc6-123">разрешить</span><span class="sxs-lookup"><span data-stu-id="b8bc6-123">allow</span></span>|<span data-ttu-id="b8bc6-124">4 </span><span class="sxs-lookup"><span data-stu-id="b8bc6-124">4</span></span>|<span data-ttu-id="b8bc6-125">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="b8bc6-126">userDefined</span><span class="sxs-lookup"><span data-stu-id="b8bc6-126">userDefined</span></span>|<span data-ttu-id="b8bc6-127">5 </span><span class="sxs-lookup"><span data-stu-id="b8bc6-127">5</span></span>|<span data-ttu-id="b8bc6-128">Разрешить пользователю определять действия, которые необходимо принять с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="b8bc6-129">block</span><span class="sxs-lookup"><span data-stu-id="b8bc6-129">block</span></span>|<span data-ttu-id="b8bc6-130">6 </span><span class="sxs-lookup"><span data-stu-id="b8bc6-130">6</span></span>|<span data-ttu-id="b8bc6-131">Заблокировать обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-131">Block the detected threat.</span></span>|




