---
title: тип перечисления Макосконтенткачингпарентселектионполици
description: Определяет, как кэширование содержимого выбирает родительский кэш.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 221d33640a3e100adbad4fe013e10b6c5ab90b4e
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790203"
---
# <a name="macoscontentcachingparentselectionpolicy-enum-type"></a><span data-ttu-id="6db00-103">тип перечисления Макосконтенткачингпарентселектионполици</span><span class="sxs-lookup"><span data-stu-id="6db00-103">macOSContentCachingParentSelectionPolicy enum type</span></span>

<span data-ttu-id="6db00-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6db00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6db00-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6db00-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6db00-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6db00-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6db00-107">Определяет, как кэширование содержимого выбирает родительский кэш.</span><span class="sxs-lookup"><span data-stu-id="6db00-107">Determines how content caches select a parent cache.</span></span>

## <a name="members"></a><span data-ttu-id="6db00-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="6db00-108">Members</span></span>
|<span data-ttu-id="6db00-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="6db00-109">Member</span></span>|<span data-ttu-id="6db00-110">Значение</span><span class="sxs-lookup"><span data-stu-id="6db00-110">Value</span></span>|<span data-ttu-id="6db00-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6db00-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6db00-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6db00-112">notConfigured</span></span>|<span data-ttu-id="6db00-113">нуль</span><span class="sxs-lookup"><span data-stu-id="6db00-113">0</span></span>|<span data-ttu-id="6db00-114">По умолчанию используется стратегия циклического перебора.</span><span class="sxs-lookup"><span data-stu-id="6db00-114">Defaults to round-robin strategy.</span></span>|
|<span data-ttu-id="6db00-115">roundRobin</span><span class="sxs-lookup"><span data-stu-id="6db00-115">roundRobin</span></span>|<span data-ttu-id="6db00-116">1 </span><span class="sxs-lookup"><span data-stu-id="6db00-116">1</span></span>|<span data-ttu-id="6db00-117">Поворачивайте родительские элементы по порядку.</span><span class="sxs-lookup"><span data-stu-id="6db00-117">Rotate through the parents in order.</span></span> <span data-ttu-id="6db00-118">Используйте эту политику для балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="6db00-118">Use this policy for load balancing.</span></span>|
|<span data-ttu-id="6db00-119">фирставаилабле</span><span class="sxs-lookup"><span data-stu-id="6db00-119">firstAvailable</span></span>|<span data-ttu-id="6db00-120">2</span><span class="sxs-lookup"><span data-stu-id="6db00-120">2</span></span>|<span data-ttu-id="6db00-121">Всегда используйте первый доступный родительский элемент в списке родителей.</span><span class="sxs-lookup"><span data-stu-id="6db00-121">Always use the first available parent in the Parents list.</span></span> <span data-ttu-id="6db00-122">Эта политика используется для назначения постоянных основных, вторичных и последующих родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6db00-122">Use this policy to designate permanent primary, secondary, and subsequent parents.</span></span>|
|<span data-ttu-id="6db00-123">урлпасхаш</span><span class="sxs-lookup"><span data-stu-id="6db00-123">urlPathHash</span></span>|<span data-ttu-id="6db00-124">4</span><span class="sxs-lookup"><span data-stu-id="6db00-124">3</span></span>|<span data-ttu-id="6db00-125">Хэширует часть пути в запрашиваемом URL-адресе, чтобы для одного URL-адреса всегда использовался один и тот же родительский элемент.</span><span class="sxs-lookup"><span data-stu-id="6db00-125">Hash the path part of the requested URL so that the same parent is always used for the same URL.</span></span> <span data-ttu-id="6db00-126">Это полезно для максимизации размера Объединенных кэшей родителей.</span><span class="sxs-lookup"><span data-stu-id="6db00-126">This is useful for maximizing the size of the combined caches of the parents.</span></span>|
|<span data-ttu-id="6db00-127">произвольную</span><span class="sxs-lookup"><span data-stu-id="6db00-127">random</span></span>|<span data-ttu-id="6db00-128">4 </span><span class="sxs-lookup"><span data-stu-id="6db00-128">4</span></span>|<span data-ttu-id="6db00-129">Выберите родительский элемент случайным образом.</span><span class="sxs-lookup"><span data-stu-id="6db00-129">Choose a parent at random.</span></span> <span data-ttu-id="6db00-130">Используйте эту политику для балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="6db00-130">Use this policy for load balancing.</span></span>|
|<span data-ttu-id="6db00-131">стиккяваилабле</span><span class="sxs-lookup"><span data-stu-id="6db00-131">stickyAvailable</span></span>|<span data-ttu-id="6db00-132">5 </span><span class="sxs-lookup"><span data-stu-id="6db00-132">5</span></span>|<span data-ttu-id="6db00-133">Используйте первый доступный родительский элемент, который доступен в списке родителей, пока он не станет недоступен, а затем перейдите к следующему.</span><span class="sxs-lookup"><span data-stu-id="6db00-133">Use the first available parent that is available in the Parents list until it becomes unavailable, then advance to the next one.</span></span> <span data-ttu-id="6db00-134">Эта политика используется для назначения плавающего основного, дополнительного и последующего родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6db00-134">Use this policy for designating floating primary, secondary, and subsequent parents.</span></span>|



