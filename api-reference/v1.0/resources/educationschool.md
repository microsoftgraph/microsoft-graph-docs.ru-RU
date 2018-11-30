---
title: Тип ресурса educationSchool
description: 'Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.  '
ms.openlocfilehash: 8a87b3a0ceebf9a3dd66978da1bdde2d677ef63e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028118"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="2aa7c-103">Тип ресурса educationSchool</span><span class="sxs-lookup"><span data-stu-id="2aa7c-103">educationSchool resource type</span></span>

<span data-ttu-id="2aa7c-104">Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-104">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  


## <a name="methods"></a><span data-ttu-id="2aa7c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="2aa7c-105">Methods</span></span>

| <span data-ttu-id="2aa7c-106">Метод</span><span class="sxs-lookup"><span data-stu-id="2aa7c-106">Method</span></span>           | <span data-ttu-id="2aa7c-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2aa7c-107">Return Type</span></span>    |<span data-ttu-id="2aa7c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2aa7c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2aa7c-109">Get</span><span class="sxs-lookup"><span data-stu-id="2aa7c-109">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="2aa7c-110">educationSchool</span><span class="sxs-lookup"><span data-stu-id="2aa7c-110">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="2aa7c-111">Считывание свойств и отношений объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-111">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="2aa7c-112">Добавление класса</span><span class="sxs-lookup"><span data-stu-id="2aa7c-112">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="2aa7c-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="2aa7c-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="2aa7c-114">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-114">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="2aa7c-115">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="2aa7c-115">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="2aa7c-116">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="2aa7c-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="2aa7c-117">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-117">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="2aa7c-118">Удаление класса</span><span class="sxs-lookup"><span data-stu-id="2aa7c-118">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="2aa7c-119">educationClass</span><span class="sxs-lookup"><span data-stu-id="2aa7c-119">educationClass</span></span>](educationclass.md)| <span data-ttu-id="2aa7c-120">Удаление **educationClass** из учебного заведения через свойство навигации classes.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-120">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="2aa7c-121">Добавление пользователя</span><span class="sxs-lookup"><span data-stu-id="2aa7c-121">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="2aa7c-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="2aa7c-122">educationUser</span></span>](educationuser.md)| <span data-ttu-id="2aa7c-123">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-123">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="2aa7c-124">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="2aa7c-124">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="2aa7c-125">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="2aa7c-125">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="2aa7c-126">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-126">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="2aa7c-127">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="2aa7c-127">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="2aa7c-128">educationUser</span><span class="sxs-lookup"><span data-stu-id="2aa7c-128">educationUser</span></span>](educationuser.md)| <span data-ttu-id="2aa7c-129">Удаление **educationUser** из учебного заведения через свойство навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-129">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="2aa7c-130">Обновление</span><span class="sxs-lookup"><span data-stu-id="2aa7c-130">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="2aa7c-131">educationSchool</span><span class="sxs-lookup"><span data-stu-id="2aa7c-131">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="2aa7c-132">Обновление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-132">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="2aa7c-133">Удаление</span><span class="sxs-lookup"><span data-stu-id="2aa7c-133">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="2aa7c-134">None</span><span class="sxs-lookup"><span data-stu-id="2aa7c-134">None</span></span> |<span data-ttu-id="2aa7c-135">Удаление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-135">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2aa7c-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="2aa7c-136">Properties</span></span>
| <span data-ttu-id="2aa7c-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="2aa7c-137">Property</span></span>     | <span data-ttu-id="2aa7c-138">Тип</span><span class="sxs-lookup"><span data-stu-id="2aa7c-138">Type</span></span>   |<span data-ttu-id="2aa7c-139">Описание</span><span class="sxs-lookup"><span data-stu-id="2aa7c-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2aa7c-140">id</span><span class="sxs-lookup"><span data-stu-id="2aa7c-140">id</span></span>|<span data-ttu-id="2aa7c-141">String</span><span class="sxs-lookup"><span data-stu-id="2aa7c-141">String</span></span>|<span data-ttu-id="2aa7c-142">GUID этого учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-142">GUID of this school.</span></span>|
|<span data-ttu-id="2aa7c-143">displayName</span><span class="sxs-lookup"><span data-stu-id="2aa7c-143">displayName</span></span>| <span data-ttu-id="2aa7c-144">String</span><span class="sxs-lookup"><span data-stu-id="2aa7c-144">String</span></span>| <span data-ttu-id="2aa7c-145">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-145">Display name of the school.</span></span>| 
|<span data-ttu-id="2aa7c-146">описание</span><span class="sxs-lookup"><span data-stu-id="2aa7c-146">description</span></span>| <span data-ttu-id="2aa7c-147">String</span><span class="sxs-lookup"><span data-stu-id="2aa7c-147">String</span></span> | <span data-ttu-id="2aa7c-148">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-148">Description of the school.</span></span>| 
|<span data-ttu-id="2aa7c-149">status</span><span class="sxs-lookup"><span data-stu-id="2aa7c-149">status</span></span>| <span data-ttu-id="2aa7c-150">string</span><span class="sxs-lookup"><span data-stu-id="2aa7c-150">string</span></span>| <span data-ttu-id="2aa7c-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-151">Read-Only.</span></span> <span data-ttu-id="2aa7c-152">Возможные значения: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-152">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="2aa7c-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="2aa7c-153">externalSource</span></span>| <span data-ttu-id="2aa7c-154">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="2aa7c-154">educationExternalSource</span></span>| <span data-ttu-id="2aa7c-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-155">Read-Only.</span></span>  <span data-ttu-id="2aa7c-156">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-156">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2aa7c-157">principalEmail</span><span class="sxs-lookup"><span data-stu-id="2aa7c-157">principalEmail</span></span>| <span data-ttu-id="2aa7c-158">String</span><span class="sxs-lookup"><span data-stu-id="2aa7c-158">String</span></span>| <span data-ttu-id="2aa7c-159">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-159">Email address of the principal.</span></span>|
|<span data-ttu-id="2aa7c-160">principalName</span><span class="sxs-lookup"><span data-stu-id="2aa7c-160">principalName</span></span>| <span data-ttu-id="2aa7c-161">String</span><span class="sxs-lookup"><span data-stu-id="2aa7c-161">String</span></span> | <span data-ttu-id="2aa7c-162">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-162">Name of the principal.</span></span>|
|<span data-ttu-id="2aa7c-163">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="2aa7c-163">externalPrincipalId</span></span>| <span data-ttu-id="2aa7c-164">String</span><span class="sxs-lookup"><span data-stu-id="2aa7c-164">String</span></span> | <span data-ttu-id="2aa7c-165">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-165">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="2aa7c-166">highestGrade</span><span class="sxs-lookup"><span data-stu-id="2aa7c-166">highestGrade</span></span>|<span data-ttu-id="2aa7c-167">String</span><span class="sxs-lookup"><span data-stu-id="2aa7c-167">String</span></span>| <span data-ttu-id="2aa7c-168">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-168">Highest grade taught.</span></span> |
|<span data-ttu-id="2aa7c-169">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="2aa7c-169">lowestGrade</span></span>|<span data-ttu-id="2aa7c-170">String</span><span class="sxs-lookup"><span data-stu-id="2aa7c-170">String</span></span>| <span data-ttu-id="2aa7c-171">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-171">Lowest grade taught.</span></span> |
|<span data-ttu-id="2aa7c-172">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="2aa7c-172">schoolNumber</span></span>|<span data-ttu-id="2aa7c-173">String</span><span class="sxs-lookup"><span data-stu-id="2aa7c-173">String</span></span>| <span data-ttu-id="2aa7c-174">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-174">School Number.</span></span>|
|<span data-ttu-id="2aa7c-175">externalId</span><span class="sxs-lookup"><span data-stu-id="2aa7c-175">externalId</span></span>|<span data-ttu-id="2aa7c-176">String</span><span class="sxs-lookup"><span data-stu-id="2aa7c-176">String</span></span>| <span data-ttu-id="2aa7c-177">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-177">ID of school in syncing system.</span></span> |
|<span data-ttu-id="2aa7c-178">phone</span><span class="sxs-lookup"><span data-stu-id="2aa7c-178">phone</span></span>|<span data-ttu-id="2aa7c-179">String</span><span class="sxs-lookup"><span data-stu-id="2aa7c-179">String</span></span>| <span data-ttu-id="2aa7c-180">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-180">Phone number of school.</span></span> |
|<span data-ttu-id="2aa7c-181">fax</span><span class="sxs-lookup"><span data-stu-id="2aa7c-181">fax</span></span>|<span data-ttu-id="2aa7c-182">String</span><span class="sxs-lookup"><span data-stu-id="2aa7c-182">String</span></span>| <span data-ttu-id="2aa7c-183">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-183">Fax number of school.</span></span> |
|<span data-ttu-id="2aa7c-184">address</span><span class="sxs-lookup"><span data-stu-id="2aa7c-184">address</span></span>|[<span data-ttu-id="2aa7c-185">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2aa7c-185">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="2aa7c-186">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-186">Address of the school.</span></span>|
|<span data-ttu-id="2aa7c-187">createdBy</span><span class="sxs-lookup"><span data-stu-id="2aa7c-187">createdBy</span></span>|[<span data-ttu-id="2aa7c-188">identitySet</span><span class="sxs-lookup"><span data-stu-id="2aa7c-188">identitySet</span></span>](identityset.md)|<span data-ttu-id="2aa7c-189">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-189">Entity who created the school.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2aa7c-190">Связи</span><span class="sxs-lookup"><span data-stu-id="2aa7c-190">Relationships</span></span>
| <span data-ttu-id="2aa7c-191">Связь</span><span class="sxs-lookup"><span data-stu-id="2aa7c-191">Relationship</span></span> | <span data-ttu-id="2aa7c-192">Тип</span><span class="sxs-lookup"><span data-stu-id="2aa7c-192">Type</span></span>   |<span data-ttu-id="2aa7c-193">Описание</span><span class="sxs-lookup"><span data-stu-id="2aa7c-193">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2aa7c-194">classes</span><span class="sxs-lookup"><span data-stu-id="2aa7c-194">classes</span></span>|<span data-ttu-id="2aa7c-195">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="2aa7c-195">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="2aa7c-196">Классы, которые обучаются в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-196">Classes taught at the school.</span></span> <span data-ttu-id="2aa7c-197">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-197">Nullable.</span></span>|
|<span data-ttu-id="2aa7c-198">users</span><span class="sxs-lookup"><span data-stu-id="2aa7c-198">users</span></span>|<span data-ttu-id="2aa7c-199">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="2aa7c-199">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="2aa7c-200">Пользователи в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-200">Users in the school.</span></span> <span data-ttu-id="2aa7c-201">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-201">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2aa7c-202">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2aa7c-202">JSON representation</span></span>

<span data-ttu-id="2aa7c-203">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2aa7c-203">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
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
