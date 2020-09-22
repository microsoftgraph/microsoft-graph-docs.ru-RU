---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5f93b35dc48087b8d40db0cc3eabc2ba3ba10c8b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032686"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="12084-103">Тип ресурса educationRoot</span><span class="sxs-lookup"><span data-stu-id="12084-103">educationRoot resource type</span></span>

<span data-ttu-id="12084-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12084-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12084-105">Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования.</span><span class="sxs-lookup"><span data-stu-id="12084-105">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="12084-106">Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)).</span><span class="sxs-lookup"><span data-stu-id="12084-106">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="12084-107">Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.</span><span class="sxs-lookup"><span data-stu-id="12084-107">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="12084-108">Методы</span><span class="sxs-lookup"><span data-stu-id="12084-108">Methods</span></span>

| <span data-ttu-id="12084-109">Метод</span><span class="sxs-lookup"><span data-stu-id="12084-109">Method</span></span>           | <span data-ttu-id="12084-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="12084-110">Return Type</span></span>    |<span data-ttu-id="12084-111">Описание</span><span class="sxs-lookup"><span data-stu-id="12084-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12084-112">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="12084-112">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="12084-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="12084-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="12084-114">Создание объекта **educationClass** путем публикации в коллекции курсов.</span><span class="sxs-lookup"><span data-stu-id="12084-114">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="12084-115">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="12084-115">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="12084-116">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="12084-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="12084-117">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="12084-117">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="12084-118">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="12084-118">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="12084-119">educationSchool</span><span class="sxs-lookup"><span data-stu-id="12084-119">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="12084-120">Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="12084-120">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="12084-121">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="12084-121">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="12084-122">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="12084-122">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="12084-123">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="12084-123">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="12084-124">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="12084-124">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="12084-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="12084-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="12084-126">Создание **educationUser** путем публикации в коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="12084-126">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="12084-127">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="12084-127">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="12084-128">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="12084-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="12084-129">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="12084-129">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="12084-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="12084-130">Properties</span></span>
<span data-ttu-id="12084-131">Нет</span><span class="sxs-lookup"><span data-stu-id="12084-131">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="12084-132">Связи</span><span class="sxs-lookup"><span data-stu-id="12084-132">Relationships</span></span>
| <span data-ttu-id="12084-133">Связь</span><span class="sxs-lookup"><span data-stu-id="12084-133">Relationship</span></span> | <span data-ttu-id="12084-134">Тип</span><span class="sxs-lookup"><span data-stu-id="12084-134">Type</span></span>   |<span data-ttu-id="12084-135">Описание</span><span class="sxs-lookup"><span data-stu-id="12084-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12084-136">classes</span><span class="sxs-lookup"><span data-stu-id="12084-136">classes</span></span>|<span data-ttu-id="12084-137">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="12084-137">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="12084-p102">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="12084-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="12084-140">me</span><span class="sxs-lookup"><span data-stu-id="12084-140">me</span></span>|[<span data-ttu-id="12084-141">educationUser</span><span class="sxs-lookup"><span data-stu-id="12084-141">educationUser</span></span>](educationuser.md)| <span data-ttu-id="12084-p103">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="12084-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="12084-144">schools</span><span class="sxs-lookup"><span data-stu-id="12084-144">schools</span></span>|<span data-ttu-id="12084-145">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="12084-145">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="12084-p104">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="12084-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="12084-148">users</span><span class="sxs-lookup"><span data-stu-id="12084-148">users</span></span>|<span data-ttu-id="12084-149">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="12084-149">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="12084-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="12084-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12084-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12084-152">JSON representation</span></span>
<span data-ttu-id="12084-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12084-153">Here is a JSON representation of the resource.</span></span>

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


# <a name="http"></a>[<span data-ttu-id="12084-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="12084-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education
```
# <a name="c"></a>[<span data-ttu-id="12084-155">C#</span><span class="sxs-lookup"><span data-stu-id="12084-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-education-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12084-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12084-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-education-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12084-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12084-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-education-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12084-158">Java</span><span class="sxs-lookup"><span data-stu-id="12084-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-education-java-snippets.md)]
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

