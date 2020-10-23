---
title: тип перечисления Макосконтенткачингпарентселектионполици
description: Определяет, как кэширование содержимого выбирает родительский кэш.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 726c6d4feb7387fd67583c451a9f3399a316f4a0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735822"
---
# <a name="macoscontentcachingparentselectionpolicy-enum-type"></a><span data-ttu-id="ec286-103">тип перечисления Макосконтенткачингпарентселектионполици</span><span class="sxs-lookup"><span data-stu-id="ec286-103">macOSContentCachingParentSelectionPolicy enum type</span></span>

<span data-ttu-id="ec286-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec286-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec286-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec286-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec286-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec286-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec286-107">Определяет, как кэширование содержимого выбирает родительский кэш.</span><span class="sxs-lookup"><span data-stu-id="ec286-107">Determines how content caches select a parent cache.</span></span>

## <a name="members"></a><span data-ttu-id="ec286-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ec286-108">Members</span></span>
|<span data-ttu-id="ec286-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ec286-109">Member</span></span>|<span data-ttu-id="ec286-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ec286-110">Value</span></span>|<span data-ttu-id="ec286-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ec286-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec286-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ec286-112">notConfigured</span></span>|<span data-ttu-id="ec286-113">нуль</span><span class="sxs-lookup"><span data-stu-id="ec286-113">0</span></span>|<span data-ttu-id="ec286-114">По умолчанию используется стратегия циклического перебора.</span><span class="sxs-lookup"><span data-stu-id="ec286-114">Defaults to round-robin strategy.</span></span>|
|<span data-ttu-id="ec286-115">roundRobin</span><span class="sxs-lookup"><span data-stu-id="ec286-115">roundRobin</span></span>|<span data-ttu-id="ec286-116">1,1</span><span class="sxs-lookup"><span data-stu-id="ec286-116">1</span></span>|<span data-ttu-id="ec286-117">Поворачивайте родительские элементы по порядку.</span><span class="sxs-lookup"><span data-stu-id="ec286-117">Rotate through the parents in order.</span></span> <span data-ttu-id="ec286-118">Используйте эту политику для балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="ec286-118">Use this policy for load balancing.</span></span>|
|<span data-ttu-id="ec286-119">фирставаилабле</span><span class="sxs-lookup"><span data-stu-id="ec286-119">firstAvailable</span></span>|<span data-ttu-id="ec286-120">2</span><span class="sxs-lookup"><span data-stu-id="ec286-120">2</span></span>|<span data-ttu-id="ec286-121">Всегда используйте первый доступный родительский элемент в списке родителей.</span><span class="sxs-lookup"><span data-stu-id="ec286-121">Always use the first available parent in the Parents list.</span></span> <span data-ttu-id="ec286-122">Эта политика используется для назначения постоянных основных, вторичных и последующих родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ec286-122">Use this policy to designate permanent primary, secondary, and subsequent parents.</span></span>|
|<span data-ttu-id="ec286-123">урлпасхаш</span><span class="sxs-lookup"><span data-stu-id="ec286-123">urlPathHash</span></span>|<span data-ttu-id="ec286-124">4</span><span class="sxs-lookup"><span data-stu-id="ec286-124">3</span></span>|<span data-ttu-id="ec286-125">Хэширует часть пути в запрашиваемом URL-адресе, чтобы для одного URL-адреса всегда использовался один и тот же родительский элемент.</span><span class="sxs-lookup"><span data-stu-id="ec286-125">Hash the path part of the requested URL so that the same parent is always used for the same URL.</span></span> <span data-ttu-id="ec286-126">Это полезно для максимизации размера Объединенных кэшей родителей.</span><span class="sxs-lookup"><span data-stu-id="ec286-126">This is useful for maximizing the size of the combined caches of the parents.</span></span>|
|<span data-ttu-id="ec286-127">произвольную</span><span class="sxs-lookup"><span data-stu-id="ec286-127">random</span></span>|<span data-ttu-id="ec286-128">4 </span><span class="sxs-lookup"><span data-stu-id="ec286-128">4</span></span>|<span data-ttu-id="ec286-129">Выберите родительский элемент случайным образом.</span><span class="sxs-lookup"><span data-stu-id="ec286-129">Choose a parent at random.</span></span> <span data-ttu-id="ec286-130">Используйте эту политику для балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="ec286-130">Use this policy for load balancing.</span></span>|
|<span data-ttu-id="ec286-131">стиккяваилабле</span><span class="sxs-lookup"><span data-stu-id="ec286-131">stickyAvailable</span></span>|<span data-ttu-id="ec286-132">5 </span><span class="sxs-lookup"><span data-stu-id="ec286-132">5</span></span>|<span data-ttu-id="ec286-133">Используйте первый доступный родительский элемент, который доступен в списке родителей, пока он не станет недоступен, а затем перейдите к следующему.</span><span class="sxs-lookup"><span data-stu-id="ec286-133">Use the first available parent that is available in the Parents list until it becomes unavailable, then advance to the next one.</span></span> <span data-ttu-id="ec286-134">Эта политика используется для назначения плавающего основного, дополнительного и последующего родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ec286-134">Use this policy for designating floating primary, secondary, and subsequent parents.</span></span>|





