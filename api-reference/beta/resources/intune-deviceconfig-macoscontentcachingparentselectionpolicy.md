---
title: тип перечисления Макосконтенткачингпарентселектионполици
description: Определяет, как кэширование содержимого выбирает родительский кэш.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 45cc23160ba937481eb6b1af8f404c0a2fd4f3cb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026637"
---
# <a name="macoscontentcachingparentselectionpolicy-enum-type"></a><span data-ttu-id="b0632-103">тип перечисления Макосконтенткачингпарентселектионполици</span><span class="sxs-lookup"><span data-stu-id="b0632-103">macOSContentCachingParentSelectionPolicy enum type</span></span>

<span data-ttu-id="b0632-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0632-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0632-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0632-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0632-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0632-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0632-107">Определяет, как кэширование содержимого выбирает родительский кэш.</span><span class="sxs-lookup"><span data-stu-id="b0632-107">Determines how content caches select a parent cache.</span></span>

## <a name="members"></a><span data-ttu-id="b0632-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b0632-108">Members</span></span>
|<span data-ttu-id="b0632-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b0632-109">Member</span></span>|<span data-ttu-id="b0632-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b0632-110">Value</span></span>|<span data-ttu-id="b0632-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b0632-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0632-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b0632-112">notConfigured</span></span>|<span data-ttu-id="b0632-113">нуль</span><span class="sxs-lookup"><span data-stu-id="b0632-113">0</span></span>|<span data-ttu-id="b0632-114">По умолчанию используется стратегия циклического перебора.</span><span class="sxs-lookup"><span data-stu-id="b0632-114">Defaults to round-robin strategy.</span></span>|
|<span data-ttu-id="b0632-115">roundRobin</span><span class="sxs-lookup"><span data-stu-id="b0632-115">roundRobin</span></span>|<span data-ttu-id="b0632-116">1 </span><span class="sxs-lookup"><span data-stu-id="b0632-116">1</span></span>|<span data-ttu-id="b0632-117">Поворачивайте родительские элементы по порядку.</span><span class="sxs-lookup"><span data-stu-id="b0632-117">Rotate through the parents in order.</span></span> <span data-ttu-id="b0632-118">Используйте эту политику для балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="b0632-118">Use this policy for load balancing.</span></span>|
|<span data-ttu-id="b0632-119">фирставаилабле</span><span class="sxs-lookup"><span data-stu-id="b0632-119">firstAvailable</span></span>|<span data-ttu-id="b0632-120">2 </span><span class="sxs-lookup"><span data-stu-id="b0632-120">2</span></span>|<span data-ttu-id="b0632-121">Всегда используйте первый доступный родительский элемент в списке родителей.</span><span class="sxs-lookup"><span data-stu-id="b0632-121">Always use the first available parent in the Parents list.</span></span> <span data-ttu-id="b0632-122">Эта политика используется для назначения постоянных основных, вторичных и последующих родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b0632-122">Use this policy to designate permanent primary, secondary, and subsequent parents.</span></span>|
|<span data-ttu-id="b0632-123">урлпасхаш</span><span class="sxs-lookup"><span data-stu-id="b0632-123">urlPathHash</span></span>|<span data-ttu-id="b0632-124">4</span><span class="sxs-lookup"><span data-stu-id="b0632-124">3</span></span>|<span data-ttu-id="b0632-125">Хэширует часть пути в запрашиваемом URL-адресе, чтобы для одного URL-адреса всегда использовался один и тот же родительский элемент.</span><span class="sxs-lookup"><span data-stu-id="b0632-125">Hash the path part of the requested URL so that the same parent is always used for the same URL.</span></span> <span data-ttu-id="b0632-126">Это полезно для максимизации размера Объединенных кэшей родителей.</span><span class="sxs-lookup"><span data-stu-id="b0632-126">This is useful for maximizing the size of the combined caches of the parents.</span></span>|
|<span data-ttu-id="b0632-127">произвольную</span><span class="sxs-lookup"><span data-stu-id="b0632-127">random</span></span>|<span data-ttu-id="b0632-128">4 </span><span class="sxs-lookup"><span data-stu-id="b0632-128">4</span></span>|<span data-ttu-id="b0632-129">Выберите родительский элемент случайным образом.</span><span class="sxs-lookup"><span data-stu-id="b0632-129">Choose a parent at random.</span></span> <span data-ttu-id="b0632-130">Используйте эту политику для балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="b0632-130">Use this policy for load balancing.</span></span>|
|<span data-ttu-id="b0632-131">стиккяваилабле</span><span class="sxs-lookup"><span data-stu-id="b0632-131">stickyAvailable</span></span>|<span data-ttu-id="b0632-132">5 </span><span class="sxs-lookup"><span data-stu-id="b0632-132">5</span></span>|<span data-ttu-id="b0632-133">Используйте первый доступный родительский элемент, который доступен в списке родителей, пока он не станет недоступен, а затем перейдите к следующему.</span><span class="sxs-lookup"><span data-stu-id="b0632-133">Use the first available parent that is available in the Parents list until it becomes unavailable, then advance to the next one.</span></span> <span data-ttu-id="b0632-134">Эта политика используется для назначения плавающего основного, дополнительного и последующего родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b0632-134">Use this policy for designating floating primary, secondary, and subsequent parents.</span></span>|






