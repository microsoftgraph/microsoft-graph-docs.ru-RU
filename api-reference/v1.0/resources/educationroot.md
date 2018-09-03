# <a name="educationroot-resource-type"></a><span data-ttu-id="6a452-101">Тип ресурса educationRoot</span><span class="sxs-lookup"><span data-stu-id="6a452-101">educationRoot resource type</span></span>

<span data-ttu-id="6a452-102">Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования.</span><span class="sxs-lookup"><span data-stu-id="6a452-102">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="6a452-103">Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)).</span><span class="sxs-lookup"><span data-stu-id="6a452-103">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="6a452-104">Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.</span><span class="sxs-lookup"><span data-stu-id="6a452-104">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="6a452-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6a452-105">Methods</span></span>

| <span data-ttu-id="6a452-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6a452-106">Method</span></span>           | <span data-ttu-id="6a452-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6a452-107">Return Type</span></span>    |<span data-ttu-id="6a452-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6a452-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a452-109">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="6a452-109">Create educationClass</span></span>](../api/educationroot_post_classes.md) |[<span data-ttu-id="6a452-110">educationClass</span><span class="sxs-lookup"><span data-stu-id="6a452-110">educationClass</span></span>](educationclass.md)| <span data-ttu-id="6a452-111">Создание объекта **educationClass** путем публикации в коллекции курсов.</span><span class="sxs-lookup"><span data-stu-id="6a452-111">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="6a452-112">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="6a452-112">List classes</span></span>](../api/educationroot_list_classes.md) |<span data-ttu-id="6a452-113">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="6a452-113">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="6a452-114">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="6a452-114">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="6a452-115">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="6a452-115">Create educationSchool</span></span>](../api/educationroot_post_schools.md) |[<span data-ttu-id="6a452-116">educationSchool</span><span class="sxs-lookup"><span data-stu-id="6a452-116">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="6a452-117">Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="6a452-117">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="6a452-118">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="6a452-118">List schools</span></span>](../api/educationroot_list_schools.md) |<span data-ttu-id="6a452-119">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="6a452-119">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="6a452-120">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="6a452-120">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="6a452-121">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="6a452-121">Create educationUser</span></span>](../api/educationroot_post_users.md) |[<span data-ttu-id="6a452-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="6a452-122">educationUser</span></span>](educationuser.md)| <span data-ttu-id="6a452-123">Создание **educationUser** путем публикации в коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="6a452-123">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="6a452-124">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="6a452-124">List users</span></span>](../api/educationroot_list_users.md) |<span data-ttu-id="6a452-125">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="6a452-125">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="6a452-126">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="6a452-126">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a452-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a452-127">Properties</span></span>
<span data-ttu-id="6a452-128">Нет</span><span class="sxs-lookup"><span data-stu-id="6a452-128">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="6a452-129">Связи</span><span class="sxs-lookup"><span data-stu-id="6a452-129">Relationships</span></span>
| <span data-ttu-id="6a452-130">Связь</span><span class="sxs-lookup"><span data-stu-id="6a452-130">Relationship</span></span> | <span data-ttu-id="6a452-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6a452-131">Type</span></span>   |<span data-ttu-id="6a452-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6a452-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a452-133">classes</span><span class="sxs-lookup"><span data-stu-id="6a452-133">classes</span></span>|<span data-ttu-id="6a452-134">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="6a452-134">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="6a452-p102">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="6a452-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="6a452-137">me</span><span class="sxs-lookup"><span data-stu-id="6a452-137">me</span></span>|[<span data-ttu-id="6a452-138">educationUser</span><span class="sxs-lookup"><span data-stu-id="6a452-138">educationUser</span></span>](educationuser.md)| <span data-ttu-id="6a452-p103">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="6a452-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="6a452-141">schools</span><span class="sxs-lookup"><span data-stu-id="6a452-141">schools</span></span>|<span data-ttu-id="6a452-142">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="6a452-142">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="6a452-p104">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="6a452-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="6a452-145">users</span><span class="sxs-lookup"><span data-stu-id="6a452-145">users</span></span>|<span data-ttu-id="6a452-146">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="6a452-146">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="6a452-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6a452-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a452-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a452-149">JSON representation</span></span>
<span data-ttu-id="6a452-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a452-150">Here is a JSON representation of the resource.</span></span>

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