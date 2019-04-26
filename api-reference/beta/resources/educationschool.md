---
title: Тип ресурса educationSchool
description: 'Учебное заведение. В настоящее время ресурс **educationSchool** соответствует ресурсу administrativeUnit и использует тот же идентификатор.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 893f01fffcc606c85cec30789ec94dd658b2a4b2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334200"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="eb6fb-104">Тип ресурса educationSchool</span><span class="sxs-lookup"><span data-stu-id="eb6fb-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb6fb-105">Учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-105">A school.</span></span> <span data-ttu-id="eb6fb-106">В настоящее время ресурс **educationSchool** соответствует ресурсу [administrativeUnit](administrativeunit.md) и использует тот же идентификатор.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="eb6fb-107">Этот ресурс является подтипом [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="eb6fb-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="eb6fb-108">Методы</span><span class="sxs-lookup"><span data-stu-id="eb6fb-108">Methods</span></span>

| <span data-ttu-id="eb6fb-109">Метод</span><span class="sxs-lookup"><span data-stu-id="eb6fb-109">Method</span></span>           | <span data-ttu-id="eb6fb-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eb6fb-110">Return Type</span></span>    |<span data-ttu-id="eb6fb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eb6fb-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eb6fb-112">Получение</span><span class="sxs-lookup"><span data-stu-id="eb6fb-112">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="eb6fb-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="eb6fb-113">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="eb6fb-114">Считывание свойств и отношений объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-114">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="eb6fb-115">Добавление класса</span><span class="sxs-lookup"><span data-stu-id="eb6fb-115">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="eb6fb-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="eb6fb-116">educationClass</span></span>](educationclass.md)| <span data-ttu-id="eb6fb-117">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="eb6fb-118">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="eb6fb-118">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="eb6fb-119">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="eb6fb-119">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="eb6fb-120">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-120">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="eb6fb-121">Удаление класса</span><span class="sxs-lookup"><span data-stu-id="eb6fb-121">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="eb6fb-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="eb6fb-122">educationClass</span></span>](educationclass.md)| <span data-ttu-id="eb6fb-123">Удаление **educationClass** из учебного заведения через свойство навигации classes.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="eb6fb-124">Добавление пользователя</span><span class="sxs-lookup"><span data-stu-id="eb6fb-124">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="eb6fb-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="eb6fb-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="eb6fb-126">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="eb6fb-127">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="eb6fb-127">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="eb6fb-128">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="eb6fb-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="eb6fb-129">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-129">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="eb6fb-130">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="eb6fb-130">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="eb6fb-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="eb6fb-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="eb6fb-132">Удаление **educationUser** из учебного заведения через свойство навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="eb6fb-133">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="eb6fb-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="eb6fb-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="eb6fb-134">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="eb6fb-135">Получение **administrativeUnit** , соответствующего этому **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="eb6fb-136">Обновление</span><span class="sxs-lookup"><span data-stu-id="eb6fb-136">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="eb6fb-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="eb6fb-137">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="eb6fb-138">Обновление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-138">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="eb6fb-139">Delete</span><span class="sxs-lookup"><span data-stu-id="eb6fb-139">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="eb6fb-140">Нет</span><span class="sxs-lookup"><span data-stu-id="eb6fb-140">None</span></span> |<span data-ttu-id="eb6fb-141">Удаление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-141">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="eb6fb-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb6fb-142">Properties</span></span>
| <span data-ttu-id="eb6fb-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb6fb-143">Property</span></span>     | <span data-ttu-id="eb6fb-144">Тип</span><span class="sxs-lookup"><span data-stu-id="eb6fb-144">Type</span></span>   |<span data-ttu-id="eb6fb-145">Описание</span><span class="sxs-lookup"><span data-stu-id="eb6fb-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb6fb-146">id</span><span class="sxs-lookup"><span data-stu-id="eb6fb-146">id</span></span>|<span data-ttu-id="eb6fb-147">Строка</span><span class="sxs-lookup"><span data-stu-id="eb6fb-147">String</span></span>|<span data-ttu-id="eb6fb-148">GUID этого учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-148">GUID of this school.</span></span>|
|<span data-ttu-id="eb6fb-149">displayName</span><span class="sxs-lookup"><span data-stu-id="eb6fb-149">displayName</span></span>| <span data-ttu-id="eb6fb-150">String</span><span class="sxs-lookup"><span data-stu-id="eb6fb-150">String</span></span>| <span data-ttu-id="eb6fb-151">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-151">Display name of the school.</span></span>| 
|<span data-ttu-id="eb6fb-152">description</span><span class="sxs-lookup"><span data-stu-id="eb6fb-152">description</span></span>| <span data-ttu-id="eb6fb-153">Строка</span><span class="sxs-lookup"><span data-stu-id="eb6fb-153">String</span></span> | <span data-ttu-id="eb6fb-154">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-154">Description of the school.</span></span>| 
|<span data-ttu-id="eb6fb-155">status</span><span class="sxs-lookup"><span data-stu-id="eb6fb-155">status</span></span>| <span data-ttu-id="eb6fb-156">string</span><span class="sxs-lookup"><span data-stu-id="eb6fb-156">string</span></span>| <span data-ttu-id="eb6fb-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-157">Read-Only.</span></span> <span data-ttu-id="eb6fb-158">Возможные значения: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-158">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="eb6fb-159">externalSource</span><span class="sxs-lookup"><span data-stu-id="eb6fb-159">externalSource</span></span>| <span data-ttu-id="eb6fb-160">string</span><span class="sxs-lookup"><span data-stu-id="eb6fb-160">string</span></span>| <span data-ttu-id="eb6fb-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-161">Read-Only.</span></span>  <span data-ttu-id="eb6fb-162">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-162">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="eb6fb-163">principalEmail</span><span class="sxs-lookup"><span data-stu-id="eb6fb-163">principalEmail</span></span>| <span data-ttu-id="eb6fb-164">String</span><span class="sxs-lookup"><span data-stu-id="eb6fb-164">String</span></span>| <span data-ttu-id="eb6fb-165">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-165">Email address of the principal.</span></span>|
|<span data-ttu-id="eb6fb-166">principalName</span><span class="sxs-lookup"><span data-stu-id="eb6fb-166">principalName</span></span>| <span data-ttu-id="eb6fb-167">String</span><span class="sxs-lookup"><span data-stu-id="eb6fb-167">String</span></span> | <span data-ttu-id="eb6fb-168">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-168">Name of the principal.</span></span>|
|<span data-ttu-id="eb6fb-169">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="eb6fb-169">externalPrincipalId</span></span>| <span data-ttu-id="eb6fb-170">String</span><span class="sxs-lookup"><span data-stu-id="eb6fb-170">String</span></span> | <span data-ttu-id="eb6fb-171">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-171">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="eb6fb-172">highestGrade</span><span class="sxs-lookup"><span data-stu-id="eb6fb-172">highestGrade</span></span>|<span data-ttu-id="eb6fb-173">String</span><span class="sxs-lookup"><span data-stu-id="eb6fb-173">String</span></span>| <span data-ttu-id="eb6fb-174">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-174">Highest grade taught.</span></span> |
|<span data-ttu-id="eb6fb-175">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="eb6fb-175">lowestGrade</span></span>|<span data-ttu-id="eb6fb-176">String</span><span class="sxs-lookup"><span data-stu-id="eb6fb-176">String</span></span>| <span data-ttu-id="eb6fb-177">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-177">Lowest grade taught.</span></span> |
|<span data-ttu-id="eb6fb-178">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="eb6fb-178">schoolNumber</span></span>|<span data-ttu-id="eb6fb-179">String</span><span class="sxs-lookup"><span data-stu-id="eb6fb-179">String</span></span>| <span data-ttu-id="eb6fb-180">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-180">School Number.</span></span>|
|<span data-ttu-id="eb6fb-181">externalId</span><span class="sxs-lookup"><span data-stu-id="eb6fb-181">externalId</span></span>|<span data-ttu-id="eb6fb-182">String</span><span class="sxs-lookup"><span data-stu-id="eb6fb-182">String</span></span>| <span data-ttu-id="eb6fb-183">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-183">ID of school in syncing system.</span></span> |
|<span data-ttu-id="eb6fb-184">phone</span><span class="sxs-lookup"><span data-stu-id="eb6fb-184">phone</span></span>|<span data-ttu-id="eb6fb-185">String</span><span class="sxs-lookup"><span data-stu-id="eb6fb-185">String</span></span>| <span data-ttu-id="eb6fb-186">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-186">Phone number of school.</span></span> |
|<span data-ttu-id="eb6fb-187">fax</span><span class="sxs-lookup"><span data-stu-id="eb6fb-187">fax</span></span>|<span data-ttu-id="eb6fb-188">String</span><span class="sxs-lookup"><span data-stu-id="eb6fb-188">String</span></span>| <span data-ttu-id="eb6fb-189">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-189">Fax number of school.</span></span> |
|<span data-ttu-id="eb6fb-190">address</span><span class="sxs-lookup"><span data-stu-id="eb6fb-190">address</span></span>|[<span data-ttu-id="eb6fb-191">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="eb6fb-191">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="eb6fb-192">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-192">Address of the school.</span></span>|
|<span data-ttu-id="eb6fb-193">createdBy</span><span class="sxs-lookup"><span data-stu-id="eb6fb-193">createdBy</span></span>|[<span data-ttu-id="eb6fb-194">identitySet</span><span class="sxs-lookup"><span data-stu-id="eb6fb-194">identitySet</span></span>](identityset.md)|<span data-ttu-id="eb6fb-195">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-195">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="eb6fb-196">Отношения</span><span class="sxs-lookup"><span data-stu-id="eb6fb-196">Relationships</span></span>
| <span data-ttu-id="eb6fb-197">Отношение</span><span class="sxs-lookup"><span data-stu-id="eb6fb-197">Relationship</span></span> | <span data-ttu-id="eb6fb-198">Тип</span><span class="sxs-lookup"><span data-stu-id="eb6fb-198">Type</span></span>   |<span data-ttu-id="eb6fb-199">Описание</span><span class="sxs-lookup"><span data-stu-id="eb6fb-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb6fb-200">classes</span><span class="sxs-lookup"><span data-stu-id="eb6fb-200">classes</span></span>|<span data-ttu-id="eb6fb-201">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="eb6fb-201">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="eb6fb-202">Классы, которые обучаются в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-202">Classes taught at the school.</span></span> <span data-ttu-id="eb6fb-203">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-203">Nullable.</span></span>|
|<span data-ttu-id="eb6fb-204">users</span><span class="sxs-lookup"><span data-stu-id="eb6fb-204">users</span></span>|<span data-ttu-id="eb6fb-205">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="eb6fb-205">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="eb6fb-206">Пользователи в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-206">Users in the school.</span></span> <span data-ttu-id="eb6fb-207">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-207">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb6fb-208">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb6fb-208">JSON representation</span></span>

<span data-ttu-id="eb6fb-209">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb6fb-209">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
<!--
{
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
