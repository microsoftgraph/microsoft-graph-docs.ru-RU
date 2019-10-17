---
title: Тип ресурса educationSchool
description: 'Учебное заведение. В настоящее время ресурс **educationSchool** соответствует ресурсу administrativeUnit и использует тот же идентификатор.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e63fa37dacea7fee6d4378a2a6040a5cf71f3790
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37553938"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="f5705-104">Тип ресурса educationSchool</span><span class="sxs-lookup"><span data-stu-id="f5705-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5705-105">Учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="f5705-105">A school.</span></span> <span data-ttu-id="f5705-106">В настоящее время ресурс **educationSchool** соответствует ресурсу [administrativeUnit](administrativeunit.md) и использует тот же идентификатор.</span><span class="sxs-lookup"><span data-stu-id="f5705-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="f5705-107">Этот ресурс является подтипом [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="f5705-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f5705-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f5705-108">Methods</span></span>

| <span data-ttu-id="f5705-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f5705-109">Method</span></span>                                                                     | <span data-ttu-id="f5705-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f5705-110">Return Type</span></span>                                      | <span data-ttu-id="f5705-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f5705-111">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="f5705-112">Получение</span><span class="sxs-lookup"><span data-stu-id="f5705-112">Get</span></span>](../api/educationschool-get.md)                                       | [<span data-ttu-id="f5705-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="f5705-113">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="f5705-114">Считывание свойств и отношений объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="f5705-114">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="f5705-115">Добавление класса</span><span class="sxs-lookup"><span data-stu-id="f5705-115">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="f5705-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="f5705-116">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="f5705-117">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.</span><span class="sxs-lookup"><span data-stu-id="f5705-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="f5705-118">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="f5705-118">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="f5705-119">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="f5705-119">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="f5705-120">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="f5705-120">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="f5705-121">Удаление класса</span><span class="sxs-lookup"><span data-stu-id="f5705-121">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="f5705-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="f5705-122">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="f5705-123">Удаление **educationClass** из учебного заведения через свойство навигации classes.</span><span class="sxs-lookup"><span data-stu-id="f5705-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="f5705-124">Добавление пользователя</span><span class="sxs-lookup"><span data-stu-id="f5705-124">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="f5705-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="f5705-125">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="f5705-126">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="f5705-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="f5705-127">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="f5705-127">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="f5705-128">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="f5705-128">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="f5705-129">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="f5705-129">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="f5705-130">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="f5705-130">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="f5705-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="f5705-131">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="f5705-132">Удаление **educationUser** из учебного заведения через свойство навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="f5705-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="f5705-133">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="f5705-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="f5705-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="f5705-134">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="f5705-135">Получение **administrativeUnit** , соответствующего этому **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="f5705-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="f5705-136">Обновление</span><span class="sxs-lookup"><span data-stu-id="f5705-136">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="f5705-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="f5705-137">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="f5705-138">Обновление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="f5705-138">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="f5705-139">Удаление</span><span class="sxs-lookup"><span data-stu-id="f5705-139">Delete</span></span>](../api/educationschool-delete.md)                                 | <span data-ttu-id="f5705-140">Нет</span><span class="sxs-lookup"><span data-stu-id="f5705-140">None</span></span>                                             | <span data-ttu-id="f5705-141">Удаление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="f5705-141">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="f5705-142">Delta</span><span class="sxs-lookup"><span data-stu-id="f5705-142">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="f5705-143">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="f5705-143">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="f5705-144">Получение добавочных изменений для **едукатионсчулс**</span><span class="sxs-lookup"><span data-stu-id="f5705-144">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="f5705-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5705-145">Properties</span></span>

| <span data-ttu-id="f5705-146">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5705-146">Property</span></span>            | <span data-ttu-id="f5705-147">Тип</span><span class="sxs-lookup"><span data-stu-id="f5705-147">Type</span></span>                                  | <span data-ttu-id="f5705-148">Описание</span><span class="sxs-lookup"><span data-stu-id="f5705-148">Description</span></span>                                        |
| :------------------ | :------------------------------------ | :------------------------------------------------- |
| <span data-ttu-id="f5705-149">id</span><span class="sxs-lookup"><span data-stu-id="f5705-149">id</span></span>                  | <span data-ttu-id="f5705-150">Строка</span><span class="sxs-lookup"><span data-stu-id="f5705-150">String</span></span>                                | <span data-ttu-id="f5705-151">GUID этого учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f5705-151">GUID of this school.</span></span>                               |
| <span data-ttu-id="f5705-152">address</span><span class="sxs-lookup"><span data-stu-id="f5705-152">address</span></span>             | [<span data-ttu-id="f5705-153">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="f5705-153">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="f5705-154">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f5705-154">Address of the school.</span></span>                             |
| <span data-ttu-id="f5705-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="f5705-155">createdBy</span></span>           | [<span data-ttu-id="f5705-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="f5705-156">identitySet</span></span>](identityset.md)         | <span data-ttu-id="f5705-157">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="f5705-157">Entity who created the school.</span></span>                     |
| <span data-ttu-id="f5705-158">description</span><span class="sxs-lookup"><span data-stu-id="f5705-158">description</span></span>         | <span data-ttu-id="f5705-159">String</span><span class="sxs-lookup"><span data-stu-id="f5705-159">String</span></span>                                | <span data-ttu-id="f5705-160">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f5705-160">Description of the school.</span></span>                         |
| <span data-ttu-id="f5705-161">displayName</span><span class="sxs-lookup"><span data-stu-id="f5705-161">displayName</span></span>         | <span data-ttu-id="f5705-162">Строка</span><span class="sxs-lookup"><span data-stu-id="f5705-162">String</span></span>                                | <span data-ttu-id="f5705-163">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f5705-163">Display name of the school.</span></span>                        |
| <span data-ttu-id="f5705-164">externalId</span><span class="sxs-lookup"><span data-stu-id="f5705-164">externalId</span></span>          | <span data-ttu-id="f5705-165">String</span><span class="sxs-lookup"><span data-stu-id="f5705-165">String</span></span>                                | <span data-ttu-id="f5705-166">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f5705-166">ID of school in syncing system.</span></span>                    |
| <span data-ttu-id="f5705-167">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="f5705-167">externalPrincipalId</span></span> | <span data-ttu-id="f5705-168">String</span><span class="sxs-lookup"><span data-stu-id="f5705-168">String</span></span>                                | <span data-ttu-id="f5705-169">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f5705-169">ID of principal in syncing system.</span></span>                 |
| <span data-ttu-id="f5705-170">externalSource</span><span class="sxs-lookup"><span data-stu-id="f5705-170">externalSource</span></span>      | <span data-ttu-id="f5705-171">string</span><span class="sxs-lookup"><span data-stu-id="f5705-171">string</span></span>                                | <span data-ttu-id="f5705-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5705-172">Read-Only.</span></span> <span data-ttu-id="f5705-173">Возможные значения: `sis` или `manual`.</span><span class="sxs-lookup"><span data-stu-id="f5705-173">Possible values are: `sis` or `manual`.</span></span> |
| <span data-ttu-id="f5705-174">highestGrade</span><span class="sxs-lookup"><span data-stu-id="f5705-174">highestGrade</span></span>        | <span data-ttu-id="f5705-175">String</span><span class="sxs-lookup"><span data-stu-id="f5705-175">String</span></span>                                | <span data-ttu-id="f5705-176">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="f5705-176">Highest grade taught.</span></span>                              |
| <span data-ttu-id="f5705-177">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="f5705-177">lowestGrade</span></span>         | <span data-ttu-id="f5705-178">String</span><span class="sxs-lookup"><span data-stu-id="f5705-178">String</span></span>                                | <span data-ttu-id="f5705-179">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="f5705-179">Lowest grade taught.</span></span>                               |
| <span data-ttu-id="f5705-180">phone</span><span class="sxs-lookup"><span data-stu-id="f5705-180">phone</span></span>               | <span data-ttu-id="f5705-181">String</span><span class="sxs-lookup"><span data-stu-id="f5705-181">String</span></span>                                | <span data-ttu-id="f5705-182">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f5705-182">Phone number of school.</span></span>                            |
| <span data-ttu-id="f5705-183">principalEmail</span><span class="sxs-lookup"><span data-stu-id="f5705-183">principalEmail</span></span>      | <span data-ttu-id="f5705-184">String</span><span class="sxs-lookup"><span data-stu-id="f5705-184">String</span></span>                                | <span data-ttu-id="f5705-185">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="f5705-185">Email address of the principal.</span></span>                    |
| <span data-ttu-id="f5705-186">principalName</span><span class="sxs-lookup"><span data-stu-id="f5705-186">principalName</span></span>       | <span data-ttu-id="f5705-187">String</span><span class="sxs-lookup"><span data-stu-id="f5705-187">String</span></span>                                | <span data-ttu-id="f5705-188">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="f5705-188">Name of the principal.</span></span>                             |
| <span data-ttu-id="f5705-189">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="f5705-189">schoolNumber</span></span>        | <span data-ttu-id="f5705-190">String</span><span class="sxs-lookup"><span data-stu-id="f5705-190">String</span></span>                                | <span data-ttu-id="f5705-191">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="f5705-191">School Number.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="f5705-192">Связи</span><span class="sxs-lookup"><span data-stu-id="f5705-192">Relationships</span></span>

| <span data-ttu-id="f5705-193">Связь</span><span class="sxs-lookup"><span data-stu-id="f5705-193">Relationship</span></span> | <span data-ttu-id="f5705-194">Тип</span><span class="sxs-lookup"><span data-stu-id="f5705-194">Type</span></span>                                           | <span data-ttu-id="f5705-195">Описание</span><span class="sxs-lookup"><span data-stu-id="f5705-195">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="f5705-196">classes</span><span class="sxs-lookup"><span data-stu-id="f5705-196">classes</span></span>      | <span data-ttu-id="f5705-197">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="f5705-197">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="f5705-198">Классы, которые обучаются в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="f5705-198">Classes taught at the school.</span></span> <span data-ttu-id="f5705-199">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f5705-199">Nullable.</span></span> |
| <span data-ttu-id="f5705-200">users</span><span class="sxs-lookup"><span data-stu-id="f5705-200">users</span></span>        | <span data-ttu-id="f5705-201">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="f5705-201">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="f5705-202">Пользователи в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="f5705-202">Users in the school.</span></span> <span data-ttu-id="f5705-203">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f5705-203">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="f5705-204">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5705-204">JSON representation</span></span>

<span data-ttu-id="f5705-205">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5705-205">The following is a JSON representation of the resource.</span></span>

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
