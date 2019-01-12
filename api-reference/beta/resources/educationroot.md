---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e610ca79dcef29d85a9190c9d3d9429cbf3b363d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949656"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="a16fd-103">Тип ресурса educationRoot</span><span class="sxs-lookup"><span data-stu-id="a16fd-103">educationRoot resource type</span></span>

> <span data-ttu-id="a16fd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a16fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a16fd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a16fd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a16fd-106">Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования.</span><span class="sxs-lookup"><span data-stu-id="a16fd-106">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="a16fd-107">Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)).</span><span class="sxs-lookup"><span data-stu-id="a16fd-107">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="a16fd-108">Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.</span><span class="sxs-lookup"><span data-stu-id="a16fd-108">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="a16fd-109">Методы</span><span class="sxs-lookup"><span data-stu-id="a16fd-109">Methods</span></span>

| <span data-ttu-id="a16fd-110">Метод</span><span class="sxs-lookup"><span data-stu-id="a16fd-110">Method</span></span>           | <span data-ttu-id="a16fd-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a16fd-111">Return Type</span></span>    |<span data-ttu-id="a16fd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a16fd-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a16fd-113">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="a16fd-113">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="a16fd-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="a16fd-114">educationClass</span></span>](educationclass.md)| <span data-ttu-id="a16fd-115">Создание объекта **educationClass** путем публикации в коллекции курсов.</span><span class="sxs-lookup"><span data-stu-id="a16fd-115">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="a16fd-116">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="a16fd-116">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="a16fd-117">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="a16fd-117">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="a16fd-118">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="a16fd-118">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="a16fd-119">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="a16fd-119">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="a16fd-120">educationSchool</span><span class="sxs-lookup"><span data-stu-id="a16fd-120">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="a16fd-121">Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="a16fd-121">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="a16fd-122">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="a16fd-122">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="a16fd-123">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="a16fd-123">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="a16fd-124">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="a16fd-124">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="a16fd-125">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="a16fd-125">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="a16fd-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="a16fd-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="a16fd-127">Создание **educationUser** путем публикации в коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="a16fd-127">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="a16fd-128">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="a16fd-128">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="a16fd-129">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="a16fd-129">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="a16fd-130">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="a16fd-130">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="a16fd-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="a16fd-131">Properties</span></span>
<span data-ttu-id="a16fd-132">Нет</span><span class="sxs-lookup"><span data-stu-id="a16fd-132">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="a16fd-133">Связи</span><span class="sxs-lookup"><span data-stu-id="a16fd-133">Relationships</span></span>
| <span data-ttu-id="a16fd-134">Связь</span><span class="sxs-lookup"><span data-stu-id="a16fd-134">Relationship</span></span> | <span data-ttu-id="a16fd-135">Тип</span><span class="sxs-lookup"><span data-stu-id="a16fd-135">Type</span></span>   |<span data-ttu-id="a16fd-136">Описание</span><span class="sxs-lookup"><span data-stu-id="a16fd-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a16fd-137">classes</span><span class="sxs-lookup"><span data-stu-id="a16fd-137">classes</span></span>|<span data-ttu-id="a16fd-138">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="a16fd-138">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="a16fd-p103">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="a16fd-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="a16fd-141">me</span><span class="sxs-lookup"><span data-stu-id="a16fd-141">me</span></span>|[<span data-ttu-id="a16fd-142">educationUser</span><span class="sxs-lookup"><span data-stu-id="a16fd-142">educationUser</span></span>](educationuser.md)| <span data-ttu-id="a16fd-p104">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="a16fd-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="a16fd-145">schools</span><span class="sxs-lookup"><span data-stu-id="a16fd-145">schools</span></span>|<span data-ttu-id="a16fd-146">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="a16fd-146">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="a16fd-p105">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="a16fd-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="a16fd-149">users</span><span class="sxs-lookup"><span data-stu-id="a16fd-149">users</span></span>|<span data-ttu-id="a16fd-150">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="a16fd-150">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="a16fd-p106">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="a16fd-p106">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
