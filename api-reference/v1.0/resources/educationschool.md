---
title: Тип ресурса educationSchool
description: 'Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 407f29c7d8f9468c5e9b1da1badad294cb655121
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531510"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="9e661-103">Тип ресурса educationSchool</span><span class="sxs-lookup"><span data-stu-id="9e661-103">educationSchool resource type</span></span>

<span data-ttu-id="9e661-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e661-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e661-105">Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="9e661-105">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  

## <a name="methods"></a><span data-ttu-id="9e661-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9e661-106">Methods</span></span>

| <span data-ttu-id="9e661-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9e661-107">Method</span></span>                                                   | <span data-ttu-id="9e661-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9e661-108">Return Type</span></span>                                    | <span data-ttu-id="9e661-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9e661-109">Description</span></span>                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="9e661-110">[получение](../api/educationschool-get.md);</span><span class="sxs-lookup"><span data-stu-id="9e661-110">[Get](../api/educationschool-get.md)</span></span>                     | [<span data-ttu-id="9e661-111">educationSchool</span><span class="sxs-lookup"><span data-stu-id="9e661-111">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="9e661-112">Считывание свойств и отношений объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="9e661-112">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="9e661-113">Добавление класса</span><span class="sxs-lookup"><span data-stu-id="9e661-113">Add class</span></span>](../api/educationschool-post-classes.md)      | [<span data-ttu-id="9e661-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="9e661-114">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="9e661-115">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.</span><span class="sxs-lookup"><span data-stu-id="9e661-115">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="9e661-116">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="9e661-116">List classes</span></span>](../api/educationschool-list-classes.md)   | <span data-ttu-id="9e661-117">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="9e661-117">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="9e661-118">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="9e661-118">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="9e661-119">Удаление класса</span><span class="sxs-lookup"><span data-stu-id="9e661-119">Remove class</span></span>](../api/educationschool-delete-classes.md) | [<span data-ttu-id="9e661-120">educationClass</span><span class="sxs-lookup"><span data-stu-id="9e661-120">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="9e661-121">Удаление **educationClass** из учебного заведения через свойство навигации classes.</span><span class="sxs-lookup"><span data-stu-id="9e661-121">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="9e661-122">Добавление пользователя</span><span class="sxs-lookup"><span data-stu-id="9e661-122">Add user</span></span>](../api/educationschool-post-users.md)         | [<span data-ttu-id="9e661-123">educationUser</span><span class="sxs-lookup"><span data-stu-id="9e661-123">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="9e661-124">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="9e661-124">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="9e661-125">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="9e661-125">List users</span></span>](../api/educationschool-list-users.md)       | <span data-ttu-id="9e661-126">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="9e661-126">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="9e661-127">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="9e661-127">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="9e661-128">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="9e661-128">Remove user</span></span>](../api/educationschool-delete-users.md)    | [<span data-ttu-id="9e661-129">educationUser</span><span class="sxs-lookup"><span data-stu-id="9e661-129">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="9e661-130">Удаление **educationUser** из учебного заведения через свойство навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="9e661-130">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="9e661-131">Обновление</span><span class="sxs-lookup"><span data-stu-id="9e661-131">Update</span></span>](../api/educationschool-update.md)               | [<span data-ttu-id="9e661-132">educationSchool</span><span class="sxs-lookup"><span data-stu-id="9e661-132">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="9e661-133">Обновление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="9e661-133">Update an **educationSchool** object.</span></span>                                                       |
| <span data-ttu-id="9e661-134">[удаление](../api/educationschool-delete.md);</span><span class="sxs-lookup"><span data-stu-id="9e661-134">[Delete](../api/educationschool-delete.md)</span></span>               | <span data-ttu-id="9e661-135">Нет</span><span class="sxs-lookup"><span data-stu-id="9e661-135">None</span></span>                                           | <span data-ttu-id="9e661-136">Удаление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="9e661-136">Delete an **educationSchool** object.</span></span>                                                       |

## <a name="properties"></a><span data-ttu-id="9e661-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e661-137">Properties</span></span>

| <span data-ttu-id="9e661-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e661-138">Property</span></span>            | <span data-ttu-id="9e661-139">Тип</span><span class="sxs-lookup"><span data-stu-id="9e661-139">Type</span></span>                                  | <span data-ttu-id="9e661-140">Описание</span><span class="sxs-lookup"><span data-stu-id="9e661-140">Description</span></span>                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="9e661-141">id</span><span class="sxs-lookup"><span data-stu-id="9e661-141">id</span></span>                  | <span data-ttu-id="9e661-142">String</span><span class="sxs-lookup"><span data-stu-id="9e661-142">String</span></span>                                | <span data-ttu-id="9e661-143">GUID этого учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="9e661-143">GUID of this school.</span></span>                                                               |
| <span data-ttu-id="9e661-144">displayName</span><span class="sxs-lookup"><span data-stu-id="9e661-144">displayName</span></span>         | <span data-ttu-id="9e661-145">Строка</span><span class="sxs-lookup"><span data-stu-id="9e661-145">String</span></span>                                | <span data-ttu-id="9e661-146">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="9e661-146">Display name of the school.</span></span>                                                        |
| <span data-ttu-id="9e661-147">description</span><span class="sxs-lookup"><span data-stu-id="9e661-147">description</span></span>         | <span data-ttu-id="9e661-148">Строка</span><span class="sxs-lookup"><span data-stu-id="9e661-148">String</span></span>                                | <span data-ttu-id="9e661-149">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="9e661-149">Description of the school.</span></span>                                                         |
| <span data-ttu-id="9e661-150">status</span><span class="sxs-lookup"><span data-stu-id="9e661-150">status</span></span>              | <span data-ttu-id="9e661-151">string</span><span class="sxs-lookup"><span data-stu-id="9e661-151">string</span></span>                                | <span data-ttu-id="9e661-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e661-152">Read-Only.</span></span> <span data-ttu-id="9e661-153">Допустимые значения: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="9e661-153">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span> |
| <span data-ttu-id="9e661-154">externalSource</span><span class="sxs-lookup"><span data-stu-id="9e661-154">externalSource</span></span>      | <span data-ttu-id="9e661-155">едукатионекстерналсаурце</span><span class="sxs-lookup"><span data-stu-id="9e661-155">educationExternalSource</span></span>               | <span data-ttu-id="9e661-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e661-156">Read-Only.</span></span>  <span data-ttu-id="9e661-157">Допустимые значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9e661-157">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>        |
| <span data-ttu-id="9e661-158">principalEmail</span><span class="sxs-lookup"><span data-stu-id="9e661-158">principalEmail</span></span>      | <span data-ttu-id="9e661-159">String</span><span class="sxs-lookup"><span data-stu-id="9e661-159">String</span></span>                                | <span data-ttu-id="9e661-160">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="9e661-160">Email address of the principal.</span></span>                                                    |
| <span data-ttu-id="9e661-161">principalName</span><span class="sxs-lookup"><span data-stu-id="9e661-161">principalName</span></span>       | <span data-ttu-id="9e661-162">String</span><span class="sxs-lookup"><span data-stu-id="9e661-162">String</span></span>                                | <span data-ttu-id="9e661-163">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="9e661-163">Name of the principal.</span></span>                                                             |
| <span data-ttu-id="9e661-164">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="9e661-164">externalPrincipalId</span></span> | <span data-ttu-id="9e661-165">String</span><span class="sxs-lookup"><span data-stu-id="9e661-165">String</span></span>                                | <span data-ttu-id="9e661-166">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="9e661-166">ID of principal in syncing system.</span></span>                                                 |
| <span data-ttu-id="9e661-167">highestGrade</span><span class="sxs-lookup"><span data-stu-id="9e661-167">highestGrade</span></span>        | <span data-ttu-id="9e661-168">String</span><span class="sxs-lookup"><span data-stu-id="9e661-168">String</span></span>                                | <span data-ttu-id="9e661-169">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="9e661-169">Highest grade taught.</span></span>                                                              |
| <span data-ttu-id="9e661-170">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="9e661-170">lowestGrade</span></span>         | <span data-ttu-id="9e661-171">String</span><span class="sxs-lookup"><span data-stu-id="9e661-171">String</span></span>                                | <span data-ttu-id="9e661-172">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="9e661-172">Lowest grade taught.</span></span>                                                               |
| <span data-ttu-id="9e661-173">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="9e661-173">schoolNumber</span></span>        | <span data-ttu-id="9e661-174">String</span><span class="sxs-lookup"><span data-stu-id="9e661-174">String</span></span>                                | <span data-ttu-id="9e661-175">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="9e661-175">School Number.</span></span>                                                                     |
| <span data-ttu-id="9e661-176">externalId</span><span class="sxs-lookup"><span data-stu-id="9e661-176">externalId</span></span>          | <span data-ttu-id="9e661-177">String</span><span class="sxs-lookup"><span data-stu-id="9e661-177">String</span></span>                                | <span data-ttu-id="9e661-178">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="9e661-178">ID of school in syncing system.</span></span>                                                    |
| <span data-ttu-id="9e661-179">phone</span><span class="sxs-lookup"><span data-stu-id="9e661-179">phone</span></span>               | <span data-ttu-id="9e661-180">String</span><span class="sxs-lookup"><span data-stu-id="9e661-180">String</span></span>                                | <span data-ttu-id="9e661-181">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="9e661-181">Phone number of school.</span></span>                                                            |
| <span data-ttu-id="9e661-182">address</span><span class="sxs-lookup"><span data-stu-id="9e661-182">address</span></span>             | [<span data-ttu-id="9e661-183">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="9e661-183">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="9e661-184">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="9e661-184">Address of the school.</span></span>                                                             |
| <span data-ttu-id="9e661-185">createdBy</span><span class="sxs-lookup"><span data-stu-id="9e661-185">createdBy</span></span>           | [<span data-ttu-id="9e661-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="9e661-186">identitySet</span></span>](identityset.md)         | <span data-ttu-id="9e661-187">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="9e661-187">Entity who created the school.</span></span>                                                     |

## <a name="relationships"></a><span data-ttu-id="9e661-188">Связи</span><span class="sxs-lookup"><span data-stu-id="9e661-188">Relationships</span></span>

| <span data-ttu-id="9e661-189">Связь</span><span class="sxs-lookup"><span data-stu-id="9e661-189">Relationship</span></span> | <span data-ttu-id="9e661-190">Тип</span><span class="sxs-lookup"><span data-stu-id="9e661-190">Type</span></span>                                           | <span data-ttu-id="9e661-191">Описание</span><span class="sxs-lookup"><span data-stu-id="9e661-191">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="9e661-192">classes</span><span class="sxs-lookup"><span data-stu-id="9e661-192">classes</span></span>      | <span data-ttu-id="9e661-193">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="9e661-193">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="9e661-194">Классы, которые обучаются в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="9e661-194">Classes taught at the school.</span></span> <span data-ttu-id="9e661-195">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9e661-195">Nullable.</span></span> |
| <span data-ttu-id="9e661-196">users</span><span class="sxs-lookup"><span data-stu-id="9e661-196">users</span></span>        | <span data-ttu-id="9e661-197">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="9e661-197">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="9e661-198">Пользователи в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="9e661-198">Users in the school.</span></span> <span data-ttu-id="9e661-199">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9e661-199">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="9e661-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e661-200">JSON representation</span></span>

<span data-ttu-id="9e661-201">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e661-201">The following is a JSON representation of the resource.</span></span>

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
