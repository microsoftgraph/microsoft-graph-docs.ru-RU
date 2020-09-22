---
title: Тип ресурса educationSchool
description: 'Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2ed10fd9be0a49fbf25acac635cf29b1759c31eb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032658"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="1fa75-103">Тип ресурса educationSchool</span><span class="sxs-lookup"><span data-stu-id="1fa75-103">educationSchool resource type</span></span>

<span data-ttu-id="1fa75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fa75-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1fa75-105">Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="1fa75-105">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  

## <a name="methods"></a><span data-ttu-id="1fa75-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1fa75-106">Methods</span></span>

| <span data-ttu-id="1fa75-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1fa75-107">Method</span></span>                                                   | <span data-ttu-id="1fa75-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1fa75-108">Return Type</span></span>                                    | <span data-ttu-id="1fa75-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1fa75-109">Description</span></span>                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="1fa75-110">[получение](../api/educationschool-get.md);</span><span class="sxs-lookup"><span data-stu-id="1fa75-110">[Get](../api/educationschool-get.md)</span></span>                     | [<span data-ttu-id="1fa75-111">educationSchool</span><span class="sxs-lookup"><span data-stu-id="1fa75-111">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="1fa75-112">Считывание свойств и отношений объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="1fa75-112">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="1fa75-113">Добавление класса</span><span class="sxs-lookup"><span data-stu-id="1fa75-113">Add class</span></span>](../api/educationschool-post-classes.md)      | [<span data-ttu-id="1fa75-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="1fa75-114">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="1fa75-115">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.</span><span class="sxs-lookup"><span data-stu-id="1fa75-115">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="1fa75-116">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="1fa75-116">List classes</span></span>](../api/educationschool-list-classes.md)   | <span data-ttu-id="1fa75-117">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="1fa75-117">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="1fa75-118">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="1fa75-118">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="1fa75-119">Удаление класса</span><span class="sxs-lookup"><span data-stu-id="1fa75-119">Remove class</span></span>](../api/educationschool-delete-classes.md) | [<span data-ttu-id="1fa75-120">educationClass</span><span class="sxs-lookup"><span data-stu-id="1fa75-120">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="1fa75-121">Удаление **educationClass** из учебного заведения через свойство навигации classes.</span><span class="sxs-lookup"><span data-stu-id="1fa75-121">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="1fa75-122">Добавление пользователя</span><span class="sxs-lookup"><span data-stu-id="1fa75-122">Add user</span></span>](../api/educationschool-post-users.md)         | [<span data-ttu-id="1fa75-123">educationUser</span><span class="sxs-lookup"><span data-stu-id="1fa75-123">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="1fa75-124">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="1fa75-124">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="1fa75-125">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="1fa75-125">List users</span></span>](../api/educationschool-list-users.md)       | <span data-ttu-id="1fa75-126">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="1fa75-126">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="1fa75-127">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="1fa75-127">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="1fa75-128">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="1fa75-128">Remove user</span></span>](../api/educationschool-delete-users.md)    | [<span data-ttu-id="1fa75-129">educationUser</span><span class="sxs-lookup"><span data-stu-id="1fa75-129">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="1fa75-130">Удаление **educationUser** из учебного заведения через свойство навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="1fa75-130">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="1fa75-131">Обновление</span><span class="sxs-lookup"><span data-stu-id="1fa75-131">Update</span></span>](../api/educationschool-update.md)               | [<span data-ttu-id="1fa75-132">educationSchool</span><span class="sxs-lookup"><span data-stu-id="1fa75-132">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="1fa75-133">Обновление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="1fa75-133">Update an **educationSchool** object.</span></span>                                                       |
| <span data-ttu-id="1fa75-134">[удаление](../api/educationschool-delete.md);</span><span class="sxs-lookup"><span data-stu-id="1fa75-134">[Delete](../api/educationschool-delete.md)</span></span>               | <span data-ttu-id="1fa75-135">Нет</span><span class="sxs-lookup"><span data-stu-id="1fa75-135">None</span></span>                                           | <span data-ttu-id="1fa75-136">Удаление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="1fa75-136">Delete an **educationSchool** object.</span></span>                                                       |

## <a name="properties"></a><span data-ttu-id="1fa75-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="1fa75-137">Properties</span></span>

| <span data-ttu-id="1fa75-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fa75-138">Property</span></span>            | <span data-ttu-id="1fa75-139">Тип</span><span class="sxs-lookup"><span data-stu-id="1fa75-139">Type</span></span>                                  | <span data-ttu-id="1fa75-140">Описание</span><span class="sxs-lookup"><span data-stu-id="1fa75-140">Description</span></span>                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="1fa75-141">id</span><span class="sxs-lookup"><span data-stu-id="1fa75-141">id</span></span>                  | <span data-ttu-id="1fa75-142">String</span><span class="sxs-lookup"><span data-stu-id="1fa75-142">String</span></span>                                | <span data-ttu-id="1fa75-143">GUID этого учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="1fa75-143">GUID of this school.</span></span>                                                               |
| <span data-ttu-id="1fa75-144">displayName</span><span class="sxs-lookup"><span data-stu-id="1fa75-144">displayName</span></span>         | <span data-ttu-id="1fa75-145">String</span><span class="sxs-lookup"><span data-stu-id="1fa75-145">String</span></span>                                | <span data-ttu-id="1fa75-146">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="1fa75-146">Display name of the school.</span></span>                                                        |
| <span data-ttu-id="1fa75-147">description</span><span class="sxs-lookup"><span data-stu-id="1fa75-147">description</span></span>         | <span data-ttu-id="1fa75-148">String</span><span class="sxs-lookup"><span data-stu-id="1fa75-148">String</span></span>                                | <span data-ttu-id="1fa75-149">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="1fa75-149">Description of the school.</span></span>                                                         |
| <span data-ttu-id="1fa75-150">status</span><span class="sxs-lookup"><span data-stu-id="1fa75-150">status</span></span>              | <span data-ttu-id="1fa75-151">string</span><span class="sxs-lookup"><span data-stu-id="1fa75-151">string</span></span>                                | <span data-ttu-id="1fa75-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1fa75-152">Read-Only.</span></span> <span data-ttu-id="1fa75-153">Допустимые значения: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="1fa75-153">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span> |
| <span data-ttu-id="1fa75-154">externalSource</span><span class="sxs-lookup"><span data-stu-id="1fa75-154">externalSource</span></span>      | <span data-ttu-id="1fa75-155">едукатионекстерналсаурце</span><span class="sxs-lookup"><span data-stu-id="1fa75-155">educationExternalSource</span></span>               | <span data-ttu-id="1fa75-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1fa75-156">Read-Only.</span></span>  <span data-ttu-id="1fa75-157">Допустимые значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1fa75-157">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>        |
| <span data-ttu-id="1fa75-158">principalEmail</span><span class="sxs-lookup"><span data-stu-id="1fa75-158">principalEmail</span></span>      | <span data-ttu-id="1fa75-159">String</span><span class="sxs-lookup"><span data-stu-id="1fa75-159">String</span></span>                                | <span data-ttu-id="1fa75-160">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="1fa75-160">Email address of the principal.</span></span>                                                    |
| <span data-ttu-id="1fa75-161">principalName</span><span class="sxs-lookup"><span data-stu-id="1fa75-161">principalName</span></span>       | <span data-ttu-id="1fa75-162">String</span><span class="sxs-lookup"><span data-stu-id="1fa75-162">String</span></span>                                | <span data-ttu-id="1fa75-163">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="1fa75-163">Name of the principal.</span></span>                                                             |
| <span data-ttu-id="1fa75-164">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="1fa75-164">externalPrincipalId</span></span> | <span data-ttu-id="1fa75-165">String</span><span class="sxs-lookup"><span data-stu-id="1fa75-165">String</span></span>                                | <span data-ttu-id="1fa75-166">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="1fa75-166">ID of principal in syncing system.</span></span>                                                 |
| <span data-ttu-id="1fa75-167">highestGrade</span><span class="sxs-lookup"><span data-stu-id="1fa75-167">highestGrade</span></span>        | <span data-ttu-id="1fa75-168">String</span><span class="sxs-lookup"><span data-stu-id="1fa75-168">String</span></span>                                | <span data-ttu-id="1fa75-169">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="1fa75-169">Highest grade taught.</span></span>                                                              |
| <span data-ttu-id="1fa75-170">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="1fa75-170">lowestGrade</span></span>         | <span data-ttu-id="1fa75-171">String</span><span class="sxs-lookup"><span data-stu-id="1fa75-171">String</span></span>                                | <span data-ttu-id="1fa75-172">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="1fa75-172">Lowest grade taught.</span></span>                                                               |
| <span data-ttu-id="1fa75-173">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="1fa75-173">schoolNumber</span></span>        | <span data-ttu-id="1fa75-174">String</span><span class="sxs-lookup"><span data-stu-id="1fa75-174">String</span></span>                                | <span data-ttu-id="1fa75-175">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="1fa75-175">School Number.</span></span>                                                                     |
| <span data-ttu-id="1fa75-176">externalId</span><span class="sxs-lookup"><span data-stu-id="1fa75-176">externalId</span></span>          | <span data-ttu-id="1fa75-177">String</span><span class="sxs-lookup"><span data-stu-id="1fa75-177">String</span></span>                                | <span data-ttu-id="1fa75-178">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="1fa75-178">ID of school in syncing system.</span></span>                                                    |
| <span data-ttu-id="1fa75-179">phone</span><span class="sxs-lookup"><span data-stu-id="1fa75-179">phone</span></span>               | <span data-ttu-id="1fa75-180">String</span><span class="sxs-lookup"><span data-stu-id="1fa75-180">String</span></span>                                | <span data-ttu-id="1fa75-181">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="1fa75-181">Phone number of school.</span></span>                                                            |
| <span data-ttu-id="1fa75-182">address</span><span class="sxs-lookup"><span data-stu-id="1fa75-182">address</span></span>             | [<span data-ttu-id="1fa75-183">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="1fa75-183">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="1fa75-184">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="1fa75-184">Address of the school.</span></span>                                                             |
| <span data-ttu-id="1fa75-185">createdBy</span><span class="sxs-lookup"><span data-stu-id="1fa75-185">createdBy</span></span>           | [<span data-ttu-id="1fa75-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="1fa75-186">identitySet</span></span>](identityset.md)         | <span data-ttu-id="1fa75-187">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="1fa75-187">Entity who created the school.</span></span>                                                     |

## <a name="relationships"></a><span data-ttu-id="1fa75-188">Связи</span><span class="sxs-lookup"><span data-stu-id="1fa75-188">Relationships</span></span>

| <span data-ttu-id="1fa75-189">Связь</span><span class="sxs-lookup"><span data-stu-id="1fa75-189">Relationship</span></span> | <span data-ttu-id="1fa75-190">Тип</span><span class="sxs-lookup"><span data-stu-id="1fa75-190">Type</span></span>                                           | <span data-ttu-id="1fa75-191">Описание</span><span class="sxs-lookup"><span data-stu-id="1fa75-191">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="1fa75-192">classes</span><span class="sxs-lookup"><span data-stu-id="1fa75-192">classes</span></span>      | <span data-ttu-id="1fa75-193">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="1fa75-193">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="1fa75-194">Классы, которые обучаются в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="1fa75-194">Classes taught at the school.</span></span> <span data-ttu-id="1fa75-195">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1fa75-195">Nullable.</span></span> |
| <span data-ttu-id="1fa75-196">users</span><span class="sxs-lookup"><span data-stu-id="1fa75-196">users</span></span>        | <span data-ttu-id="1fa75-197">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="1fa75-197">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="1fa75-198">Пользователи в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="1fa75-198">Users in the school.</span></span> <span data-ttu-id="1fa75-199">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1fa75-199">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="1fa75-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1fa75-200">JSON representation</span></span>

<span data-ttu-id="1fa75-201">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1fa75-201">The following is a JSON representation of the resource.</span></span>

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

