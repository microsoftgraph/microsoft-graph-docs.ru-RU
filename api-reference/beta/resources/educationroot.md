---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 91f0162402b8c87042fab622710d314f27d6f4e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507156"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="24b35-103">Тип ресурса educationRoot</span><span class="sxs-lookup"><span data-stu-id="24b35-103">educationRoot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24b35-104">Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования.</span><span class="sxs-lookup"><span data-stu-id="24b35-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="24b35-105">Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)).</span><span class="sxs-lookup"><span data-stu-id="24b35-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="24b35-106">Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.</span><span class="sxs-lookup"><span data-stu-id="24b35-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="24b35-107">Методы</span><span class="sxs-lookup"><span data-stu-id="24b35-107">Methods</span></span>

| <span data-ttu-id="24b35-108">Метод</span><span class="sxs-lookup"><span data-stu-id="24b35-108">Method</span></span>           | <span data-ttu-id="24b35-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="24b35-109">Return Type</span></span>    |<span data-ttu-id="24b35-110">Описание</span><span class="sxs-lookup"><span data-stu-id="24b35-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="24b35-111">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="24b35-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="24b35-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="24b35-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="24b35-113">Создание объекта **educationClass** путем публикации в коллекции курсов.</span><span class="sxs-lookup"><span data-stu-id="24b35-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="24b35-114">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="24b35-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="24b35-115">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="24b35-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="24b35-116">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="24b35-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="24b35-117">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="24b35-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="24b35-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="24b35-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="24b35-119">Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="24b35-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="24b35-120">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="24b35-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="24b35-121">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="24b35-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="24b35-122">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="24b35-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="24b35-123">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="24b35-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="24b35-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="24b35-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="24b35-125">Создание **educationUser** путем публикации в коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="24b35-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="24b35-126">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="24b35-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="24b35-127">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="24b35-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="24b35-128">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="24b35-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="24b35-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="24b35-129">Properties</span></span>
<span data-ttu-id="24b35-130">Нет</span><span class="sxs-lookup"><span data-stu-id="24b35-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="24b35-131">Связи</span><span class="sxs-lookup"><span data-stu-id="24b35-131">Relationships</span></span>
| <span data-ttu-id="24b35-132">Отношение</span><span class="sxs-lookup"><span data-stu-id="24b35-132">Relationship</span></span> | <span data-ttu-id="24b35-133">Тип</span><span class="sxs-lookup"><span data-stu-id="24b35-133">Type</span></span>   |<span data-ttu-id="24b35-134">Описание</span><span class="sxs-lookup"><span data-stu-id="24b35-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24b35-135">classes</span><span class="sxs-lookup"><span data-stu-id="24b35-135">classes</span></span>|<span data-ttu-id="24b35-136">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="24b35-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="24b35-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="24b35-137">Read-only.</span></span> <span data-ttu-id="24b35-138">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="24b35-138">Nullable.</span></span>|
|<span data-ttu-id="24b35-139">me</span><span class="sxs-lookup"><span data-stu-id="24b35-139">me</span></span>|[<span data-ttu-id="24b35-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="24b35-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="24b35-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="24b35-141">Read-only.</span></span> <span data-ttu-id="24b35-142">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="24b35-142">Nullable.</span></span>|
|<span data-ttu-id="24b35-143">schools</span><span class="sxs-lookup"><span data-stu-id="24b35-143">schools</span></span>|<span data-ttu-id="24b35-144">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="24b35-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="24b35-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="24b35-145">Read-only.</span></span> <span data-ttu-id="24b35-146">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="24b35-146">Nullable.</span></span>|
|<span data-ttu-id="24b35-147">users</span><span class="sxs-lookup"><span data-stu-id="24b35-147">users</span></span>|<span data-ttu-id="24b35-148">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="24b35-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="24b35-p105">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="24b35-p105">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationroot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
