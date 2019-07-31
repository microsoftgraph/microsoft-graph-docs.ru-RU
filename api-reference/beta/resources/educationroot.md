---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8084b1aae61ffb9e9982fbf8b5f4b8e430a85da1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972567"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="41854-103">Тип ресурса educationRoot</span><span class="sxs-lookup"><span data-stu-id="41854-103">educationRoot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41854-104">Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования.</span><span class="sxs-lookup"><span data-stu-id="41854-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="41854-105">Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)).</span><span class="sxs-lookup"><span data-stu-id="41854-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="41854-106">Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.</span><span class="sxs-lookup"><span data-stu-id="41854-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="41854-107">Методы</span><span class="sxs-lookup"><span data-stu-id="41854-107">Methods</span></span>

| <span data-ttu-id="41854-108">Метод</span><span class="sxs-lookup"><span data-stu-id="41854-108">Method</span></span>           | <span data-ttu-id="41854-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="41854-109">Return Type</span></span>    |<span data-ttu-id="41854-110">Описание</span><span class="sxs-lookup"><span data-stu-id="41854-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41854-111">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="41854-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="41854-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="41854-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="41854-113">Создание объекта **educationClass** путем публикации в коллекции курсов.</span><span class="sxs-lookup"><span data-stu-id="41854-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="41854-114">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="41854-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="41854-115">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="41854-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="41854-116">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="41854-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="41854-117">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="41854-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="41854-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="41854-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="41854-119">Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="41854-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="41854-120">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="41854-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="41854-121">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="41854-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="41854-122">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="41854-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="41854-123">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="41854-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="41854-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="41854-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="41854-125">Создание **educationUser** путем публикации в коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="41854-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="41854-126">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="41854-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="41854-127">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="41854-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="41854-128">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="41854-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="41854-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="41854-129">Properties</span></span>
<span data-ttu-id="41854-130">Нет</span><span class="sxs-lookup"><span data-stu-id="41854-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="41854-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="41854-131">Relationships</span></span>
| <span data-ttu-id="41854-132">Отношение</span><span class="sxs-lookup"><span data-stu-id="41854-132">Relationship</span></span> | <span data-ttu-id="41854-133">Тип</span><span class="sxs-lookup"><span data-stu-id="41854-133">Type</span></span>   |<span data-ttu-id="41854-134">Описание</span><span class="sxs-lookup"><span data-stu-id="41854-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41854-135">classes</span><span class="sxs-lookup"><span data-stu-id="41854-135">classes</span></span>|<span data-ttu-id="41854-136">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="41854-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="41854-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41854-137">Read-only.</span></span> <span data-ttu-id="41854-138">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="41854-138">Nullable.</span></span>|
|<span data-ttu-id="41854-139">me</span><span class="sxs-lookup"><span data-stu-id="41854-139">me</span></span>|[<span data-ttu-id="41854-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="41854-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="41854-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41854-141">Read-only.</span></span> <span data-ttu-id="41854-142">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="41854-142">Nullable.</span></span>|
|<span data-ttu-id="41854-143">schools</span><span class="sxs-lookup"><span data-stu-id="41854-143">schools</span></span>|<span data-ttu-id="41854-144">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="41854-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="41854-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41854-145">Read-only.</span></span> <span data-ttu-id="41854-146">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="41854-146">Nullable.</span></span>|
|<span data-ttu-id="41854-147">users</span><span class="sxs-lookup"><span data-stu-id="41854-147">users</span></span>|<span data-ttu-id="41854-148">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="41854-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="41854-p105">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="41854-p105">Read-only. Nullable.</span></span>|

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
