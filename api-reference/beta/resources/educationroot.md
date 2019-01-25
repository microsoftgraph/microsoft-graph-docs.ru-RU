---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 91f0162402b8c87042fab622710d314f27d6f4e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523514"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="38a9c-103">Тип ресурса educationRoot</span><span class="sxs-lookup"><span data-stu-id="38a9c-103">educationRoot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38a9c-104">Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования.</span><span class="sxs-lookup"><span data-stu-id="38a9c-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="38a9c-105">Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)).</span><span class="sxs-lookup"><span data-stu-id="38a9c-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="38a9c-106">Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.</span><span class="sxs-lookup"><span data-stu-id="38a9c-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="38a9c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="38a9c-107">Methods</span></span>

| <span data-ttu-id="38a9c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="38a9c-108">Method</span></span>           | <span data-ttu-id="38a9c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="38a9c-109">Return Type</span></span>    |<span data-ttu-id="38a9c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="38a9c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38a9c-111">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="38a9c-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="38a9c-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="38a9c-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="38a9c-113">Создание объекта **educationClass** путем публикации в коллекции курсов.</span><span class="sxs-lookup"><span data-stu-id="38a9c-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="38a9c-114">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="38a9c-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="38a9c-115">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="38a9c-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="38a9c-116">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="38a9c-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="38a9c-117">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="38a9c-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="38a9c-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="38a9c-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="38a9c-119">Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="38a9c-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="38a9c-120">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="38a9c-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="38a9c-121">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="38a9c-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="38a9c-122">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="38a9c-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="38a9c-123">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="38a9c-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="38a9c-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="38a9c-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="38a9c-125">Создание **educationUser** путем публикации в коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="38a9c-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="38a9c-126">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="38a9c-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="38a9c-127">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="38a9c-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="38a9c-128">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="38a9c-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="38a9c-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="38a9c-129">Properties</span></span>
<span data-ttu-id="38a9c-130">Нет</span><span class="sxs-lookup"><span data-stu-id="38a9c-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="38a9c-131">Связи</span><span class="sxs-lookup"><span data-stu-id="38a9c-131">Relationships</span></span>
| <span data-ttu-id="38a9c-132">Связь</span><span class="sxs-lookup"><span data-stu-id="38a9c-132">Relationship</span></span> | <span data-ttu-id="38a9c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="38a9c-133">Type</span></span>   |<span data-ttu-id="38a9c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="38a9c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38a9c-135">classes</span><span class="sxs-lookup"><span data-stu-id="38a9c-135">classes</span></span>|<span data-ttu-id="38a9c-136">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="38a9c-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="38a9c-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="38a9c-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="38a9c-139">me</span><span class="sxs-lookup"><span data-stu-id="38a9c-139">me</span></span>|[<span data-ttu-id="38a9c-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="38a9c-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="38a9c-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="38a9c-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="38a9c-143">schools</span><span class="sxs-lookup"><span data-stu-id="38a9c-143">schools</span></span>|<span data-ttu-id="38a9c-144">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="38a9c-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="38a9c-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="38a9c-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="38a9c-147">users</span><span class="sxs-lookup"><span data-stu-id="38a9c-147">users</span></span>|<span data-ttu-id="38a9c-148">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="38a9c-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="38a9c-p105">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="38a9c-p105">Read-only. Nullable.</span></span>|

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
