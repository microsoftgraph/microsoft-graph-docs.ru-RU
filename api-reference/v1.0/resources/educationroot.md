---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 84b7312515174c19837a5cda3fa3ffb466f65c23
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458756"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="b0b00-103">Тип ресурса educationRoot</span><span class="sxs-lookup"><span data-stu-id="b0b00-103">educationRoot resource type</span></span>

<span data-ttu-id="b0b00-104">Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования.</span><span class="sxs-lookup"><span data-stu-id="b0b00-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="b0b00-105">Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)).</span><span class="sxs-lookup"><span data-stu-id="b0b00-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="b0b00-106">Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.</span><span class="sxs-lookup"><span data-stu-id="b0b00-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="b0b00-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b0b00-107">Methods</span></span>

| <span data-ttu-id="b0b00-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b0b00-108">Method</span></span>           | <span data-ttu-id="b0b00-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b0b00-109">Return Type</span></span>    |<span data-ttu-id="b0b00-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b0b00-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0b00-111">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="b0b00-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="b0b00-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="b0b00-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="b0b00-113">Создание объекта **educationClass** путем публикации в коллекции курсов.</span><span class="sxs-lookup"><span data-stu-id="b0b00-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="b0b00-114">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="b0b00-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="b0b00-115">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="b0b00-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="b0b00-116">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="b0b00-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="b0b00-117">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="b0b00-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="b0b00-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="b0b00-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="b0b00-119">Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="b0b00-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="b0b00-120">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="b0b00-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="b0b00-121">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="b0b00-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="b0b00-122">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="b0b00-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="b0b00-123">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="b0b00-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="b0b00-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="b0b00-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="b0b00-125">Создание **educationUser** путем публикации в коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="b0b00-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="b0b00-126">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="b0b00-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="b0b00-127">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="b0b00-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="b0b00-128">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="b0b00-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0b00-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0b00-129">Properties</span></span>
<span data-ttu-id="b0b00-130">Нет</span><span class="sxs-lookup"><span data-stu-id="b0b00-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="b0b00-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="b0b00-131">Relationships</span></span>
| <span data-ttu-id="b0b00-132">Отношение</span><span class="sxs-lookup"><span data-stu-id="b0b00-132">Relationship</span></span> | <span data-ttu-id="b0b00-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b0b00-133">Type</span></span>   |<span data-ttu-id="b0b00-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b0b00-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0b00-135">classes</span><span class="sxs-lookup"><span data-stu-id="b0b00-135">classes</span></span>|<span data-ttu-id="b0b00-136">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="b0b00-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="b0b00-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b0b00-137">Read-only.</span></span> <span data-ttu-id="b0b00-138">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b0b00-138">Nullable.</span></span>|
|<span data-ttu-id="b0b00-139">me</span><span class="sxs-lookup"><span data-stu-id="b0b00-139">me</span></span>|[<span data-ttu-id="b0b00-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="b0b00-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="b0b00-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b0b00-141">Read-only.</span></span> <span data-ttu-id="b0b00-142">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b0b00-142">Nullable.</span></span>|
|<span data-ttu-id="b0b00-143">schools</span><span class="sxs-lookup"><span data-stu-id="b0b00-143">schools</span></span>|<span data-ttu-id="b0b00-144">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="b0b00-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="b0b00-p104">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="b0b00-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="b0b00-147">users</span><span class="sxs-lookup"><span data-stu-id="b0b00-147">users</span></span>|<span data-ttu-id="b0b00-148">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="b0b00-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="b0b00-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b0b00-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0b00-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0b00-151">JSON representation</span></span>
<span data-ttu-id="b0b00-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0b00-152">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationRoot"
}-->

```json
{
}
```


# <a name="httptabhttp"></a>[<span data-ttu-id="b0b00-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0b00-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0b00-154">C#</span><span class="sxs-lookup"><span data-stu-id="b0b00-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-education-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0b00-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0b00-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-education-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0b00-156">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b0b00-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-education-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
