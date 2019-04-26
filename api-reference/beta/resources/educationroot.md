---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 83879a2fe448e97f62dc592b42d1cbc1d3d5cf39
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334194"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="5e754-103">Тип ресурса educationRoot</span><span class="sxs-lookup"><span data-stu-id="5e754-103">educationRoot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e754-104">Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования.</span><span class="sxs-lookup"><span data-stu-id="5e754-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="5e754-105">Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)).</span><span class="sxs-lookup"><span data-stu-id="5e754-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="5e754-106">Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.</span><span class="sxs-lookup"><span data-stu-id="5e754-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="5e754-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5e754-107">Methods</span></span>

| <span data-ttu-id="5e754-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5e754-108">Method</span></span>           | <span data-ttu-id="5e754-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5e754-109">Return Type</span></span>    |<span data-ttu-id="5e754-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5e754-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e754-111">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="5e754-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="5e754-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="5e754-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="5e754-113">Создание объекта **educationClass** путем публикации в коллекции курсов.</span><span class="sxs-lookup"><span data-stu-id="5e754-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="5e754-114">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="5e754-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="5e754-115">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="5e754-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="5e754-116">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="5e754-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="5e754-117">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="5e754-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="5e754-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="5e754-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="5e754-119">Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="5e754-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="5e754-120">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="5e754-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="5e754-121">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="5e754-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="5e754-122">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="5e754-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="5e754-123">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="5e754-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="5e754-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="5e754-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="5e754-125">Создание **educationUser** путем публикации в коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="5e754-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="5e754-126">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="5e754-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="5e754-127">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="5e754-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="5e754-128">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="5e754-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e754-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e754-129">Properties</span></span>
<span data-ttu-id="5e754-130">Нет</span><span class="sxs-lookup"><span data-stu-id="5e754-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="5e754-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="5e754-131">Relationships</span></span>
| <span data-ttu-id="5e754-132">Отношение</span><span class="sxs-lookup"><span data-stu-id="5e754-132">Relationship</span></span> | <span data-ttu-id="5e754-133">Тип</span><span class="sxs-lookup"><span data-stu-id="5e754-133">Type</span></span>   |<span data-ttu-id="5e754-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5e754-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e754-135">classes</span><span class="sxs-lookup"><span data-stu-id="5e754-135">classes</span></span>|<span data-ttu-id="5e754-136">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="5e754-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="5e754-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e754-137">Read-only.</span></span> <span data-ttu-id="5e754-138">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="5e754-138">Nullable.</span></span>|
|<span data-ttu-id="5e754-139">me</span><span class="sxs-lookup"><span data-stu-id="5e754-139">me</span></span>|[<span data-ttu-id="5e754-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="5e754-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="5e754-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e754-141">Read-only.</span></span> <span data-ttu-id="5e754-142">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="5e754-142">Nullable.</span></span>|
|<span data-ttu-id="5e754-143">schools</span><span class="sxs-lookup"><span data-stu-id="5e754-143">schools</span></span>|<span data-ttu-id="5e754-144">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="5e754-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="5e754-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e754-145">Read-only.</span></span> <span data-ttu-id="5e754-146">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="5e754-146">Nullable.</span></span>|
|<span data-ttu-id="5e754-147">users</span><span class="sxs-lookup"><span data-stu-id="5e754-147">users</span></span>|<span data-ttu-id="5e754-148">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="5e754-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="5e754-p105">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="5e754-p105">Read-only. Nullable.</span></span>|

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
