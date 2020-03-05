---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 14e152fa5aa24366eade56b632d96e2c4e4bfcc8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501061"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="98fee-103">Тип ресурса educationRoot</span><span class="sxs-lookup"><span data-stu-id="98fee-103">educationRoot resource type</span></span>

<span data-ttu-id="98fee-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="98fee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98fee-105">Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования.</span><span class="sxs-lookup"><span data-stu-id="98fee-105">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="98fee-106">Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)).</span><span class="sxs-lookup"><span data-stu-id="98fee-106">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="98fee-107">Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.</span><span class="sxs-lookup"><span data-stu-id="98fee-107">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="98fee-108">Методы</span><span class="sxs-lookup"><span data-stu-id="98fee-108">Methods</span></span>

| <span data-ttu-id="98fee-109">Метод</span><span class="sxs-lookup"><span data-stu-id="98fee-109">Method</span></span>           | <span data-ttu-id="98fee-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="98fee-110">Return Type</span></span>    |<span data-ttu-id="98fee-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98fee-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98fee-112">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="98fee-112">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="98fee-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="98fee-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="98fee-114">Создание объекта **educationClass** путем публикации в коллекции курсов.</span><span class="sxs-lookup"><span data-stu-id="98fee-114">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="98fee-115">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="98fee-115">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="98fee-116">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="98fee-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="98fee-117">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="98fee-117">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="98fee-118">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="98fee-118">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="98fee-119">educationSchool</span><span class="sxs-lookup"><span data-stu-id="98fee-119">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="98fee-120">Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="98fee-120">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="98fee-121">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="98fee-121">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="98fee-122">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="98fee-122">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="98fee-123">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="98fee-123">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="98fee-124">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="98fee-124">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="98fee-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="98fee-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="98fee-126">Создание **educationUser** путем публикации в коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="98fee-126">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="98fee-127">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="98fee-127">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="98fee-128">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="98fee-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="98fee-129">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="98fee-129">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="98fee-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="98fee-130">Properties</span></span>
<span data-ttu-id="98fee-131">Нет</span><span class="sxs-lookup"><span data-stu-id="98fee-131">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="98fee-132">Связи</span><span class="sxs-lookup"><span data-stu-id="98fee-132">Relationships</span></span>
| <span data-ttu-id="98fee-133">Связь</span><span class="sxs-lookup"><span data-stu-id="98fee-133">Relationship</span></span> | <span data-ttu-id="98fee-134">Тип</span><span class="sxs-lookup"><span data-stu-id="98fee-134">Type</span></span>   |<span data-ttu-id="98fee-135">Описание</span><span class="sxs-lookup"><span data-stu-id="98fee-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98fee-136">classes</span><span class="sxs-lookup"><span data-stu-id="98fee-136">classes</span></span>|<span data-ttu-id="98fee-137">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="98fee-137">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="98fee-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98fee-138">Read-only.</span></span> <span data-ttu-id="98fee-139">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="98fee-139">Nullable.</span></span>|
|<span data-ttu-id="98fee-140">me</span><span class="sxs-lookup"><span data-stu-id="98fee-140">me</span></span>|[<span data-ttu-id="98fee-141">educationUser</span><span class="sxs-lookup"><span data-stu-id="98fee-141">educationUser</span></span>](educationuser.md)| <span data-ttu-id="98fee-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98fee-142">Read-only.</span></span> <span data-ttu-id="98fee-143">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="98fee-143">Nullable.</span></span>|
|<span data-ttu-id="98fee-144">schools</span><span class="sxs-lookup"><span data-stu-id="98fee-144">schools</span></span>|<span data-ttu-id="98fee-145">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="98fee-145">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="98fee-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98fee-146">Read-only.</span></span> <span data-ttu-id="98fee-147">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="98fee-147">Nullable.</span></span>|
|<span data-ttu-id="98fee-148">users</span><span class="sxs-lookup"><span data-stu-id="98fee-148">users</span></span>|<span data-ttu-id="98fee-149">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="98fee-149">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="98fee-p105">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="98fee-p105">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
