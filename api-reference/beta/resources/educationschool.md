---
title: Тип ресурса educationSchool
description: 'Учебное заведение. В настоящее время ресурс **educationSchool** соответствует ресурсу administrativeUnit и использует тот же идентификатор.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 67baa3f5a57e968b53ae3f51a6c49b3743be25a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500949"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="b9413-104">Тип ресурса educationSchool</span><span class="sxs-lookup"><span data-stu-id="b9413-104">educationSchool resource type</span></span>

<span data-ttu-id="b9413-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9413-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9413-106">Учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="b9413-106">A school.</span></span> <span data-ttu-id="b9413-107">В настоящее время ресурс **educationSchool** соответствует ресурсу [administrativeUnit](administrativeunit.md) и использует тот же идентификатор.</span><span class="sxs-lookup"><span data-stu-id="b9413-107">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="b9413-108">Этот ресурс является подтипом [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="b9413-108">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b9413-109">Методы</span><span class="sxs-lookup"><span data-stu-id="b9413-109">Methods</span></span>

| <span data-ttu-id="b9413-110">Метод</span><span class="sxs-lookup"><span data-stu-id="b9413-110">Method</span></span>                                                                     | <span data-ttu-id="b9413-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b9413-111">Return Type</span></span>                                      | <span data-ttu-id="b9413-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b9413-112">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="b9413-113">[получение](../api/educationschool-get.md);</span><span class="sxs-lookup"><span data-stu-id="b9413-113">[Get](../api/educationschool-get.md)</span></span>                                       | [<span data-ttu-id="b9413-114">educationSchool</span><span class="sxs-lookup"><span data-stu-id="b9413-114">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="b9413-115">Считывание свойств и отношений объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="b9413-115">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="b9413-116">Добавление класса</span><span class="sxs-lookup"><span data-stu-id="b9413-116">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="b9413-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="b9413-117">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="b9413-118">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.</span><span class="sxs-lookup"><span data-stu-id="b9413-118">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="b9413-119">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="b9413-119">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="b9413-120">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="b9413-120">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="b9413-121">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="b9413-121">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="b9413-122">Удаление класса</span><span class="sxs-lookup"><span data-stu-id="b9413-122">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="b9413-123">educationClass</span><span class="sxs-lookup"><span data-stu-id="b9413-123">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="b9413-124">Удаление **educationClass** из учебного заведения через свойство навигации classes.</span><span class="sxs-lookup"><span data-stu-id="b9413-124">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="b9413-125">Добавление пользователя</span><span class="sxs-lookup"><span data-stu-id="b9413-125">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="b9413-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="b9413-126">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="b9413-127">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="b9413-127">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="b9413-128">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="b9413-128">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="b9413-129">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="b9413-129">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="b9413-130">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="b9413-130">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="b9413-131">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="b9413-131">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="b9413-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="b9413-132">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="b9413-133">Удаление **educationUser** из учебного заведения через свойство навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="b9413-133">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="b9413-134">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="b9413-134">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="b9413-135">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="b9413-135">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="b9413-136">Получение **administrativeUnit** , соответствующего этому **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="b9413-136">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="b9413-137">Обновление</span><span class="sxs-lookup"><span data-stu-id="b9413-137">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="b9413-138">educationSchool</span><span class="sxs-lookup"><span data-stu-id="b9413-138">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="b9413-139">Обновление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="b9413-139">Update an **educationSchool** object.</span></span>                                                       |
| <span data-ttu-id="b9413-140">[удаление](../api/educationschool-delete.md);</span><span class="sxs-lookup"><span data-stu-id="b9413-140">[Delete](../api/educationschool-delete.md)</span></span>                                 | <span data-ttu-id="b9413-141">Нет</span><span class="sxs-lookup"><span data-stu-id="b9413-141">None</span></span>                                             | <span data-ttu-id="b9413-142">Удаление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="b9413-142">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="b9413-143">Delta</span><span class="sxs-lookup"><span data-stu-id="b9413-143">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="b9413-144">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="b9413-144">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="b9413-145">Получение добавочных изменений для **едукатионсчулс**</span><span class="sxs-lookup"><span data-stu-id="b9413-145">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="b9413-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9413-146">Properties</span></span>

| <span data-ttu-id="b9413-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9413-147">Property</span></span>            | <span data-ttu-id="b9413-148">Тип</span><span class="sxs-lookup"><span data-stu-id="b9413-148">Type</span></span>                                  | <span data-ttu-id="b9413-149">Описание</span><span class="sxs-lookup"><span data-stu-id="b9413-149">Description</span></span>                                        |
| :------------------ | :------------------------------------ | :------------------------------------------------- |
| <span data-ttu-id="b9413-150">id</span><span class="sxs-lookup"><span data-stu-id="b9413-150">id</span></span>                  | <span data-ttu-id="b9413-151">Строка</span><span class="sxs-lookup"><span data-stu-id="b9413-151">String</span></span>                                | <span data-ttu-id="b9413-152">GUID этого учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="b9413-152">GUID of this school.</span></span>                               |
| <span data-ttu-id="b9413-153">address</span><span class="sxs-lookup"><span data-stu-id="b9413-153">address</span></span>             | [<span data-ttu-id="b9413-154">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b9413-154">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="b9413-155">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="b9413-155">Address of the school.</span></span>                             |
| <span data-ttu-id="b9413-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="b9413-156">createdBy</span></span>           | [<span data-ttu-id="b9413-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="b9413-157">identitySet</span></span>](identityset.md)         | <span data-ttu-id="b9413-158">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="b9413-158">Entity who created the school.</span></span>                     |
| <span data-ttu-id="b9413-159">description</span><span class="sxs-lookup"><span data-stu-id="b9413-159">description</span></span>         | <span data-ttu-id="b9413-160">String</span><span class="sxs-lookup"><span data-stu-id="b9413-160">String</span></span>                                | <span data-ttu-id="b9413-161">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="b9413-161">Description of the school.</span></span>                         |
| <span data-ttu-id="b9413-162">displayName</span><span class="sxs-lookup"><span data-stu-id="b9413-162">displayName</span></span>         | <span data-ttu-id="b9413-163">Строка</span><span class="sxs-lookup"><span data-stu-id="b9413-163">String</span></span>                                | <span data-ttu-id="b9413-164">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="b9413-164">Display name of the school.</span></span>                        |
| <span data-ttu-id="b9413-165">externalId</span><span class="sxs-lookup"><span data-stu-id="b9413-165">externalId</span></span>          | <span data-ttu-id="b9413-166">String</span><span class="sxs-lookup"><span data-stu-id="b9413-166">String</span></span>                                | <span data-ttu-id="b9413-167">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b9413-167">ID of school in syncing system.</span></span>                    |
| <span data-ttu-id="b9413-168">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="b9413-168">externalPrincipalId</span></span> | <span data-ttu-id="b9413-169">String</span><span class="sxs-lookup"><span data-stu-id="b9413-169">String</span></span>                                | <span data-ttu-id="b9413-170">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b9413-170">ID of principal in syncing system.</span></span>                 |
| <span data-ttu-id="b9413-171">externalSource</span><span class="sxs-lookup"><span data-stu-id="b9413-171">externalSource</span></span>      | <span data-ttu-id="b9413-172">string</span><span class="sxs-lookup"><span data-stu-id="b9413-172">string</span></span>                                | <span data-ttu-id="b9413-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9413-173">Read-Only.</span></span> <span data-ttu-id="b9413-174">Возможные значения: `sis` или `manual`.</span><span class="sxs-lookup"><span data-stu-id="b9413-174">Possible values are: `sis` or `manual`.</span></span> |
| <span data-ttu-id="b9413-175">highestGrade</span><span class="sxs-lookup"><span data-stu-id="b9413-175">highestGrade</span></span>        | <span data-ttu-id="b9413-176">String</span><span class="sxs-lookup"><span data-stu-id="b9413-176">String</span></span>                                | <span data-ttu-id="b9413-177">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="b9413-177">Highest grade taught.</span></span>                              |
| <span data-ttu-id="b9413-178">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="b9413-178">lowestGrade</span></span>         | <span data-ttu-id="b9413-179">String</span><span class="sxs-lookup"><span data-stu-id="b9413-179">String</span></span>                                | <span data-ttu-id="b9413-180">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="b9413-180">Lowest grade taught.</span></span>                               |
| <span data-ttu-id="b9413-181">phone</span><span class="sxs-lookup"><span data-stu-id="b9413-181">phone</span></span>               | <span data-ttu-id="b9413-182">String</span><span class="sxs-lookup"><span data-stu-id="b9413-182">String</span></span>                                | <span data-ttu-id="b9413-183">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="b9413-183">Phone number of school.</span></span>                            |
| <span data-ttu-id="b9413-184">principalEmail</span><span class="sxs-lookup"><span data-stu-id="b9413-184">principalEmail</span></span>      | <span data-ttu-id="b9413-185">String</span><span class="sxs-lookup"><span data-stu-id="b9413-185">String</span></span>                                | <span data-ttu-id="b9413-186">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="b9413-186">Email address of the principal.</span></span>                    |
| <span data-ttu-id="b9413-187">principalName</span><span class="sxs-lookup"><span data-stu-id="b9413-187">principalName</span></span>       | <span data-ttu-id="b9413-188">String</span><span class="sxs-lookup"><span data-stu-id="b9413-188">String</span></span>                                | <span data-ttu-id="b9413-189">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="b9413-189">Name of the principal.</span></span>                             |
| <span data-ttu-id="b9413-190">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="b9413-190">schoolNumber</span></span>        | <span data-ttu-id="b9413-191">String</span><span class="sxs-lookup"><span data-stu-id="b9413-191">String</span></span>                                | <span data-ttu-id="b9413-192">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="b9413-192">School Number.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="b9413-193">Связи</span><span class="sxs-lookup"><span data-stu-id="b9413-193">Relationships</span></span>

| <span data-ttu-id="b9413-194">Связь</span><span class="sxs-lookup"><span data-stu-id="b9413-194">Relationship</span></span> | <span data-ttu-id="b9413-195">Тип</span><span class="sxs-lookup"><span data-stu-id="b9413-195">Type</span></span>                                           | <span data-ttu-id="b9413-196">Описание</span><span class="sxs-lookup"><span data-stu-id="b9413-196">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="b9413-197">classes</span><span class="sxs-lookup"><span data-stu-id="b9413-197">classes</span></span>      | <span data-ttu-id="b9413-198">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="b9413-198">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="b9413-199">Классы, которые обучаются в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="b9413-199">Classes taught at the school.</span></span> <span data-ttu-id="b9413-200">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b9413-200">Nullable.</span></span> |
| <span data-ttu-id="b9413-201">users</span><span class="sxs-lookup"><span data-stu-id="b9413-201">users</span></span>        | <span data-ttu-id="b9413-202">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="b9413-202">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="b9413-203">Пользователи в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="b9413-203">Users in the school.</span></span> <span data-ttu-id="b9413-204">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b9413-204">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="b9413-205">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9413-205">JSON representation</span></span>

<span data-ttu-id="b9413-206">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9413-206">The following is a JSON representation of the resource.</span></span>

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
