---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
ms.openlocfilehash: 11aaaec20ccd688b16b74224d1a8c6937e52c5cd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342471"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="fa51d-103">Тип ресурса educationRoot</span><span class="sxs-lookup"><span data-stu-id="fa51d-103">educationRoot resource type</span></span>

<span data-ttu-id="fa51d-104">Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования.</span><span class="sxs-lookup"><span data-stu-id="fa51d-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="fa51d-105">Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)).</span><span class="sxs-lookup"><span data-stu-id="fa51d-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="fa51d-106">Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.</span><span class="sxs-lookup"><span data-stu-id="fa51d-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="fa51d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="fa51d-107">Methods</span></span>

| <span data-ttu-id="fa51d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="fa51d-108">Method</span></span>           | <span data-ttu-id="fa51d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fa51d-109">Return Type</span></span>    |<span data-ttu-id="fa51d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fa51d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fa51d-111">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="fa51d-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="fa51d-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="fa51d-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="fa51d-113">Создание объекта **educationClass** путем публикации в коллекции курсов.</span><span class="sxs-lookup"><span data-stu-id="fa51d-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="fa51d-114">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="fa51d-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="fa51d-115">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="fa51d-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="fa51d-116">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="fa51d-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="fa51d-117">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="fa51d-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="fa51d-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="fa51d-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="fa51d-119">Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="fa51d-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="fa51d-120">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="fa51d-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="fa51d-121">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="fa51d-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="fa51d-122">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="fa51d-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="fa51d-123">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="fa51d-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="fa51d-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="fa51d-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="fa51d-125">Создание **educationUser** путем публикации в коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="fa51d-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="fa51d-126">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="fa51d-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="fa51d-127">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="fa51d-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="fa51d-128">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="fa51d-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="fa51d-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa51d-129">Properties</span></span>
<span data-ttu-id="fa51d-130">Нет</span><span class="sxs-lookup"><span data-stu-id="fa51d-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="fa51d-131">Связи</span><span class="sxs-lookup"><span data-stu-id="fa51d-131">Relationships</span></span>
| <span data-ttu-id="fa51d-132">Связь</span><span class="sxs-lookup"><span data-stu-id="fa51d-132">Relationship</span></span> | <span data-ttu-id="fa51d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="fa51d-133">Type</span></span>   |<span data-ttu-id="fa51d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="fa51d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa51d-135">classes</span><span class="sxs-lookup"><span data-stu-id="fa51d-135">classes</span></span>|<span data-ttu-id="fa51d-136">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="fa51d-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="fa51d-p102">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="fa51d-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="fa51d-139">me</span><span class="sxs-lookup"><span data-stu-id="fa51d-139">me</span></span>|[<span data-ttu-id="fa51d-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="fa51d-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="fa51d-p103">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="fa51d-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="fa51d-143">schools</span><span class="sxs-lookup"><span data-stu-id="fa51d-143">schools</span></span>|<span data-ttu-id="fa51d-144">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="fa51d-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="fa51d-p104">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="fa51d-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="fa51d-147">users</span><span class="sxs-lookup"><span data-stu-id="fa51d-147">users</span></span>|<span data-ttu-id="fa51d-148">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="fa51d-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="fa51d-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="fa51d-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa51d-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa51d-151">JSON representation</span></span>
<span data-ttu-id="fa51d-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa51d-152">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```

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
  "tocPath": ""
}-->