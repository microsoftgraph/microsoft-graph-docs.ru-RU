---
title: Тип ресурса educationSchool
description: 'Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: bd25283390e2683affe2e2cb636344c60a772a2e
ms.sourcegitcommit: 6714f71e0d229f1ab56150a9976b5106b4c8b785
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2020
ms.locfileid: "49368168"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="42282-103">Тип ресурса educationSchool</span><span class="sxs-lookup"><span data-stu-id="42282-103">educationSchool resource type</span></span>

<span data-ttu-id="42282-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42282-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="42282-105">Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="42282-105">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  

## <a name="methods"></a><span data-ttu-id="42282-106">Методы</span><span class="sxs-lookup"><span data-stu-id="42282-106">Methods</span></span>

| <span data-ttu-id="42282-107">Метод</span><span class="sxs-lookup"><span data-stu-id="42282-107">Method</span></span>                                                   | <span data-ttu-id="42282-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="42282-108">Return Type</span></span>                                    | <span data-ttu-id="42282-109">Описание</span><span class="sxs-lookup"><span data-stu-id="42282-109">Description</span></span>                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="42282-110">[получение](../api/educationschool-get.md);</span><span class="sxs-lookup"><span data-stu-id="42282-110">[Get](../api/educationschool-get.md)</span></span>                     | [<span data-ttu-id="42282-111">educationSchool</span><span class="sxs-lookup"><span data-stu-id="42282-111">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="42282-112">Считывание свойств и отношений объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="42282-112">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="42282-113">Добавление класса</span><span class="sxs-lookup"><span data-stu-id="42282-113">Add class</span></span>](../api/educationschool-post-classes.md)      | [<span data-ttu-id="42282-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="42282-114">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="42282-115">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.</span><span class="sxs-lookup"><span data-stu-id="42282-115">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="42282-116">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="42282-116">List classes</span></span>](../api/educationschool-list-classes.md)   | <span data-ttu-id="42282-117">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="42282-117">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="42282-118">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="42282-118">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="42282-119">Удаление класса</span><span class="sxs-lookup"><span data-stu-id="42282-119">Remove class</span></span>](../api/educationschool-delete-classes.md) | [<span data-ttu-id="42282-120">educationClass</span><span class="sxs-lookup"><span data-stu-id="42282-120">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="42282-121">Удаление **educationClass** из учебного заведения через свойство навигации classes.</span><span class="sxs-lookup"><span data-stu-id="42282-121">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="42282-122">Добавление пользователя</span><span class="sxs-lookup"><span data-stu-id="42282-122">Add user</span></span>](../api/educationschool-post-users.md)         | [<span data-ttu-id="42282-123">educationUser</span><span class="sxs-lookup"><span data-stu-id="42282-123">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="42282-124">Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="42282-124">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="42282-125">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="42282-125">List users</span></span>](../api/educationschool-list-users.md)       | <span data-ttu-id="42282-126">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="42282-126">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="42282-127">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="42282-127">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="42282-128">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="42282-128">Remove user</span></span>](../api/educationschool-delete-users.md)    | [<span data-ttu-id="42282-129">educationUser</span><span class="sxs-lookup"><span data-stu-id="42282-129">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="42282-130">Удаление **educationUser** из учебного заведения через свойство навигации **users**.</span><span class="sxs-lookup"><span data-stu-id="42282-130">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="42282-131">Обновление</span><span class="sxs-lookup"><span data-stu-id="42282-131">Update</span></span>](../api/educationschool-update.md)               | [<span data-ttu-id="42282-132">educationSchool</span><span class="sxs-lookup"><span data-stu-id="42282-132">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="42282-133">Обновление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="42282-133">Update an **educationSchool** object.</span></span>                                                       |
| <span data-ttu-id="42282-134">[удаление](../api/educationschool-delete.md);</span><span class="sxs-lookup"><span data-stu-id="42282-134">[Delete](../api/educationschool-delete.md)</span></span>               | <span data-ttu-id="42282-135">Нет</span><span class="sxs-lookup"><span data-stu-id="42282-135">None</span></span>                                           | <span data-ttu-id="42282-136">Удаление объекта **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="42282-136">Delete an **educationSchool** object.</span></span>                                                       |

## <a name="properties"></a><span data-ttu-id="42282-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="42282-137">Properties</span></span>

| <span data-ttu-id="42282-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="42282-138">Property</span></span>            | <span data-ttu-id="42282-139">Тип</span><span class="sxs-lookup"><span data-stu-id="42282-139">Type</span></span>                                  | <span data-ttu-id="42282-140">Описание</span><span class="sxs-lookup"><span data-stu-id="42282-140">Description</span></span>                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="42282-141">id</span><span class="sxs-lookup"><span data-stu-id="42282-141">id</span></span>                  | <span data-ttu-id="42282-142">Строка</span><span class="sxs-lookup"><span data-stu-id="42282-142">String</span></span>                                | <span data-ttu-id="42282-143">GUID этого учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="42282-143">GUID of this school.</span></span>                                                               |
| <span data-ttu-id="42282-144">displayName</span><span class="sxs-lookup"><span data-stu-id="42282-144">displayName</span></span>         | <span data-ttu-id="42282-145">Строка</span><span class="sxs-lookup"><span data-stu-id="42282-145">String</span></span>                                | <span data-ttu-id="42282-146">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="42282-146">Display name of the school.</span></span>                                                        |
| <span data-ttu-id="42282-147">description</span><span class="sxs-lookup"><span data-stu-id="42282-147">description</span></span>         | <span data-ttu-id="42282-148">Строка</span><span class="sxs-lookup"><span data-stu-id="42282-148">String</span></span>                                | <span data-ttu-id="42282-149">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="42282-149">Description of the school.</span></span>                                                         |
| <span data-ttu-id="42282-150">status</span><span class="sxs-lookup"><span data-stu-id="42282-150">status</span></span>              | <span data-ttu-id="42282-151">string</span><span class="sxs-lookup"><span data-stu-id="42282-151">string</span></span>                                | <span data-ttu-id="42282-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42282-152">Read-Only.</span></span> <span data-ttu-id="42282-153">Допустимые значения: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="42282-153">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span> |
| <span data-ttu-id="42282-154">externalSource</span><span class="sxs-lookup"><span data-stu-id="42282-154">externalSource</span></span>      | <span data-ttu-id="42282-155">едукатионекстерналсаурце</span><span class="sxs-lookup"><span data-stu-id="42282-155">educationExternalSource</span></span>               | <span data-ttu-id="42282-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42282-156">Read-Only.</span></span>  <span data-ttu-id="42282-157">Допустимые значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="42282-157">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>        |
| <span data-ttu-id="42282-158">principalEmail</span><span class="sxs-lookup"><span data-stu-id="42282-158">principalEmail</span></span>      | <span data-ttu-id="42282-159">String</span><span class="sxs-lookup"><span data-stu-id="42282-159">String</span></span>                                | <span data-ttu-id="42282-160">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="42282-160">Email address of the principal.</span></span>                                                    |
| <span data-ttu-id="42282-161">principalName</span><span class="sxs-lookup"><span data-stu-id="42282-161">principalName</span></span>       | <span data-ttu-id="42282-162">String</span><span class="sxs-lookup"><span data-stu-id="42282-162">String</span></span>                                | <span data-ttu-id="42282-163">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="42282-163">Name of the principal.</span></span>                                                             |
| <span data-ttu-id="42282-164">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="42282-164">externalPrincipalId</span></span> | <span data-ttu-id="42282-165">String</span><span class="sxs-lookup"><span data-stu-id="42282-165">String</span></span>                                | <span data-ttu-id="42282-166">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="42282-166">ID of principal in syncing system.</span></span>                                                 |
| <span data-ttu-id="42282-167">highestGrade</span><span class="sxs-lookup"><span data-stu-id="42282-167">highestGrade</span></span>        | <span data-ttu-id="42282-168">String</span><span class="sxs-lookup"><span data-stu-id="42282-168">String</span></span>                                | <span data-ttu-id="42282-169">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="42282-169">Highest grade taught.</span></span>                                                              |
| <span data-ttu-id="42282-170">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="42282-170">lowestGrade</span></span>         | <span data-ttu-id="42282-171">String</span><span class="sxs-lookup"><span data-stu-id="42282-171">String</span></span>                                | <span data-ttu-id="42282-172">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="42282-172">Lowest grade taught.</span></span>                                                               |
| <span data-ttu-id="42282-173">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="42282-173">schoolNumber</span></span>        | <span data-ttu-id="42282-174">String</span><span class="sxs-lookup"><span data-stu-id="42282-174">String</span></span>                                | <span data-ttu-id="42282-175">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="42282-175">School Number.</span></span>                                                                     |
| <span data-ttu-id="42282-176">externalId</span><span class="sxs-lookup"><span data-stu-id="42282-176">externalId</span></span>          | <span data-ttu-id="42282-177">String</span><span class="sxs-lookup"><span data-stu-id="42282-177">String</span></span>                                | <span data-ttu-id="42282-178">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="42282-178">ID of school in syncing system.</span></span>                                                    |
| <span data-ttu-id="42282-179">phone</span><span class="sxs-lookup"><span data-stu-id="42282-179">phone</span></span>               | <span data-ttu-id="42282-180">String</span><span class="sxs-lookup"><span data-stu-id="42282-180">String</span></span>                                | <span data-ttu-id="42282-181">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="42282-181">Phone number of school.</span></span>                                                            |
| <span data-ttu-id="42282-182">address</span><span class="sxs-lookup"><span data-stu-id="42282-182">address</span></span>             | [<span data-ttu-id="42282-183">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="42282-183">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="42282-184">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="42282-184">Address of the school.</span></span>                                                             |
| <span data-ttu-id="42282-185">createdBy</span><span class="sxs-lookup"><span data-stu-id="42282-185">createdBy</span></span>           | [<span data-ttu-id="42282-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="42282-186">identitySet</span></span>](identityset.md)         | <span data-ttu-id="42282-187">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="42282-187">Entity who created the school.</span></span>                                                     |

## <a name="relationships"></a><span data-ttu-id="42282-188">Связи</span><span class="sxs-lookup"><span data-stu-id="42282-188">Relationships</span></span>

| <span data-ttu-id="42282-189">Связь</span><span class="sxs-lookup"><span data-stu-id="42282-189">Relationship</span></span> | <span data-ttu-id="42282-190">Тип</span><span class="sxs-lookup"><span data-stu-id="42282-190">Type</span></span>                                           | <span data-ttu-id="42282-191">Описание</span><span class="sxs-lookup"><span data-stu-id="42282-191">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="42282-192">classes</span><span class="sxs-lookup"><span data-stu-id="42282-192">classes</span></span>      | <span data-ttu-id="42282-193">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="42282-193">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="42282-194">Классы, которые обучаются в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="42282-194">Classes taught at the school.</span></span> <span data-ttu-id="42282-195">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="42282-195">Nullable.</span></span> |
| <span data-ttu-id="42282-196">users</span><span class="sxs-lookup"><span data-stu-id="42282-196">users</span></span>        | <span data-ttu-id="42282-197">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="42282-197">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="42282-198">Пользователи в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="42282-198">Users in the school.</span></span> <span data-ttu-id="42282-199">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="42282-199">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="42282-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42282-200">JSON representation</span></span>

<span data-ttu-id="42282-201">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42282-201">The following is a JSON representation of the resource.</span></span>

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
  "phone": "String"
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

