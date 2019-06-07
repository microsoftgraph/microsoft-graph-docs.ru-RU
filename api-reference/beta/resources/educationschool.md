---
title: Тип ресурса educationSchool
description: 'Учебное заведение. В настоящее время ресурс **educationSchool** соответствует ресурсу administrativeUnit и использует тот же идентификатор.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9cded9db9ab9d7310a10ab690e05f49dca8711c8
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750145"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="dede7-104">Тип ресурса educationSchool</span><span class="sxs-lookup"><span data-stu-id="dede7-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dede7-105">Учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="dede7-105">A school.</span></span> <span data-ttu-id="dede7-106">В настоящее время ресурс **educationSchool** соответствует ресурсу [administrativeUnit](administrativeunit.md) и использует тот же идентификатор.</span><span class="sxs-lookup"><span data-stu-id="dede7-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="dede7-107">Этот ресурс является подтипом [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="dede7-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dede7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="dede7-108">Methods</span></span>

| <span data-ttu-id="dede7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="dede7-109">Method</span></span>                                                                     | <span data-ttu-id="dede7-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dede7-110">Return Type</span></span>                                      | <span data-ttu-id="dede7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dede7-111">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="dede7-112">Получение</span><span class="sxs-lookup"><span data-stu-id="dede7-112">Get</span></span>](../api/educationschool-get.md)                                       | [<span data-ttu-id="dede7-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="dede7-113">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="dede7-114">Считывание свойств и отношений объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="dede7-114">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="dede7-115">Добавление класса</span><span class="sxs-lookup"><span data-stu-id="dede7-115">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="dede7-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="dede7-116">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="dede7-117">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.</span><span class="sxs-lookup"><span data-stu-id="dede7-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="dede7-118">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="dede7-118">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="dede7-119">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="dede7-119">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="dede7-120">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="dede7-120">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="dede7-121">Удаление класса</span><span class="sxs-lookup"><span data-stu-id="dede7-121">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="dede7-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="dede7-122">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="dede7-123">Удаление **educationClass** из учебного заведения через свойство навигации classes.</span><span class="sxs-lookup"><span data-stu-id="dede7-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="dede7-124">Добавление пользователя</span><span class="sxs-lookup"><span data-stu-id="dede7-124">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="dede7-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="dede7-125">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="dede7-126">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="dede7-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="dede7-127">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="dede7-127">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="dede7-128">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="dede7-128">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="dede7-129">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="dede7-129">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="dede7-130">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="dede7-130">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="dede7-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="dede7-131">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="dede7-132">Удаление **educationUser** из учебного заведения через свойство навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="dede7-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="dede7-133">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="dede7-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="dede7-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="dede7-134">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="dede7-135">Получение **administrativeUnit** , соответствующего этому **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="dede7-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="dede7-136">Обновление</span><span class="sxs-lookup"><span data-stu-id="dede7-136">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="dede7-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="dede7-137">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="dede7-138">Обновление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="dede7-138">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="dede7-139">Удаление</span><span class="sxs-lookup"><span data-stu-id="dede7-139">Delete</span></span>](../api/educationschool-delete.md)                                 | <span data-ttu-id="dede7-140">Нет</span><span class="sxs-lookup"><span data-stu-id="dede7-140">None</span></span>                                             | <span data-ttu-id="dede7-141">Удаление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="dede7-141">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="dede7-142">Delta</span><span class="sxs-lookup"><span data-stu-id="dede7-142">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="dede7-143">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="dede7-143">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="dede7-144">Получение добавочных изменений для **едукатионсчулс**</span><span class="sxs-lookup"><span data-stu-id="dede7-144">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="dede7-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="dede7-145">Properties</span></span>

| <span data-ttu-id="dede7-146">Свойство</span><span class="sxs-lookup"><span data-stu-id="dede7-146">Property</span></span>            | <span data-ttu-id="dede7-147">Тип</span><span class="sxs-lookup"><span data-stu-id="dede7-147">Type</span></span>                                  | <span data-ttu-id="dede7-148">Описание</span><span class="sxs-lookup"><span data-stu-id="dede7-148">Description</span></span>                                        |
| :------------------ | :------------------------------------ | :------------------------------------------------- |
| <span data-ttu-id="dede7-149">id</span><span class="sxs-lookup"><span data-stu-id="dede7-149">id</span></span>                  | <span data-ttu-id="dede7-150">Строка</span><span class="sxs-lookup"><span data-stu-id="dede7-150">String</span></span>                                | <span data-ttu-id="dede7-151">GUID этого учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="dede7-151">GUID of this school.</span></span>                               |
| <span data-ttu-id="dede7-152">address</span><span class="sxs-lookup"><span data-stu-id="dede7-152">address</span></span>             | [<span data-ttu-id="dede7-153">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="dede7-153">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="dede7-154">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="dede7-154">Address of the school.</span></span>                             |
| <span data-ttu-id="dede7-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="dede7-155">createdBy</span></span>           | [<span data-ttu-id="dede7-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="dede7-156">identitySet</span></span>](identityset.md)         | <span data-ttu-id="dede7-157">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="dede7-157">Entity who created the school.</span></span>                     |
| <span data-ttu-id="dede7-158">description</span><span class="sxs-lookup"><span data-stu-id="dede7-158">description</span></span>         | <span data-ttu-id="dede7-159">String</span><span class="sxs-lookup"><span data-stu-id="dede7-159">String</span></span>                                | <span data-ttu-id="dede7-160">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="dede7-160">Description of the school.</span></span>                         |
| <span data-ttu-id="dede7-161">displayName</span><span class="sxs-lookup"><span data-stu-id="dede7-161">displayName</span></span>         | <span data-ttu-id="dede7-162">Строка</span><span class="sxs-lookup"><span data-stu-id="dede7-162">String</span></span>                                | <span data-ttu-id="dede7-163">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="dede7-163">Display name of the school.</span></span>                        |
| <span data-ttu-id="dede7-164">externalId</span><span class="sxs-lookup"><span data-stu-id="dede7-164">externalId</span></span>          | <span data-ttu-id="dede7-165">String</span><span class="sxs-lookup"><span data-stu-id="dede7-165">String</span></span>                                | <span data-ttu-id="dede7-166">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="dede7-166">ID of school in syncing system.</span></span>                    |
| <span data-ttu-id="dede7-167">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="dede7-167">externalPrincipalId</span></span> | <span data-ttu-id="dede7-168">String</span><span class="sxs-lookup"><span data-stu-id="dede7-168">String</span></span>                                | <span data-ttu-id="dede7-169">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="dede7-169">ID of principal in syncing system.</span></span>                 |
| <span data-ttu-id="dede7-170">externalSource</span><span class="sxs-lookup"><span data-stu-id="dede7-170">externalSource</span></span>      | <span data-ttu-id="dede7-171">string</span><span class="sxs-lookup"><span data-stu-id="dede7-171">string</span></span>                                | <span data-ttu-id="dede7-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dede7-172">Read-Only.</span></span> <span data-ttu-id="dede7-173">Возможные значения: `sis` или `manual`.</span><span class="sxs-lookup"><span data-stu-id="dede7-173">Possible values are: `sis` or `manual`.</span></span> |
| <span data-ttu-id="dede7-174">fax</span><span class="sxs-lookup"><span data-stu-id="dede7-174">fax</span></span>                 | <span data-ttu-id="dede7-175">String</span><span class="sxs-lookup"><span data-stu-id="dede7-175">String</span></span>                                | <span data-ttu-id="dede7-176">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="dede7-176">Fax number of school.</span></span>                              |
| <span data-ttu-id="dede7-177">highestGrade</span><span class="sxs-lookup"><span data-stu-id="dede7-177">highestGrade</span></span>        | <span data-ttu-id="dede7-178">String</span><span class="sxs-lookup"><span data-stu-id="dede7-178">String</span></span>                                | <span data-ttu-id="dede7-179">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="dede7-179">Highest grade taught.</span></span>                              |
| <span data-ttu-id="dede7-180">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="dede7-180">lowestGrade</span></span>         | <span data-ttu-id="dede7-181">String</span><span class="sxs-lookup"><span data-stu-id="dede7-181">String</span></span>                                | <span data-ttu-id="dede7-182">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="dede7-182">Lowest grade taught.</span></span>                               |
| <span data-ttu-id="dede7-183">phone</span><span class="sxs-lookup"><span data-stu-id="dede7-183">phone</span></span>               | <span data-ttu-id="dede7-184">String</span><span class="sxs-lookup"><span data-stu-id="dede7-184">String</span></span>                                | <span data-ttu-id="dede7-185">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="dede7-185">Phone number of school.</span></span>                            |
| <span data-ttu-id="dede7-186">principalEmail</span><span class="sxs-lookup"><span data-stu-id="dede7-186">principalEmail</span></span>      | <span data-ttu-id="dede7-187">String</span><span class="sxs-lookup"><span data-stu-id="dede7-187">String</span></span>                                | <span data-ttu-id="dede7-188">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="dede7-188">Email address of the principal.</span></span>                    |
| <span data-ttu-id="dede7-189">principalName</span><span class="sxs-lookup"><span data-stu-id="dede7-189">principalName</span></span>       | <span data-ttu-id="dede7-190">String</span><span class="sxs-lookup"><span data-stu-id="dede7-190">String</span></span>                                | <span data-ttu-id="dede7-191">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="dede7-191">Name of the principal.</span></span>                             |
| <span data-ttu-id="dede7-192">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="dede7-192">schoolNumber</span></span>        | <span data-ttu-id="dede7-193">String</span><span class="sxs-lookup"><span data-stu-id="dede7-193">String</span></span>                                | <span data-ttu-id="dede7-194">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="dede7-194">School Number.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="dede7-195">Отношения</span><span class="sxs-lookup"><span data-stu-id="dede7-195">Relationships</span></span>

| <span data-ttu-id="dede7-196">Отношение</span><span class="sxs-lookup"><span data-stu-id="dede7-196">Relationship</span></span> | <span data-ttu-id="dede7-197">Тип</span><span class="sxs-lookup"><span data-stu-id="dede7-197">Type</span></span>                                           | <span data-ttu-id="dede7-198">Описание</span><span class="sxs-lookup"><span data-stu-id="dede7-198">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="dede7-199">classes</span><span class="sxs-lookup"><span data-stu-id="dede7-199">classes</span></span>      | <span data-ttu-id="dede7-200">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="dede7-200">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="dede7-201">Классы, которые обучаются в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="dede7-201">Classes taught at the school.</span></span> <span data-ttu-id="dede7-202">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="dede7-202">Nullable.</span></span> |
| <span data-ttu-id="dede7-203">users</span><span class="sxs-lookup"><span data-stu-id="dede7-203">users</span></span>        | <span data-ttu-id="dede7-204">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="dede7-204">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="dede7-205">Пользователи в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="dede7-205">Users in the school.</span></span> <span data-ttu-id="dede7-206">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="dede7-206">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="dede7-207">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dede7-207">JSON representation</span></span>

<span data-ttu-id="dede7-208">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dede7-208">The following is a JSON representation of the resource.</span></span>

<!-- {
"blockType": "resource",
"keyProperty": "id",
"optionalProperties": [

],
"@odata.type": "microsoft.graph.educationSchool"
}-->


```json
{
  "address": { "@odata.type": "microsoft.graph.physicalAddress" },
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalPrincipalId": "String",
  "externalSource": "string",
  "fax": "String",
  "highestGrade": "String",
  "id": "String (identifier)",
  "lowestGrade": "String",
  "phone": "String",
  "principalEmail": "String",
  "principalName": "String",
  "schoolNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
    "Error: Resource educationSchool has documented navigation properties, but we thought it was a complex type!" 
  ]  
}-->
