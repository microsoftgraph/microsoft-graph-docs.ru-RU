---
title: Тип ресурса educationSchool
description: 'Учебное заведение. В настоящее время ресурс **educationSchool** соответствует ресурсу administrativeUnit и использует тот же идентификатор.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 917395324e6ae519af468a4bb4b31056796e1498
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542964"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="65fac-104">Тип ресурса educationSchool</span><span class="sxs-lookup"><span data-stu-id="65fac-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65fac-105">Учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="65fac-105">A school.</span></span> <span data-ttu-id="65fac-106">В настоящее время ресурс **educationSchool** соответствует ресурсу [administrativeUnit](administrativeunit.md) и использует тот же идентификатор.</span><span class="sxs-lookup"><span data-stu-id="65fac-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="65fac-107">Этот ресурс является подтипом [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="65fac-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="65fac-108">Методы</span><span class="sxs-lookup"><span data-stu-id="65fac-108">Methods</span></span>

| <span data-ttu-id="65fac-109">Метод</span><span class="sxs-lookup"><span data-stu-id="65fac-109">Method</span></span>           | <span data-ttu-id="65fac-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="65fac-110">Return Type</span></span>    |<span data-ttu-id="65fac-111">Описание</span><span class="sxs-lookup"><span data-stu-id="65fac-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65fac-112">Get</span><span class="sxs-lookup"><span data-stu-id="65fac-112">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="65fac-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="65fac-113">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="65fac-114">Считывание свойств и отношений объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="65fac-114">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="65fac-115">Добавление класса</span><span class="sxs-lookup"><span data-stu-id="65fac-115">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="65fac-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="65fac-116">educationClass</span></span>](educationclass.md)| <span data-ttu-id="65fac-117">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.</span><span class="sxs-lookup"><span data-stu-id="65fac-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="65fac-118">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="65fac-118">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="65fac-119">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="65fac-119">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="65fac-120">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="65fac-120">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="65fac-121">Удаление класса</span><span class="sxs-lookup"><span data-stu-id="65fac-121">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="65fac-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="65fac-122">educationClass</span></span>](educationclass.md)| <span data-ttu-id="65fac-123">Удаление **educationClass** из учебного заведения через свойство навигации classes.</span><span class="sxs-lookup"><span data-stu-id="65fac-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="65fac-124">Добавление пользователя</span><span class="sxs-lookup"><span data-stu-id="65fac-124">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="65fac-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="65fac-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="65fac-126">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="65fac-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="65fac-127">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="65fac-127">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="65fac-128">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="65fac-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="65fac-129">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="65fac-129">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="65fac-130">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="65fac-130">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="65fac-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="65fac-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="65fac-132">Удаление **educationUser** из учебного заведения через свойство навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="65fac-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="65fac-133">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="65fac-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="65fac-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="65fac-134">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="65fac-135">Получение **administrativeUnit** , соответствующего этому **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="65fac-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="65fac-136">Обновление</span><span class="sxs-lookup"><span data-stu-id="65fac-136">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="65fac-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="65fac-137">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="65fac-138">Обновление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="65fac-138">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="65fac-139">Удаление</span><span class="sxs-lookup"><span data-stu-id="65fac-139">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="65fac-140">Нет</span><span class="sxs-lookup"><span data-stu-id="65fac-140">None</span></span> |<span data-ttu-id="65fac-141">Удаление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="65fac-141">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="65fac-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="65fac-142">Properties</span></span>
| <span data-ttu-id="65fac-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="65fac-143">Property</span></span>     | <span data-ttu-id="65fac-144">Тип</span><span class="sxs-lookup"><span data-stu-id="65fac-144">Type</span></span>   |<span data-ttu-id="65fac-145">Описание</span><span class="sxs-lookup"><span data-stu-id="65fac-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65fac-146">id</span><span class="sxs-lookup"><span data-stu-id="65fac-146">id</span></span>|<span data-ttu-id="65fac-147">Строка</span><span class="sxs-lookup"><span data-stu-id="65fac-147">String</span></span>|<span data-ttu-id="65fac-148">GUID этого учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="65fac-148">GUID of this school.</span></span>|
|<span data-ttu-id="65fac-149">displayName</span><span class="sxs-lookup"><span data-stu-id="65fac-149">displayName</span></span>| <span data-ttu-id="65fac-150">String</span><span class="sxs-lookup"><span data-stu-id="65fac-150">String</span></span>| <span data-ttu-id="65fac-151">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="65fac-151">Display name of the school.</span></span>| 
|<span data-ttu-id="65fac-152">description</span><span class="sxs-lookup"><span data-stu-id="65fac-152">description</span></span>| <span data-ttu-id="65fac-153">String</span><span class="sxs-lookup"><span data-stu-id="65fac-153">String</span></span> | <span data-ttu-id="65fac-154">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="65fac-154">Description of the school.</span></span>| 
|<span data-ttu-id="65fac-155">status</span><span class="sxs-lookup"><span data-stu-id="65fac-155">status</span></span>| <span data-ttu-id="65fac-156">string</span><span class="sxs-lookup"><span data-stu-id="65fac-156">string</span></span>| <span data-ttu-id="65fac-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65fac-157">Read-Only.</span></span> <span data-ttu-id="65fac-158">Возможные значения: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="65fac-158">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="65fac-159">externalSource</span><span class="sxs-lookup"><span data-stu-id="65fac-159">externalSource</span></span>| <span data-ttu-id="65fac-160">string</span><span class="sxs-lookup"><span data-stu-id="65fac-160">string</span></span>| <span data-ttu-id="65fac-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65fac-161">Read-Only.</span></span>  <span data-ttu-id="65fac-162">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="65fac-162">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="65fac-163">principalEmail</span><span class="sxs-lookup"><span data-stu-id="65fac-163">principalEmail</span></span>| <span data-ttu-id="65fac-164">String</span><span class="sxs-lookup"><span data-stu-id="65fac-164">String</span></span>| <span data-ttu-id="65fac-165">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="65fac-165">Email address of the principal.</span></span>|
|<span data-ttu-id="65fac-166">principalName</span><span class="sxs-lookup"><span data-stu-id="65fac-166">principalName</span></span>| <span data-ttu-id="65fac-167">String</span><span class="sxs-lookup"><span data-stu-id="65fac-167">String</span></span> | <span data-ttu-id="65fac-168">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="65fac-168">Name of the principal.</span></span>|
|<span data-ttu-id="65fac-169">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="65fac-169">externalPrincipalId</span></span>| <span data-ttu-id="65fac-170">String</span><span class="sxs-lookup"><span data-stu-id="65fac-170">String</span></span> | <span data-ttu-id="65fac-171">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="65fac-171">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="65fac-172">highestGrade</span><span class="sxs-lookup"><span data-stu-id="65fac-172">highestGrade</span></span>|<span data-ttu-id="65fac-173">String</span><span class="sxs-lookup"><span data-stu-id="65fac-173">String</span></span>| <span data-ttu-id="65fac-174">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="65fac-174">Highest grade taught.</span></span> |
|<span data-ttu-id="65fac-175">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="65fac-175">lowestGrade</span></span>|<span data-ttu-id="65fac-176">String</span><span class="sxs-lookup"><span data-stu-id="65fac-176">String</span></span>| <span data-ttu-id="65fac-177">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="65fac-177">Lowest grade taught.</span></span> |
|<span data-ttu-id="65fac-178">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="65fac-178">schoolNumber</span></span>|<span data-ttu-id="65fac-179">String</span><span class="sxs-lookup"><span data-stu-id="65fac-179">String</span></span>| <span data-ttu-id="65fac-180">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="65fac-180">School Number.</span></span>|
|<span data-ttu-id="65fac-181">externalId</span><span class="sxs-lookup"><span data-stu-id="65fac-181">externalId</span></span>|<span data-ttu-id="65fac-182">String</span><span class="sxs-lookup"><span data-stu-id="65fac-182">String</span></span>| <span data-ttu-id="65fac-183">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="65fac-183">ID of school in syncing system.</span></span> |
|<span data-ttu-id="65fac-184">phone</span><span class="sxs-lookup"><span data-stu-id="65fac-184">phone</span></span>|<span data-ttu-id="65fac-185">String</span><span class="sxs-lookup"><span data-stu-id="65fac-185">String</span></span>| <span data-ttu-id="65fac-186">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="65fac-186">Phone number of school.</span></span> |
|<span data-ttu-id="65fac-187">fax</span><span class="sxs-lookup"><span data-stu-id="65fac-187">fax</span></span>|<span data-ttu-id="65fac-188">String</span><span class="sxs-lookup"><span data-stu-id="65fac-188">String</span></span>| <span data-ttu-id="65fac-189">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="65fac-189">Fax number of school.</span></span> |
|<span data-ttu-id="65fac-190">address</span><span class="sxs-lookup"><span data-stu-id="65fac-190">address</span></span>|[<span data-ttu-id="65fac-191">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="65fac-191">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="65fac-192">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="65fac-192">Address of the school.</span></span>|
|<span data-ttu-id="65fac-193">createdBy</span><span class="sxs-lookup"><span data-stu-id="65fac-193">createdBy</span></span>|[<span data-ttu-id="65fac-194">identitySet</span><span class="sxs-lookup"><span data-stu-id="65fac-194">identitySet</span></span>](identityset.md)|<span data-ttu-id="65fac-195">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="65fac-195">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="65fac-196">Связи</span><span class="sxs-lookup"><span data-stu-id="65fac-196">Relationships</span></span>
| <span data-ttu-id="65fac-197">Отношение</span><span class="sxs-lookup"><span data-stu-id="65fac-197">Relationship</span></span> | <span data-ttu-id="65fac-198">Тип</span><span class="sxs-lookup"><span data-stu-id="65fac-198">Type</span></span>   |<span data-ttu-id="65fac-199">Описание</span><span class="sxs-lookup"><span data-stu-id="65fac-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65fac-200">classes</span><span class="sxs-lookup"><span data-stu-id="65fac-200">classes</span></span>|<span data-ttu-id="65fac-201">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="65fac-201">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="65fac-202">Классы, которые обучаются в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="65fac-202">Classes taught at the school.</span></span> <span data-ttu-id="65fac-203">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="65fac-203">Nullable.</span></span>|
|<span data-ttu-id="65fac-204">users</span><span class="sxs-lookup"><span data-stu-id="65fac-204">users</span></span>|<span data-ttu-id="65fac-205">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="65fac-205">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="65fac-206">Пользователи в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="65fac-206">Users in the school.</span></span> <span data-ttu-id="65fac-207">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="65fac-207">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65fac-208">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65fac-208">JSON representation</span></span>

<span data-ttu-id="65fac-209">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65fac-209">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationschool.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
