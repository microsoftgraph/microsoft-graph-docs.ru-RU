---
title: тип ресурса conditionalAccess
description: Ресурс **conditionalaccess** является точкой входа для объектной модели Conditinal Access. Он не содержит никаких полезных свойств.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3683965cda79f003cb5e548101272d869be902b8
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547529"
---
# <a name="conditionalaccess-resource-type"></a><span data-ttu-id="b7b98-104">тип ресурса conditionalaccess</span><span class="sxs-lookup"><span data-stu-id="b7b98-104">conditionalaccess resource type</span></span>

<span data-ttu-id="b7b98-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7b98-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7b98-106">Ресурс **conditionalAccess —** это точка входа для объектной модели условного доступа.</span><span class="sxs-lookup"><span data-stu-id="b7b98-106">The **conditionalAccess** resource is the entry point for the Conditional Access object model.</span></span> <span data-ttu-id="b7b98-107">Он не содержит никаких полезных свойств.</span><span class="sxs-lookup"><span data-stu-id="b7b98-107">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="b7b98-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b7b98-108">Methods</span></span>

| <span data-ttu-id="b7b98-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b7b98-109">Method</span></span>           | <span data-ttu-id="b7b98-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b7b98-110">Return Type</span></span>    |<span data-ttu-id="b7b98-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b7b98-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b7b98-112">Создание conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="b7b98-112">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) |[<span data-ttu-id="b7b98-113">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="b7b98-113">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md)| <span data-ttu-id="b7b98-114">Создайте **новое условноеaccessPolicy,** разместив в коллекции conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="b7b98-114">Create a new **conditionalAccessPolicy** by posting to the conditionalAccessPolicy collection.</span></span>|
|[<span data-ttu-id="b7b98-115">Создание namedLocations</span><span class="sxs-lookup"><span data-stu-id="b7b98-115">Create namedLocations</span></span>](../api/conditionalaccessroot-post-namedlocations.md) |[<span data-ttu-id="b7b98-116">namedLocation</span><span class="sxs-lookup"><span data-stu-id="b7b98-116">namedLocation</span></span>](namedlocation.md)| <span data-ttu-id="b7b98-117">Создайте новые **именаLocations,** разместив их в коллекции namedLocations.</span><span class="sxs-lookup"><span data-stu-id="b7b98-117">Create a new **namedLocations** by posting to the namedLocations collection.</span></span>|
|[<span data-ttu-id="b7b98-118">Создание проверки подлинностиContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="b7b98-118">Create authenticationContextClassReferences</span></span>](../api/conditionalaccessroot-post-authenticationcontextclassreferences.md)|[<span data-ttu-id="b7b98-119">authenticationContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="b7b98-119">authenticationContextClassReferences</span></span>](authenticationcontextclassreference.md)|<span data-ttu-id="b7b98-120">Создайте новую **проверку подлинностиContextClassReferences,** разместив их в коллекции authenticationContextClassReferences.</span><span class="sxs-lookup"><span data-stu-id="b7b98-120">Create a new **authenticationContextClassReferences** by posting to authenticationContextClassReferences collection.</span></span>|


## <a name="properties"></a><span data-ttu-id="b7b98-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7b98-121">Properties</span></span>

<span data-ttu-id="b7b98-122">Ресурс conditionalAccess является точкой входа для объектной модели условного доступа и не содержит никаких свойств.</span><span class="sxs-lookup"><span data-stu-id="b7b98-122">The conditionalAccess resource is the entry point for the Conditional Access object model and doesn't contain any properties.</span></span>

## <a name="relationships"></a><span data-ttu-id="b7b98-123">Связи</span><span class="sxs-lookup"><span data-stu-id="b7b98-123">Relationships</span></span>
| <span data-ttu-id="b7b98-124">Связь</span><span class="sxs-lookup"><span data-stu-id="b7b98-124">Relationship</span></span> | <span data-ttu-id="b7b98-125">Тип</span><span class="sxs-lookup"><span data-stu-id="b7b98-125">Type</span></span>   |<span data-ttu-id="b7b98-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b7b98-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7b98-127">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="b7b98-127">conditionalAccessPolicy</span></span>|<span data-ttu-id="b7b98-128">Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b7b98-128">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span>| <span data-ttu-id="b7b98-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b7b98-129">Read-only.</span></span> <span data-ttu-id="b7b98-130">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b7b98-130">Nullable.</span></span> <span data-ttu-id="b7b98-131">Возвращает коллекцию указанных политик условного доступа.</span><span class="sxs-lookup"><span data-stu-id="b7b98-131">Returns a collection of the specified Conditional Access policies.</span></span>|
|<span data-ttu-id="b7b98-132">namedLocations</span><span class="sxs-lookup"><span data-stu-id="b7b98-132">namedLocations</span></span>|<span data-ttu-id="b7b98-133">[коллекция namedLocations](namedlocation.md)</span><span class="sxs-lookup"><span data-stu-id="b7b98-133">[namedLocations](namedlocation.md) collection</span></span>| <span data-ttu-id="b7b98-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b7b98-134">Read-only.</span></span> <span data-ttu-id="b7b98-135">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b7b98-135">Nullable.</span></span> <span data-ttu-id="b7b98-136">Возвращает коллекцию указанных именных местоположений.</span><span class="sxs-lookup"><span data-stu-id="b7b98-136">Returns a collection of the specified named locations.</span></span>|
|<span data-ttu-id="b7b98-137">authenticationContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="b7b98-137">authenticationContextClassReferences</span></span>|<span data-ttu-id="b7b98-138">[коллекция authenticationContextClassReferences](authenticationcontextclassreference.md)</span><span class="sxs-lookup"><span data-stu-id="b7b98-138">[authenticationContextClassReferences](authenticationcontextclassreference.md) collection</span></span>|<span data-ttu-id="b7b98-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b7b98-139">Read-only.</span></span> <span data-ttu-id="b7b98-140">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b7b98-140">Nullable.</span></span> <span data-ttu-id="b7b98-141">Возвращает коллекцию ссылок на определенный класс проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b7b98-141">Returns a collection of the specified authentication context class references.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conditional access resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

