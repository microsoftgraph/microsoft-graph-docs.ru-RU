---
title: Тип ресурса educationSchool
description: 'Учебное заведение. Ресурс **EducationSchool** в настоящее время соответствует ресурсу administrativeUnit, и у них общий идентификатор.  '
localization_priority: Normal
ms.openlocfilehash: 20eacb87b68cbf490131b98a15d3ab3239d73478
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830452"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="5a48f-104">Тип ресурса educationSchool</span><span class="sxs-lookup"><span data-stu-id="5a48f-104">educationSchool resource type</span></span>

> <span data-ttu-id="5a48f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5a48f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a48f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a48f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a48f-107">Учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="5a48f-107">A school.</span></span> <span data-ttu-id="5a48f-108">Ресурс **EducationSchool** в настоящее время соответствует ресурсу [administrativeUnit](administrativeunit.md), и у них общий идентификатор.</span><span class="sxs-lookup"><span data-stu-id="5a48f-108">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="5a48f-109">Этот ресурс — подтип [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="5a48f-109">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="5a48f-110">Методы</span><span class="sxs-lookup"><span data-stu-id="5a48f-110">Methods</span></span>

| <span data-ttu-id="5a48f-111">Метод</span><span class="sxs-lookup"><span data-stu-id="5a48f-111">Method</span></span>           | <span data-ttu-id="5a48f-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5a48f-112">Return Type</span></span>    |<span data-ttu-id="5a48f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="5a48f-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5a48f-114">Get</span><span class="sxs-lookup"><span data-stu-id="5a48f-114">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="5a48f-115">educationSchool</span><span class="sxs-lookup"><span data-stu-id="5a48f-115">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="5a48f-116">Считывание свойств и отношений объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="5a48f-116">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="5a48f-117">Добавление класса</span><span class="sxs-lookup"><span data-stu-id="5a48f-117">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="5a48f-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="5a48f-118">educationClass</span></span>](educationclass.md)| <span data-ttu-id="5a48f-119">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.</span><span class="sxs-lookup"><span data-stu-id="5a48f-119">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="5a48f-120">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="5a48f-120">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="5a48f-121">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="5a48f-121">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="5a48f-122">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="5a48f-122">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="5a48f-123">Удаление класса</span><span class="sxs-lookup"><span data-stu-id="5a48f-123">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="5a48f-124">educationClass</span><span class="sxs-lookup"><span data-stu-id="5a48f-124">educationClass</span></span>](educationclass.md)| <span data-ttu-id="5a48f-125">Удаление **educationClass** из учебного заведения через свойство навигации classes.</span><span class="sxs-lookup"><span data-stu-id="5a48f-125">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="5a48f-126">Добавление пользователя</span><span class="sxs-lookup"><span data-stu-id="5a48f-126">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="5a48f-127">educationUser</span><span class="sxs-lookup"><span data-stu-id="5a48f-127">educationUser</span></span>](educationuser.md)| <span data-ttu-id="5a48f-128">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="5a48f-128">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="5a48f-129">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="5a48f-129">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="5a48f-130">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="5a48f-130">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="5a48f-131">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="5a48f-131">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="5a48f-132">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="5a48f-132">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="5a48f-133">educationUser</span><span class="sxs-lookup"><span data-stu-id="5a48f-133">educationUser</span></span>](educationuser.md)| <span data-ttu-id="5a48f-134">Удаление **educationUser** из учебного заведения через свойство навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="5a48f-134">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="5a48f-135">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="5a48f-135">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="5a48f-136">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="5a48f-136">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="5a48f-137">Получение элемента **administrativeUnit**, соответствующего учебному заведению **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="5a48f-137">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="5a48f-138">Обновление</span><span class="sxs-lookup"><span data-stu-id="5a48f-138">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="5a48f-139">educationSchool</span><span class="sxs-lookup"><span data-stu-id="5a48f-139">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="5a48f-140">Обновление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="5a48f-140">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="5a48f-141">Удаление</span><span class="sxs-lookup"><span data-stu-id="5a48f-141">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="5a48f-142">None</span><span class="sxs-lookup"><span data-stu-id="5a48f-142">None</span></span> |<span data-ttu-id="5a48f-143">Удаление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="5a48f-143">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5a48f-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a48f-144">Properties</span></span>
| <span data-ttu-id="5a48f-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a48f-145">Property</span></span>     | <span data-ttu-id="5a48f-146">Тип</span><span class="sxs-lookup"><span data-stu-id="5a48f-146">Type</span></span>   |<span data-ttu-id="5a48f-147">Описание</span><span class="sxs-lookup"><span data-stu-id="5a48f-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a48f-148">id</span><span class="sxs-lookup"><span data-stu-id="5a48f-148">id</span></span>|<span data-ttu-id="5a48f-149">String</span><span class="sxs-lookup"><span data-stu-id="5a48f-149">String</span></span>|<span data-ttu-id="5a48f-150">GUID этого учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="5a48f-150">GUID of this school.</span></span>|
|<span data-ttu-id="5a48f-151">displayName</span><span class="sxs-lookup"><span data-stu-id="5a48f-151">displayName</span></span>| <span data-ttu-id="5a48f-152">String</span><span class="sxs-lookup"><span data-stu-id="5a48f-152">String</span></span>| <span data-ttu-id="5a48f-153">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="5a48f-153">Display name of the school.</span></span>| 
|<span data-ttu-id="5a48f-154">описание</span><span class="sxs-lookup"><span data-stu-id="5a48f-154">description</span></span>| <span data-ttu-id="5a48f-155">String</span><span class="sxs-lookup"><span data-stu-id="5a48f-155">String</span></span> | <span data-ttu-id="5a48f-156">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="5a48f-156">Description of the school.</span></span>| 
|<span data-ttu-id="5a48f-157">status</span><span class="sxs-lookup"><span data-stu-id="5a48f-157">status</span></span>| <span data-ttu-id="5a48f-158">string</span><span class="sxs-lookup"><span data-stu-id="5a48f-158">string</span></span>| <span data-ttu-id="5a48f-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a48f-159">Read-Only.</span></span> <span data-ttu-id="5a48f-160">Возможные значения: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="5a48f-160">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="5a48f-161">externalSource</span><span class="sxs-lookup"><span data-stu-id="5a48f-161">externalSource</span></span>| <span data-ttu-id="5a48f-162">string</span><span class="sxs-lookup"><span data-stu-id="5a48f-162">string</span></span>| <span data-ttu-id="5a48f-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a48f-163">Read-Only.</span></span>  <span data-ttu-id="5a48f-164">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5a48f-164">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5a48f-165">principalEmail</span><span class="sxs-lookup"><span data-stu-id="5a48f-165">principalEmail</span></span>| <span data-ttu-id="5a48f-166">String</span><span class="sxs-lookup"><span data-stu-id="5a48f-166">String</span></span>| <span data-ttu-id="5a48f-167">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="5a48f-167">Email address of the principal.</span></span>|
|<span data-ttu-id="5a48f-168">principalName</span><span class="sxs-lookup"><span data-stu-id="5a48f-168">principalName</span></span>| <span data-ttu-id="5a48f-169">String</span><span class="sxs-lookup"><span data-stu-id="5a48f-169">String</span></span> | <span data-ttu-id="5a48f-170">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="5a48f-170">Name of the principal.</span></span>|
|<span data-ttu-id="5a48f-171">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="5a48f-171">externalPrincipalId</span></span>| <span data-ttu-id="5a48f-172">String</span><span class="sxs-lookup"><span data-stu-id="5a48f-172">String</span></span> | <span data-ttu-id="5a48f-173">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5a48f-173">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="5a48f-174">highestGrade</span><span class="sxs-lookup"><span data-stu-id="5a48f-174">highestGrade</span></span>|<span data-ttu-id="5a48f-175">String</span><span class="sxs-lookup"><span data-stu-id="5a48f-175">String</span></span>| <span data-ttu-id="5a48f-176">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="5a48f-176">Highest grade taught.</span></span> |
|<span data-ttu-id="5a48f-177">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="5a48f-177">lowestGrade</span></span>|<span data-ttu-id="5a48f-178">String</span><span class="sxs-lookup"><span data-stu-id="5a48f-178">String</span></span>| <span data-ttu-id="5a48f-179">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="5a48f-179">Lowest grade taught.</span></span> |
|<span data-ttu-id="5a48f-180">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="5a48f-180">schoolNumber</span></span>|<span data-ttu-id="5a48f-181">String</span><span class="sxs-lookup"><span data-stu-id="5a48f-181">String</span></span>| <span data-ttu-id="5a48f-182">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="5a48f-182">School Number.</span></span>|
|<span data-ttu-id="5a48f-183">externalId</span><span class="sxs-lookup"><span data-stu-id="5a48f-183">externalId</span></span>|<span data-ttu-id="5a48f-184">String</span><span class="sxs-lookup"><span data-stu-id="5a48f-184">String</span></span>| <span data-ttu-id="5a48f-185">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5a48f-185">ID of school in syncing system.</span></span> |
|<span data-ttu-id="5a48f-186">phone</span><span class="sxs-lookup"><span data-stu-id="5a48f-186">phone</span></span>|<span data-ttu-id="5a48f-187">String</span><span class="sxs-lookup"><span data-stu-id="5a48f-187">String</span></span>| <span data-ttu-id="5a48f-188">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="5a48f-188">Phone number of school.</span></span> |
|<span data-ttu-id="5a48f-189">fax</span><span class="sxs-lookup"><span data-stu-id="5a48f-189">fax</span></span>|<span data-ttu-id="5a48f-190">String</span><span class="sxs-lookup"><span data-stu-id="5a48f-190">String</span></span>| <span data-ttu-id="5a48f-191">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="5a48f-191">Fax number of school.</span></span> |
|<span data-ttu-id="5a48f-192">address</span><span class="sxs-lookup"><span data-stu-id="5a48f-192">address</span></span>|[<span data-ttu-id="5a48f-193">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="5a48f-193">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="5a48f-194">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="5a48f-194">Address of the school.</span></span>|
|<span data-ttu-id="5a48f-195">createdBy</span><span class="sxs-lookup"><span data-stu-id="5a48f-195">createdBy</span></span>|[<span data-ttu-id="5a48f-196">identitySet</span><span class="sxs-lookup"><span data-stu-id="5a48f-196">identitySet</span></span>](identityset.md)|<span data-ttu-id="5a48f-197">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="5a48f-197">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="5a48f-198">Связи</span><span class="sxs-lookup"><span data-stu-id="5a48f-198">Relationships</span></span>
| <span data-ttu-id="5a48f-199">Связь</span><span class="sxs-lookup"><span data-stu-id="5a48f-199">Relationship</span></span> | <span data-ttu-id="5a48f-200">Тип</span><span class="sxs-lookup"><span data-stu-id="5a48f-200">Type</span></span>   |<span data-ttu-id="5a48f-201">Описание</span><span class="sxs-lookup"><span data-stu-id="5a48f-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a48f-202">classes</span><span class="sxs-lookup"><span data-stu-id="5a48f-202">classes</span></span>|<span data-ttu-id="5a48f-203">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="5a48f-203">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="5a48f-204">Классы, которые обучаются в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="5a48f-204">Classes taught at the school.</span></span> <span data-ttu-id="5a48f-205">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5a48f-205">Nullable.</span></span>|
|<span data-ttu-id="5a48f-206">users</span><span class="sxs-lookup"><span data-stu-id="5a48f-206">users</span></span>|<span data-ttu-id="5a48f-207">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="5a48f-207">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="5a48f-208">Пользователи в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="5a48f-208">Users in the school.</span></span> <span data-ttu-id="5a48f-209">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5a48f-209">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a48f-210">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a48f-210">JSON representation</span></span>

<span data-ttu-id="5a48f-211">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a48f-211">The following is a JSON representation of the resource.</span></span>

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
