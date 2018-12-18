---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
ms.openlocfilehash: 2a9eac02552e62e7bfb889e9e87efe47fa5f88f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307436"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="dd70f-103">Тип ресурса educationRoot</span><span class="sxs-lookup"><span data-stu-id="dd70f-103">educationRoot resource type</span></span>

> <span data-ttu-id="dd70f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dd70f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd70f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd70f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd70f-106">Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования.</span><span class="sxs-lookup"><span data-stu-id="dd70f-106">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="dd70f-107">Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)).</span><span class="sxs-lookup"><span data-stu-id="dd70f-107">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="dd70f-108">Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.</span><span class="sxs-lookup"><span data-stu-id="dd70f-108">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="dd70f-109">Методы</span><span class="sxs-lookup"><span data-stu-id="dd70f-109">Methods</span></span>

| <span data-ttu-id="dd70f-110">Метод</span><span class="sxs-lookup"><span data-stu-id="dd70f-110">Method</span></span>           | <span data-ttu-id="dd70f-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dd70f-111">Return Type</span></span>    |<span data-ttu-id="dd70f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dd70f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd70f-113">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="dd70f-113">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="dd70f-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="dd70f-114">educationClass</span></span>](educationclass.md)| <span data-ttu-id="dd70f-115">Создание объекта **educationClass** путем публикации в коллекции курсов.</span><span class="sxs-lookup"><span data-stu-id="dd70f-115">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="dd70f-116">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="dd70f-116">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="dd70f-117">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="dd70f-117">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="dd70f-118">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="dd70f-118">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="dd70f-119">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="dd70f-119">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="dd70f-120">educationSchool</span><span class="sxs-lookup"><span data-stu-id="dd70f-120">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="dd70f-121">Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="dd70f-121">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="dd70f-122">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="dd70f-122">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="dd70f-123">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="dd70f-123">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="dd70f-124">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="dd70f-124">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="dd70f-125">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="dd70f-125">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="dd70f-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="dd70f-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="dd70f-127">Создание **educationUser** путем публикации в коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="dd70f-127">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="dd70f-128">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="dd70f-128">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="dd70f-129">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="dd70f-129">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="dd70f-130">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="dd70f-130">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="dd70f-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd70f-131">Properties</span></span>
<span data-ttu-id="dd70f-132">Нет</span><span class="sxs-lookup"><span data-stu-id="dd70f-132">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="dd70f-133">Связи</span><span class="sxs-lookup"><span data-stu-id="dd70f-133">Relationships</span></span>
| <span data-ttu-id="dd70f-134">Связь</span><span class="sxs-lookup"><span data-stu-id="dd70f-134">Relationship</span></span> | <span data-ttu-id="dd70f-135">Тип</span><span class="sxs-lookup"><span data-stu-id="dd70f-135">Type</span></span>   |<span data-ttu-id="dd70f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="dd70f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd70f-137">classes</span><span class="sxs-lookup"><span data-stu-id="dd70f-137">classes</span></span>|<span data-ttu-id="dd70f-138">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="dd70f-138">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="dd70f-p103">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="dd70f-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="dd70f-141">me</span><span class="sxs-lookup"><span data-stu-id="dd70f-141">me</span></span>|[<span data-ttu-id="dd70f-142">educationUser</span><span class="sxs-lookup"><span data-stu-id="dd70f-142">educationUser</span></span>](educationuser.md)| <span data-ttu-id="dd70f-p104">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="dd70f-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="dd70f-145">schools</span><span class="sxs-lookup"><span data-stu-id="dd70f-145">schools</span></span>|<span data-ttu-id="dd70f-146">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="dd70f-146">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="dd70f-p105">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="dd70f-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="dd70f-149">users</span><span class="sxs-lookup"><span data-stu-id="dd70f-149">users</span></span>|<span data-ttu-id="dd70f-150">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="dd70f-150">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="dd70f-p106">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="dd70f-p106">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->