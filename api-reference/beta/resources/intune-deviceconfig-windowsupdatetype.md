---
title: тип перечисления Виндовсупдатетипе
description: Какие устройства филиала будут получать обновления от
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 77dc988570ebd089d273fd767987068313e03866
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441088"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="f74ef-103">тип перечисления Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="f74ef-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="f74ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f74ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f74ef-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f74ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f74ef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f74ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f74ef-107">Какие устройства филиала будут получать обновления от</span><span class="sxs-lookup"><span data-stu-id="f74ef-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="f74ef-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f74ef-108">Members</span></span>
|<span data-ttu-id="f74ef-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f74ef-109">Member</span></span>|<span data-ttu-id="f74ef-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f74ef-110">Value</span></span>|<span data-ttu-id="f74ef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f74ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f74ef-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="f74ef-112">userDefined</span></span>|<span data-ttu-id="f74ef-113">нуль</span><span class="sxs-lookup"><span data-stu-id="f74ef-113">0</span></span>|<span data-ttu-id="f74ef-114">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="f74ef-114">Allow the user to set.</span></span>|
|<span data-ttu-id="f74ef-115">ко</span><span class="sxs-lookup"><span data-stu-id="f74ef-115">all</span></span>|<span data-ttu-id="f74ef-116">1,1</span><span class="sxs-lookup"><span data-stu-id="f74ef-116">1</span></span>|<span data-ttu-id="f74ef-117">Половина ежегодного канала (нацеленная).</span><span class="sxs-lookup"><span data-stu-id="f74ef-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="f74ef-118">Device получает все подходящее обновление компонентов из Полугодого канала (нацелено).</span><span class="sxs-lookup"><span data-stu-id="f74ef-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="f74ef-119">бусинессреадйонли</span><span class="sxs-lookup"><span data-stu-id="f74ef-119">businessReadyOnly</span></span>|<span data-ttu-id="f74ef-120">2</span><span class="sxs-lookup"><span data-stu-id="f74ef-120">2</span></span>|<span data-ttu-id="f74ef-121">Половина ежегодного канала.</span><span class="sxs-lookup"><span data-stu-id="f74ef-121">Semi-annual Channel.</span></span> <span data-ttu-id="f74ef-122">Устройство получает обновления компонентов из Полугодого канала.</span><span class="sxs-lookup"><span data-stu-id="f74ef-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="f74ef-123">виндовсинсидербуилдфаст</span><span class="sxs-lookup"><span data-stu-id="f74ef-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="f74ef-124">4</span><span class="sxs-lookup"><span data-stu-id="f74ef-124">3</span></span>|<span data-ttu-id="f74ef-125">Предварительная сборка Windows для предварительной сборки — Быстрая</span><span class="sxs-lookup"><span data-stu-id="f74ef-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="f74ef-126">виндовсинсидербуилдслов</span><span class="sxs-lookup"><span data-stu-id="f74ef-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="f74ef-127">4 </span><span class="sxs-lookup"><span data-stu-id="f74ef-127">4</span></span>|<span data-ttu-id="f74ef-128">Сборка для предварительной оценки Windows — низкая</span><span class="sxs-lookup"><span data-stu-id="f74ef-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="f74ef-129">виндовсинсидербуилдрелеасе</span><span class="sxs-lookup"><span data-stu-id="f74ef-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="f74ef-130">5 </span><span class="sxs-lookup"><span data-stu-id="f74ef-130">5</span></span>|<span data-ttu-id="f74ef-131">Выпуск сборки предварительной оценки Windows</span><span class="sxs-lookup"><span data-stu-id="f74ef-131">Release Windows Insider build</span></span>|



