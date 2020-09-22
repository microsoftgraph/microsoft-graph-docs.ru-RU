---
title: тип перечисления Виндовсупдатетипе
description: Какие устройства филиала будут получать обновления от
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 71a1c43cdcb0668f903871cc1bd1a680beee80e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039610"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="81bd9-103">тип перечисления Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="81bd9-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="81bd9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81bd9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81bd9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81bd9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81bd9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81bd9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81bd9-107">Какие устройства филиала будут получать обновления от</span><span class="sxs-lookup"><span data-stu-id="81bd9-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="81bd9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="81bd9-108">Members</span></span>
|<span data-ttu-id="81bd9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="81bd9-109">Member</span></span>|<span data-ttu-id="81bd9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="81bd9-110">Value</span></span>|<span data-ttu-id="81bd9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="81bd9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81bd9-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="81bd9-112">userDefined</span></span>|<span data-ttu-id="81bd9-113">нуль</span><span class="sxs-lookup"><span data-stu-id="81bd9-113">0</span></span>|<span data-ttu-id="81bd9-114">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="81bd9-114">Allow the user to set.</span></span>|
|<span data-ttu-id="81bd9-115">ко</span><span class="sxs-lookup"><span data-stu-id="81bd9-115">all</span></span>|<span data-ttu-id="81bd9-116">1 </span><span class="sxs-lookup"><span data-stu-id="81bd9-116">1</span></span>|<span data-ttu-id="81bd9-117">Половина ежегодного канала (нацеленная).</span><span class="sxs-lookup"><span data-stu-id="81bd9-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="81bd9-118">Device получает все подходящее обновление компонентов из Полугодого канала (нацелено).</span><span class="sxs-lookup"><span data-stu-id="81bd9-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="81bd9-119">бусинессреадйонли</span><span class="sxs-lookup"><span data-stu-id="81bd9-119">businessReadyOnly</span></span>|<span data-ttu-id="81bd9-120">2 </span><span class="sxs-lookup"><span data-stu-id="81bd9-120">2</span></span>|<span data-ttu-id="81bd9-121">Половина ежегодного канала.</span><span class="sxs-lookup"><span data-stu-id="81bd9-121">Semi-annual Channel.</span></span> <span data-ttu-id="81bd9-122">Устройство получает обновления компонентов из Полугодого канала.</span><span class="sxs-lookup"><span data-stu-id="81bd9-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="81bd9-123">виндовсинсидербуилдфаст</span><span class="sxs-lookup"><span data-stu-id="81bd9-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="81bd9-124">4</span><span class="sxs-lookup"><span data-stu-id="81bd9-124">3</span></span>|<span data-ttu-id="81bd9-125">Предварительная сборка Windows для предварительной сборки — Быстрая</span><span class="sxs-lookup"><span data-stu-id="81bd9-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="81bd9-126">виндовсинсидербуилдслов</span><span class="sxs-lookup"><span data-stu-id="81bd9-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="81bd9-127">4 </span><span class="sxs-lookup"><span data-stu-id="81bd9-127">4</span></span>|<span data-ttu-id="81bd9-128">Сборка для предварительной оценки Windows — низкая</span><span class="sxs-lookup"><span data-stu-id="81bd9-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="81bd9-129">виндовсинсидербуилдрелеасе</span><span class="sxs-lookup"><span data-stu-id="81bd9-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="81bd9-130">5 </span><span class="sxs-lookup"><span data-stu-id="81bd9-130">5</span></span>|<span data-ttu-id="81bd9-131">Выпуск сборки предварительной оценки Windows</span><span class="sxs-lookup"><span data-stu-id="81bd9-131">Release Windows Insider build</span></span>|






