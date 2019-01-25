---
title: Тип ресурса educationSchool
description: 'Учебное заведение. Ресурс **EducationSchool** в настоящее время соответствует ресурсу administrativeUnit, и у них общий идентификатор.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 917395324e6ae519af468a4bb4b31056796e1498
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512544"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="ca639-104">Тип ресурса educationSchool</span><span class="sxs-lookup"><span data-stu-id="ca639-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca639-105">Учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="ca639-105">A school.</span></span> <span data-ttu-id="ca639-106">Ресурс **EducationSchool** в настоящее время соответствует ресурсу [administrativeUnit](administrativeunit.md), и у них общий идентификатор.</span><span class="sxs-lookup"><span data-stu-id="ca639-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="ca639-107">Этот ресурс — подтип [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="ca639-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="ca639-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ca639-108">Methods</span></span>

| <span data-ttu-id="ca639-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ca639-109">Method</span></span>           | <span data-ttu-id="ca639-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ca639-110">Return Type</span></span>    |<span data-ttu-id="ca639-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ca639-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ca639-112">Get</span><span class="sxs-lookup"><span data-stu-id="ca639-112">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="ca639-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="ca639-113">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="ca639-114">Считывание свойств и отношений объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="ca639-114">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="ca639-115">Добавление класса</span><span class="sxs-lookup"><span data-stu-id="ca639-115">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="ca639-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="ca639-116">educationClass</span></span>](educationclass.md)| <span data-ttu-id="ca639-117">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.</span><span class="sxs-lookup"><span data-stu-id="ca639-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="ca639-118">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="ca639-118">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="ca639-119">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="ca639-119">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="ca639-120">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="ca639-120">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="ca639-121">Удаление класса</span><span class="sxs-lookup"><span data-stu-id="ca639-121">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="ca639-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="ca639-122">educationClass</span></span>](educationclass.md)| <span data-ttu-id="ca639-123">Удаление **educationClass** из учебного заведения через свойство навигации classes.</span><span class="sxs-lookup"><span data-stu-id="ca639-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="ca639-124">Добавление пользователя</span><span class="sxs-lookup"><span data-stu-id="ca639-124">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="ca639-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="ca639-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="ca639-126">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="ca639-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="ca639-127">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="ca639-127">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="ca639-128">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="ca639-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="ca639-129">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="ca639-129">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="ca639-130">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="ca639-130">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="ca639-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="ca639-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="ca639-132">Удаление **educationUser** из учебного заведения через свойство навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="ca639-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="ca639-133">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="ca639-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="ca639-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="ca639-134">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="ca639-135">Получение элемента **administrativeUnit**, соответствующего учебному заведению **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="ca639-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="ca639-136">Обновление</span><span class="sxs-lookup"><span data-stu-id="ca639-136">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="ca639-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="ca639-137">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="ca639-138">Обновление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="ca639-138">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="ca639-139">Удаление</span><span class="sxs-lookup"><span data-stu-id="ca639-139">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="ca639-140">None</span><span class="sxs-lookup"><span data-stu-id="ca639-140">None</span></span> |<span data-ttu-id="ca639-141">Удаление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="ca639-141">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ca639-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca639-142">Properties</span></span>
| <span data-ttu-id="ca639-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca639-143">Property</span></span>     | <span data-ttu-id="ca639-144">Тип</span><span class="sxs-lookup"><span data-stu-id="ca639-144">Type</span></span>   |<span data-ttu-id="ca639-145">Описание</span><span class="sxs-lookup"><span data-stu-id="ca639-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca639-146">id</span><span class="sxs-lookup"><span data-stu-id="ca639-146">id</span></span>|<span data-ttu-id="ca639-147">String</span><span class="sxs-lookup"><span data-stu-id="ca639-147">String</span></span>|<span data-ttu-id="ca639-148">GUID этого учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="ca639-148">GUID of this school.</span></span>|
|<span data-ttu-id="ca639-149">displayName</span><span class="sxs-lookup"><span data-stu-id="ca639-149">displayName</span></span>| <span data-ttu-id="ca639-150">String</span><span class="sxs-lookup"><span data-stu-id="ca639-150">String</span></span>| <span data-ttu-id="ca639-151">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="ca639-151">Display name of the school.</span></span>| 
|<span data-ttu-id="ca639-152">description</span><span class="sxs-lookup"><span data-stu-id="ca639-152">description</span></span>| <span data-ttu-id="ca639-153">Строка</span><span class="sxs-lookup"><span data-stu-id="ca639-153">String</span></span> | <span data-ttu-id="ca639-154">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="ca639-154">Description of the school.</span></span>| 
|<span data-ttu-id="ca639-155">status</span><span class="sxs-lookup"><span data-stu-id="ca639-155">status</span></span>| <span data-ttu-id="ca639-156">string</span><span class="sxs-lookup"><span data-stu-id="ca639-156">string</span></span>| <span data-ttu-id="ca639-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca639-157">Read-Only.</span></span> <span data-ttu-id="ca639-158">Возможные значения: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="ca639-158">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="ca639-159">externalSource</span><span class="sxs-lookup"><span data-stu-id="ca639-159">externalSource</span></span>| <span data-ttu-id="ca639-160">string</span><span class="sxs-lookup"><span data-stu-id="ca639-160">string</span></span>| <span data-ttu-id="ca639-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca639-161">Read-Only.</span></span>  <span data-ttu-id="ca639-162">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ca639-162">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ca639-163">principalEmail</span><span class="sxs-lookup"><span data-stu-id="ca639-163">principalEmail</span></span>| <span data-ttu-id="ca639-164">String</span><span class="sxs-lookup"><span data-stu-id="ca639-164">String</span></span>| <span data-ttu-id="ca639-165">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="ca639-165">Email address of the principal.</span></span>|
|<span data-ttu-id="ca639-166">principalName</span><span class="sxs-lookup"><span data-stu-id="ca639-166">principalName</span></span>| <span data-ttu-id="ca639-167">String</span><span class="sxs-lookup"><span data-stu-id="ca639-167">String</span></span> | <span data-ttu-id="ca639-168">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="ca639-168">Name of the principal.</span></span>|
|<span data-ttu-id="ca639-169">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="ca639-169">externalPrincipalId</span></span>| <span data-ttu-id="ca639-170">String</span><span class="sxs-lookup"><span data-stu-id="ca639-170">String</span></span> | <span data-ttu-id="ca639-171">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ca639-171">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="ca639-172">highestGrade</span><span class="sxs-lookup"><span data-stu-id="ca639-172">highestGrade</span></span>|<span data-ttu-id="ca639-173">String</span><span class="sxs-lookup"><span data-stu-id="ca639-173">String</span></span>| <span data-ttu-id="ca639-174">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="ca639-174">Highest grade taught.</span></span> |
|<span data-ttu-id="ca639-175">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="ca639-175">lowestGrade</span></span>|<span data-ttu-id="ca639-176">String</span><span class="sxs-lookup"><span data-stu-id="ca639-176">String</span></span>| <span data-ttu-id="ca639-177">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="ca639-177">Lowest grade taught.</span></span> |
|<span data-ttu-id="ca639-178">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="ca639-178">schoolNumber</span></span>|<span data-ttu-id="ca639-179">String</span><span class="sxs-lookup"><span data-stu-id="ca639-179">String</span></span>| <span data-ttu-id="ca639-180">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="ca639-180">School Number.</span></span>|
|<span data-ttu-id="ca639-181">externalId</span><span class="sxs-lookup"><span data-stu-id="ca639-181">externalId</span></span>|<span data-ttu-id="ca639-182">String</span><span class="sxs-lookup"><span data-stu-id="ca639-182">String</span></span>| <span data-ttu-id="ca639-183">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ca639-183">ID of school in syncing system.</span></span> |
|<span data-ttu-id="ca639-184">phone</span><span class="sxs-lookup"><span data-stu-id="ca639-184">phone</span></span>|<span data-ttu-id="ca639-185">String</span><span class="sxs-lookup"><span data-stu-id="ca639-185">String</span></span>| <span data-ttu-id="ca639-186">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="ca639-186">Phone number of school.</span></span> |
|<span data-ttu-id="ca639-187">fax</span><span class="sxs-lookup"><span data-stu-id="ca639-187">fax</span></span>|<span data-ttu-id="ca639-188">String</span><span class="sxs-lookup"><span data-stu-id="ca639-188">String</span></span>| <span data-ttu-id="ca639-189">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="ca639-189">Fax number of school.</span></span> |
|<span data-ttu-id="ca639-190">address</span><span class="sxs-lookup"><span data-stu-id="ca639-190">address</span></span>|[<span data-ttu-id="ca639-191">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="ca639-191">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="ca639-192">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="ca639-192">Address of the school.</span></span>|
|<span data-ttu-id="ca639-193">createdBy</span><span class="sxs-lookup"><span data-stu-id="ca639-193">createdBy</span></span>|[<span data-ttu-id="ca639-194">identitySet</span><span class="sxs-lookup"><span data-stu-id="ca639-194">identitySet</span></span>](identityset.md)|<span data-ttu-id="ca639-195">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="ca639-195">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="ca639-196">Связи</span><span class="sxs-lookup"><span data-stu-id="ca639-196">Relationships</span></span>
| <span data-ttu-id="ca639-197">Связь</span><span class="sxs-lookup"><span data-stu-id="ca639-197">Relationship</span></span> | <span data-ttu-id="ca639-198">Тип</span><span class="sxs-lookup"><span data-stu-id="ca639-198">Type</span></span>   |<span data-ttu-id="ca639-199">Описание</span><span class="sxs-lookup"><span data-stu-id="ca639-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca639-200">classes</span><span class="sxs-lookup"><span data-stu-id="ca639-200">classes</span></span>|<span data-ttu-id="ca639-201">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="ca639-201">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="ca639-202">Классы, которые обучаются в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="ca639-202">Classes taught at the school.</span></span> <span data-ttu-id="ca639-203">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ca639-203">Nullable.</span></span>|
|<span data-ttu-id="ca639-204">users</span><span class="sxs-lookup"><span data-stu-id="ca639-204">users</span></span>|<span data-ttu-id="ca639-205">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="ca639-205">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="ca639-206">Пользователи в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="ca639-206">Users in the school.</span></span> <span data-ttu-id="ca639-207">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ca639-207">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca639-208">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca639-208">JSON representation</span></span>

<span data-ttu-id="ca639-209">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca639-209">The following is a JSON representation of the resource.</span></span>

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
