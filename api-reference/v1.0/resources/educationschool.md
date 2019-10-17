---
title: Тип ресурса educationSchool
description: 'Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d7cc20b01b35f678b20e18e21dcb099a89982ab9
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37553910"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="17be0-103">Тип ресурса educationSchool</span><span class="sxs-lookup"><span data-stu-id="17be0-103">educationSchool resource type</span></span>

<span data-ttu-id="17be0-104">Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="17be0-104">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  

## <a name="methods"></a><span data-ttu-id="17be0-105">Методы</span><span class="sxs-lookup"><span data-stu-id="17be0-105">Methods</span></span>

| <span data-ttu-id="17be0-106">Метод</span><span class="sxs-lookup"><span data-stu-id="17be0-106">Method</span></span>                                                   | <span data-ttu-id="17be0-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="17be0-107">Return Type</span></span>                                    | <span data-ttu-id="17be0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="17be0-108">Description</span></span>                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="17be0-109">Получение</span><span class="sxs-lookup"><span data-stu-id="17be0-109">Get</span></span>](../api/educationschool-get.md)                     | [<span data-ttu-id="17be0-110">educationSchool</span><span class="sxs-lookup"><span data-stu-id="17be0-110">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="17be0-111">Считывание свойств и отношений объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="17be0-111">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="17be0-112">Добавление класса</span><span class="sxs-lookup"><span data-stu-id="17be0-112">Add class</span></span>](../api/educationschool-post-classes.md)      | [<span data-ttu-id="17be0-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="17be0-113">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="17be0-114">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.</span><span class="sxs-lookup"><span data-stu-id="17be0-114">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="17be0-115">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="17be0-115">List classes</span></span>](../api/educationschool-list-classes.md)   | <span data-ttu-id="17be0-116">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="17be0-116">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="17be0-117">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="17be0-117">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="17be0-118">Удаление класса</span><span class="sxs-lookup"><span data-stu-id="17be0-118">Remove class</span></span>](../api/educationschool-delete-classes.md) | [<span data-ttu-id="17be0-119">educationClass</span><span class="sxs-lookup"><span data-stu-id="17be0-119">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="17be0-120">Удаление **educationClass** из учебного заведения через свойство навигации classes.</span><span class="sxs-lookup"><span data-stu-id="17be0-120">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="17be0-121">Добавление пользователя</span><span class="sxs-lookup"><span data-stu-id="17be0-121">Add user</span></span>](../api/educationschool-post-users.md)         | [<span data-ttu-id="17be0-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="17be0-122">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="17be0-123">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="17be0-123">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="17be0-124">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="17be0-124">List users</span></span>](../api/educationschool-list-users.md)       | <span data-ttu-id="17be0-125">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="17be0-125">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="17be0-126">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="17be0-126">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="17be0-127">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="17be0-127">Remove user</span></span>](../api/educationschool-delete-users.md)    | [<span data-ttu-id="17be0-128">educationUser</span><span class="sxs-lookup"><span data-stu-id="17be0-128">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="17be0-129">Удаление **educationUser** из учебного заведения через свойство навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="17be0-129">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="17be0-130">Обновление</span><span class="sxs-lookup"><span data-stu-id="17be0-130">Update</span></span>](../api/educationschool-update.md)               | [<span data-ttu-id="17be0-131">educationSchool</span><span class="sxs-lookup"><span data-stu-id="17be0-131">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="17be0-132">Обновление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="17be0-132">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="17be0-133">Удаление</span><span class="sxs-lookup"><span data-stu-id="17be0-133">Delete</span></span>](../api/educationschool-delete.md)               | <span data-ttu-id="17be0-134">Нет</span><span class="sxs-lookup"><span data-stu-id="17be0-134">None</span></span>                                           | <span data-ttu-id="17be0-135">Удаление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="17be0-135">Delete an **educationSchool** object.</span></span>                                                       |

## <a name="properties"></a><span data-ttu-id="17be0-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="17be0-136">Properties</span></span>

| <span data-ttu-id="17be0-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="17be0-137">Property</span></span>            | <span data-ttu-id="17be0-138">Тип</span><span class="sxs-lookup"><span data-stu-id="17be0-138">Type</span></span>                                  | <span data-ttu-id="17be0-139">Описание</span><span class="sxs-lookup"><span data-stu-id="17be0-139">Description</span></span>                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="17be0-140">id</span><span class="sxs-lookup"><span data-stu-id="17be0-140">id</span></span>                  | <span data-ttu-id="17be0-141">String</span><span class="sxs-lookup"><span data-stu-id="17be0-141">String</span></span>                                | <span data-ttu-id="17be0-142">GUID этого учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="17be0-142">GUID of this school.</span></span>                                                               |
| <span data-ttu-id="17be0-143">displayName</span><span class="sxs-lookup"><span data-stu-id="17be0-143">displayName</span></span>         | <span data-ttu-id="17be0-144">Строка</span><span class="sxs-lookup"><span data-stu-id="17be0-144">String</span></span>                                | <span data-ttu-id="17be0-145">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="17be0-145">Display name of the school.</span></span>                                                        |
| <span data-ttu-id="17be0-146">description</span><span class="sxs-lookup"><span data-stu-id="17be0-146">description</span></span>         | <span data-ttu-id="17be0-147">Строка</span><span class="sxs-lookup"><span data-stu-id="17be0-147">String</span></span>                                | <span data-ttu-id="17be0-148">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="17be0-148">Description of the school.</span></span>                                                         |
| <span data-ttu-id="17be0-149">status</span><span class="sxs-lookup"><span data-stu-id="17be0-149">status</span></span>              | <span data-ttu-id="17be0-150">string</span><span class="sxs-lookup"><span data-stu-id="17be0-150">string</span></span>                                | <span data-ttu-id="17be0-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17be0-151">Read-Only.</span></span> <span data-ttu-id="17be0-152">Допустимые значения: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="17be0-152">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span> |
| <span data-ttu-id="17be0-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="17be0-153">externalSource</span></span>      | <span data-ttu-id="17be0-154">едукатионекстерналсаурце</span><span class="sxs-lookup"><span data-stu-id="17be0-154">educationExternalSource</span></span>               | <span data-ttu-id="17be0-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17be0-155">Read-Only.</span></span>  <span data-ttu-id="17be0-156">Допустимые значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="17be0-156">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>        |
| <span data-ttu-id="17be0-157">principalEmail</span><span class="sxs-lookup"><span data-stu-id="17be0-157">principalEmail</span></span>      | <span data-ttu-id="17be0-158">String</span><span class="sxs-lookup"><span data-stu-id="17be0-158">String</span></span>                                | <span data-ttu-id="17be0-159">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="17be0-159">Email address of the principal.</span></span>                                                    |
| <span data-ttu-id="17be0-160">principalName</span><span class="sxs-lookup"><span data-stu-id="17be0-160">principalName</span></span>       | <span data-ttu-id="17be0-161">String</span><span class="sxs-lookup"><span data-stu-id="17be0-161">String</span></span>                                | <span data-ttu-id="17be0-162">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="17be0-162">Name of the principal.</span></span>                                                             |
| <span data-ttu-id="17be0-163">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="17be0-163">externalPrincipalId</span></span> | <span data-ttu-id="17be0-164">String</span><span class="sxs-lookup"><span data-stu-id="17be0-164">String</span></span>                                | <span data-ttu-id="17be0-165">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="17be0-165">ID of principal in syncing system.</span></span>                                                 |
| <span data-ttu-id="17be0-166">highestGrade</span><span class="sxs-lookup"><span data-stu-id="17be0-166">highestGrade</span></span>        | <span data-ttu-id="17be0-167">String</span><span class="sxs-lookup"><span data-stu-id="17be0-167">String</span></span>                                | <span data-ttu-id="17be0-168">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="17be0-168">Highest grade taught.</span></span>                                                              |
| <span data-ttu-id="17be0-169">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="17be0-169">lowestGrade</span></span>         | <span data-ttu-id="17be0-170">String</span><span class="sxs-lookup"><span data-stu-id="17be0-170">String</span></span>                                | <span data-ttu-id="17be0-171">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="17be0-171">Lowest grade taught.</span></span>                                                               |
| <span data-ttu-id="17be0-172">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="17be0-172">schoolNumber</span></span>        | <span data-ttu-id="17be0-173">String</span><span class="sxs-lookup"><span data-stu-id="17be0-173">String</span></span>                                | <span data-ttu-id="17be0-174">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="17be0-174">School Number.</span></span>                                                                     |
| <span data-ttu-id="17be0-175">externalId</span><span class="sxs-lookup"><span data-stu-id="17be0-175">externalId</span></span>          | <span data-ttu-id="17be0-176">String</span><span class="sxs-lookup"><span data-stu-id="17be0-176">String</span></span>                                | <span data-ttu-id="17be0-177">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="17be0-177">ID of school in syncing system.</span></span>                                                    |
| <span data-ttu-id="17be0-178">phone</span><span class="sxs-lookup"><span data-stu-id="17be0-178">phone</span></span>               | <span data-ttu-id="17be0-179">String</span><span class="sxs-lookup"><span data-stu-id="17be0-179">String</span></span>                                | <span data-ttu-id="17be0-180">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="17be0-180">Phone number of school.</span></span>                                                            |
| <span data-ttu-id="17be0-181">address</span><span class="sxs-lookup"><span data-stu-id="17be0-181">address</span></span>             | [<span data-ttu-id="17be0-182">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="17be0-182">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="17be0-183">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="17be0-183">Address of the school.</span></span>                                                             |
| <span data-ttu-id="17be0-184">createdBy</span><span class="sxs-lookup"><span data-stu-id="17be0-184">createdBy</span></span>           | [<span data-ttu-id="17be0-185">identitySet</span><span class="sxs-lookup"><span data-stu-id="17be0-185">identitySet</span></span>](identityset.md)         | <span data-ttu-id="17be0-186">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="17be0-186">Entity who created the school.</span></span>                                                     |

## <a name="relationships"></a><span data-ttu-id="17be0-187">Связи</span><span class="sxs-lookup"><span data-stu-id="17be0-187">Relationships</span></span>

| <span data-ttu-id="17be0-188">Связь</span><span class="sxs-lookup"><span data-stu-id="17be0-188">Relationship</span></span> | <span data-ttu-id="17be0-189">Тип</span><span class="sxs-lookup"><span data-stu-id="17be0-189">Type</span></span>                                           | <span data-ttu-id="17be0-190">Описание</span><span class="sxs-lookup"><span data-stu-id="17be0-190">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="17be0-191">classes</span><span class="sxs-lookup"><span data-stu-id="17be0-191">classes</span></span>      | <span data-ttu-id="17be0-192">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="17be0-192">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="17be0-193">Классы, которые обучаются в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="17be0-193">Classes taught at the school.</span></span> <span data-ttu-id="17be0-194">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="17be0-194">Nullable.</span></span> |
| <span data-ttu-id="17be0-195">users</span><span class="sxs-lookup"><span data-stu-id="17be0-195">users</span></span>        | <span data-ttu-id="17be0-196">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="17be0-196">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="17be0-197">Пользователи в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="17be0-197">Users in the school.</span></span> <span data-ttu-id="17be0-198">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="17be0-198">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="17be0-199">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17be0-199">JSON representation</span></span>

<span data-ttu-id="17be0-200">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17be0-200">The following is a JSON representation of the resource.</span></span>

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
