---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
ms.openlocfilehash: 3a49c3b7605cada8cd3f6018fd2ce78280b180f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027843"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="8270b-103">Тип ресурса educationRoot</span><span class="sxs-lookup"><span data-stu-id="8270b-103">educationRoot resource type</span></span>

<span data-ttu-id="8270b-104">Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования.</span><span class="sxs-lookup"><span data-stu-id="8270b-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="8270b-105">Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)).</span><span class="sxs-lookup"><span data-stu-id="8270b-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="8270b-106">Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.</span><span class="sxs-lookup"><span data-stu-id="8270b-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="8270b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8270b-107">Methods</span></span>

| <span data-ttu-id="8270b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8270b-108">Method</span></span>           | <span data-ttu-id="8270b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8270b-109">Return Type</span></span>    |<span data-ttu-id="8270b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8270b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8270b-111">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="8270b-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="8270b-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="8270b-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="8270b-113">Создание объекта **educationClass** путем публикации в коллекции курсов.</span><span class="sxs-lookup"><span data-stu-id="8270b-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="8270b-114">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="8270b-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="8270b-115">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="8270b-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="8270b-116">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="8270b-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="8270b-117">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="8270b-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="8270b-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="8270b-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="8270b-119">Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="8270b-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="8270b-120">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="8270b-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="8270b-121">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="8270b-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="8270b-122">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="8270b-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="8270b-123">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="8270b-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="8270b-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="8270b-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="8270b-125">Создание **educationUser** путем публикации в коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="8270b-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="8270b-126">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="8270b-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="8270b-127">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="8270b-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="8270b-128">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="8270b-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="8270b-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="8270b-129">Properties</span></span>
<span data-ttu-id="8270b-130">Нет</span><span class="sxs-lookup"><span data-stu-id="8270b-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="8270b-131">Связи</span><span class="sxs-lookup"><span data-stu-id="8270b-131">Relationships</span></span>
| <span data-ttu-id="8270b-132">Связь</span><span class="sxs-lookup"><span data-stu-id="8270b-132">Relationship</span></span> | <span data-ttu-id="8270b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8270b-133">Type</span></span>   |<span data-ttu-id="8270b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8270b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8270b-135">classes</span><span class="sxs-lookup"><span data-stu-id="8270b-135">classes</span></span>|<span data-ttu-id="8270b-136">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="8270b-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="8270b-p102">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="8270b-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="8270b-139">me</span><span class="sxs-lookup"><span data-stu-id="8270b-139">me</span></span>|[<span data-ttu-id="8270b-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="8270b-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="8270b-p103">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="8270b-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="8270b-143">schools</span><span class="sxs-lookup"><span data-stu-id="8270b-143">schools</span></span>|<span data-ttu-id="8270b-144">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="8270b-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="8270b-p104">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="8270b-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="8270b-147">users</span><span class="sxs-lookup"><span data-stu-id="8270b-147">users</span></span>|<span data-ttu-id="8270b-148">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="8270b-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="8270b-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="8270b-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8270b-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8270b-151">JSON representation</span></span>
<span data-ttu-id="8270b-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8270b-152">Here is a JSON representation of the resource.</span></span>

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