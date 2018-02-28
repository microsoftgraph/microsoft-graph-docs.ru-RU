# <a name="educationschool-resource-type"></a><span data-ttu-id="850e6-101">Тип ресурса educationSchool</span><span class="sxs-lookup"><span data-stu-id="850e6-101">educationSchool resource type</span></span>

<span data-ttu-id="850e6-102">Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="850e6-102">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  


## <a name="methods"></a><span data-ttu-id="850e6-103">Методы</span><span class="sxs-lookup"><span data-stu-id="850e6-103">Methods</span></span>

| <span data-ttu-id="850e6-104">Метод</span><span class="sxs-lookup"><span data-stu-id="850e6-104">Method</span></span>           | <span data-ttu-id="850e6-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="850e6-105">Return Type</span></span>    |<span data-ttu-id="850e6-106">Описание</span><span class="sxs-lookup"><span data-stu-id="850e6-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="850e6-107">Get</span><span class="sxs-lookup"><span data-stu-id="850e6-107">Get</span></span>](../api/educationschool_get.md) | [<span data-ttu-id="850e6-108">educationSchool</span><span class="sxs-lookup"><span data-stu-id="850e6-108">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="850e6-109">Считывание свойств и отношений объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="850e6-109">Read properties and relationships of the **windowsDefenderAdvancedThreatProtectionConfiguration** object.</span></span>|
|[<span data-ttu-id="850e6-110">Добавление класса</span><span class="sxs-lookup"><span data-stu-id="850e6-110">Add class</span></span>](../api/educationschool_post_classes.md) |[<span data-ttu-id="850e6-111">educationClass</span><span class="sxs-lookup"><span data-stu-id="850e6-111">educationClass</span></span>](educationclass.md)| <span data-ttu-id="850e6-112">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.</span><span class="sxs-lookup"><span data-stu-id="850e6-112">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="850e6-113">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="850e6-113">List classes</span></span>](../api/educationschool_list_classes.md) |<span data-ttu-id="850e6-114">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="850e6-114">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="850e6-115">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="850e6-115">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="850e6-116">Удаление класса</span><span class="sxs-lookup"><span data-stu-id="850e6-116">Remove class</span></span>](../api/educationschool_delete_classes.md) |[<span data-ttu-id="850e6-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="850e6-117">educationClass</span></span>](educationclass.md)| <span data-ttu-id="850e6-118">Удаление **educationClass** из учебного заведения через свойство навигации classes.</span><span class="sxs-lookup"><span data-stu-id="850e6-118">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="850e6-119">Добавление пользователя</span><span class="sxs-lookup"><span data-stu-id="850e6-119">Add user</span></span>](../api/educationschool_post_users.md) |[<span data-ttu-id="850e6-120">educationUser</span><span class="sxs-lookup"><span data-stu-id="850e6-120">educationUser</span></span>](educationuser.md)| <span data-ttu-id="850e6-121">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="850e6-121">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="850e6-122">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="850e6-122">List users</span></span>](../api/educationschool_list_users.md) |<span data-ttu-id="850e6-123">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="850e6-123">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="850e6-124">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="850e6-124">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="850e6-125">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="850e6-125">Remove user</span></span>](../api/educationschool_delete_users.md) |[<span data-ttu-id="850e6-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="850e6-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="850e6-127">Удаление **educationUser** из учебного заведения через свойство навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="850e6-127">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="850e6-128">Обновление</span><span class="sxs-lookup"><span data-stu-id="850e6-128">Update</span></span>](../api/educationschool_update.md) | [<span data-ttu-id="850e6-129">educationSchool</span><span class="sxs-lookup"><span data-stu-id="850e6-129">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="850e6-130">Обновление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="850e6-130">Update an **event** object.</span></span> |
|[<span data-ttu-id="850e6-131">Удаление</span><span class="sxs-lookup"><span data-stu-id="850e6-131">Delete</span></span>](../api/educationschool_delete.md) | <span data-ttu-id="850e6-132">None</span><span class="sxs-lookup"><span data-stu-id="850e6-132">None</span></span> |<span data-ttu-id="850e6-133">Удаление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="850e6-133">Delete an **event** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="850e6-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="850e6-134">Properties</span></span>
| <span data-ttu-id="850e6-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="850e6-135">Property</span></span>     | <span data-ttu-id="850e6-136">Тип</span><span class="sxs-lookup"><span data-stu-id="850e6-136">Type</span></span>   |<span data-ttu-id="850e6-137">Описание</span><span class="sxs-lookup"><span data-stu-id="850e6-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="850e6-138">id</span><span class="sxs-lookup"><span data-stu-id="850e6-138">id</span></span>|<span data-ttu-id="850e6-139">String</span><span class="sxs-lookup"><span data-stu-id="850e6-139">String</span></span>|<span data-ttu-id="850e6-140">GUID этого учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="850e6-140">GUID of this school.</span></span>|
|<span data-ttu-id="850e6-141">displayName</span><span class="sxs-lookup"><span data-stu-id="850e6-141">displayName</span></span>| <span data-ttu-id="850e6-142">String</span><span class="sxs-lookup"><span data-stu-id="850e6-142">String</span></span>| <span data-ttu-id="850e6-143">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="850e6-143">Display name of the partner.</span></span>| 
|<span data-ttu-id="850e6-144">description</span><span class="sxs-lookup"><span data-stu-id="850e6-144">description</span></span>| <span data-ttu-id="850e6-145">String</span><span class="sxs-lookup"><span data-stu-id="850e6-145">String</span></span> | <span data-ttu-id="850e6-146">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="850e6-146">Description of the template.</span></span>| 
|<span data-ttu-id="850e6-147">status</span><span class="sxs-lookup"><span data-stu-id="850e6-147">status</span></span>| <span data-ttu-id="850e6-148">string</span><span class="sxs-lookup"><span data-stu-id="850e6-148">string</span></span>| <span data-ttu-id="850e6-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="850e6-149">Read-only.</span></span> <span data-ttu-id="850e6-150">Возможные значения: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="850e6-150">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="850e6-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="850e6-151">externalSource</span></span>| <span data-ttu-id="850e6-152">string</span><span class="sxs-lookup"><span data-stu-id="850e6-152">string</span></span>| <span data-ttu-id="850e6-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="850e6-153">Read-only.</span></span>  <span data-ttu-id="850e6-154">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="850e6-154">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="850e6-155">principalEmail</span><span class="sxs-lookup"><span data-stu-id="850e6-155">principalEmail</span></span>| <span data-ttu-id="850e6-156">String</span><span class="sxs-lookup"><span data-stu-id="850e6-156">String</span></span>| <span data-ttu-id="850e6-157">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="850e6-157">Email address of the principal.</span></span>|
|<span data-ttu-id="850e6-158">principalName</span><span class="sxs-lookup"><span data-stu-id="850e6-158">principalName</span></span>| <span data-ttu-id="850e6-159">String</span><span class="sxs-lookup"><span data-stu-id="850e6-159">String</span></span> | <span data-ttu-id="850e6-160">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="850e6-160">Name of the principal.</span></span>|
|<span data-ttu-id="850e6-161">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="850e6-161">externalPrincipalId</span></span>| <span data-ttu-id="850e6-162">String</span><span class="sxs-lookup"><span data-stu-id="850e6-162">String</span></span> | <span data-ttu-id="850e6-163">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="850e6-163">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="850e6-164">highestGrade</span><span class="sxs-lookup"><span data-stu-id="850e6-164">highestGrade</span></span>|<span data-ttu-id="850e6-165">String</span><span class="sxs-lookup"><span data-stu-id="850e6-165">String</span></span>| <span data-ttu-id="850e6-166">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="850e6-166">Highest grade taught.</span></span> |
|<span data-ttu-id="850e6-167">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="850e6-167">lowestGrade</span></span>|<span data-ttu-id="850e6-168">String</span><span class="sxs-lookup"><span data-stu-id="850e6-168">String</span></span>| <span data-ttu-id="850e6-169">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="850e6-169">Lowest grade taught.</span></span> |
|<span data-ttu-id="850e6-170">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="850e6-170">schoolNumber</span></span>|<span data-ttu-id="850e6-171">String</span><span class="sxs-lookup"><span data-stu-id="850e6-171">String</span></span>| <span data-ttu-id="850e6-172">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="850e6-172">School Number.</span></span>|
|<span data-ttu-id="850e6-173">externalId</span><span class="sxs-lookup"><span data-stu-id="850e6-173">externalId</span></span>|<span data-ttu-id="850e6-174">String</span><span class="sxs-lookup"><span data-stu-id="850e6-174">String</span></span>| <span data-ttu-id="850e6-175">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="850e6-175">ID of school in syncing system.</span></span> |
|<span data-ttu-id="850e6-176">phone</span><span class="sxs-lookup"><span data-stu-id="850e6-176">Phone</span></span>|<span data-ttu-id="850e6-177">String</span><span class="sxs-lookup"><span data-stu-id="850e6-177">String</span></span>| <span data-ttu-id="850e6-178">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="850e6-178">Phone number of school.</span></span> |
|<span data-ttu-id="850e6-179">fax</span><span class="sxs-lookup"><span data-stu-id="850e6-179">fax</span></span>|<span data-ttu-id="850e6-180">String</span><span class="sxs-lookup"><span data-stu-id="850e6-180">String</span></span>| <span data-ttu-id="850e6-181">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="850e6-181">Fax number of school.</span></span> |
|<span data-ttu-id="850e6-182">address</span><span class="sxs-lookup"><span data-stu-id="850e6-182">address</span></span>|[<span data-ttu-id="850e6-183">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="850e6-183">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="850e6-184">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="850e6-184">Address of the school.</span></span>|
|<span data-ttu-id="850e6-185">createdBy</span><span class="sxs-lookup"><span data-stu-id="850e6-185">createdBy</span></span>|[<span data-ttu-id="850e6-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="850e6-186">identitySet</span></span>](identityset.md)|<span data-ttu-id="850e6-187">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="850e6-187">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="850e6-188">Связи</span><span class="sxs-lookup"><span data-stu-id="850e6-188">Relationships</span></span>
| <span data-ttu-id="850e6-189">Связь</span><span class="sxs-lookup"><span data-stu-id="850e6-189">Relationship</span></span> | <span data-ttu-id="850e6-190">Тип</span><span class="sxs-lookup"><span data-stu-id="850e6-190">Type</span></span>   |<span data-ttu-id="850e6-191">Описание</span><span class="sxs-lookup"><span data-stu-id="850e6-191">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="850e6-192">classes</span><span class="sxs-lookup"><span data-stu-id="850e6-192">Classes</span></span>|<span data-ttu-id="850e6-193">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="850e6-193">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="850e6-194">Классы, которые обучаются в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="850e6-194">Classes taught at the school.</span></span> <span data-ttu-id="850e6-195">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="850e6-195">Nullable.</span></span>|
|<span data-ttu-id="850e6-196">users</span><span class="sxs-lookup"><span data-stu-id="850e6-196">users</span></span>|<span data-ttu-id="850e6-197">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="850e6-197">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="850e6-198">Пользователи в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="850e6-198">Users in the school.</span></span> <span data-ttu-id="850e6-199">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="850e6-199">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="850e6-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="850e6-200">JSON representation</span></span>

<span data-ttu-id="850e6-201">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="850e6-201">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
