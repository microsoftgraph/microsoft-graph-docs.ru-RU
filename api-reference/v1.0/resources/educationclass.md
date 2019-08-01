---
title: Тип ресурса educationClass
description: 'Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Office 365, для него используется тот же идентификатор. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1dc246c3a8f48980b65c896bba4b6fbe1ae66809
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029332"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="f7a92-106">Тип ресурса educationClass</span><span class="sxs-lookup"><span data-stu-id="f7a92-106">educationClass resource type</span></span>

<span data-ttu-id="f7a92-107">Представляет курс в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="f7a92-107">Represents a class within a school.</span></span> <span data-ttu-id="f7a92-108">Ресурс **educationClass** соответствует группе Office 365, для него используется тот же идентификатор.</span><span class="sxs-lookup"><span data-stu-id="f7a92-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="f7a92-109">Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами.</span><span class="sxs-lookup"><span data-stu-id="f7a92-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="f7a92-110">Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.</span><span class="sxs-lookup"><span data-stu-id="f7a92-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="f7a92-111">Методы</span><span class="sxs-lookup"><span data-stu-id="f7a92-111">Methods</span></span>

| <span data-ttu-id="f7a92-112">Метод</span><span class="sxs-lookup"><span data-stu-id="f7a92-112">Method</span></span>           | <span data-ttu-id="f7a92-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f7a92-113">Return Type</span></span>    |<span data-ttu-id="f7a92-114">Описание</span><span class="sxs-lookup"><span data-stu-id="f7a92-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f7a92-115">Получение educationClass</span><span class="sxs-lookup"><span data-stu-id="f7a92-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="f7a92-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="f7a92-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="f7a92-117">Считывание свойств и связей объекта **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="f7a92-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="f7a92-118">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="f7a92-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="f7a92-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="f7a92-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="f7a92-120">Добавление нового объекта **educationUser** для курса путем публикации в свойстве навигации members.</span><span class="sxs-lookup"><span data-stu-id="f7a92-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="f7a92-121">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="f7a92-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="f7a92-122">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="f7a92-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="f7a92-123">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="f7a92-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="f7a92-124">Удаление учащегося</span><span class="sxs-lookup"><span data-stu-id="f7a92-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="f7a92-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="f7a92-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="f7a92-126">Удаление **educationUser** для курса с использованием свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="f7a92-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="f7a92-127">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="f7a92-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="f7a92-128">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="f7a92-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="f7a92-129">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="f7a92-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="f7a92-130">Добавление преподавателя</span><span class="sxs-lookup"><span data-stu-id="f7a92-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="f7a92-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="f7a92-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="f7a92-132">Добавление нового объекта **educationUser** для курса путем публикации в свойстве навигации teachers.</span><span class="sxs-lookup"><span data-stu-id="f7a92-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="f7a92-133">Перечисление преподавателей</span><span class="sxs-lookup"><span data-stu-id="f7a92-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="f7a92-134">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="f7a92-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="f7a92-135">Получение списка преподавателей для курса.</span><span class="sxs-lookup"><span data-stu-id="f7a92-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="f7a92-136">Удаление преподавателя</span><span class="sxs-lookup"><span data-stu-id="f7a92-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="f7a92-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="f7a92-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="f7a92-138">Удаление **educationUser** для курса с использованием свойства навигации teachers.</span><span class="sxs-lookup"><span data-stu-id="f7a92-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="f7a92-139">Получение группы</span><span class="sxs-lookup"><span data-stu-id="f7a92-139">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="f7a92-140">group</span><span class="sxs-lookup"><span data-stu-id="f7a92-140">group</span></span>](group.md)| <span data-ttu-id="f7a92-141">Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="f7a92-141">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="f7a92-142">Обновление</span><span class="sxs-lookup"><span data-stu-id="f7a92-142">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="f7a92-143">educationClass</span><span class="sxs-lookup"><span data-stu-id="f7a92-143">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="f7a92-144">Обновление объекта **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="f7a92-144">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="f7a92-145">Удаление</span><span class="sxs-lookup"><span data-stu-id="f7a92-145">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="f7a92-146">Нет</span><span class="sxs-lookup"><span data-stu-id="f7a92-146">None</span></span> |<span data-ttu-id="f7a92-147">Удаление объекта **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="f7a92-147">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f7a92-148">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7a92-148">Properties</span></span>
| <span data-ttu-id="f7a92-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7a92-149">Property</span></span>     | <span data-ttu-id="f7a92-150">Тип</span><span class="sxs-lookup"><span data-stu-id="f7a92-150">Type</span></span>   |<span data-ttu-id="f7a92-151">Описание</span><span class="sxs-lookup"><span data-stu-id="f7a92-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7a92-152">id</span><span class="sxs-lookup"><span data-stu-id="f7a92-152">id</span></span>| <span data-ttu-id="f7a92-153">Строка</span><span class="sxs-lookup"><span data-stu-id="f7a92-153">String</span></span>| <span data-ttu-id="f7a92-154">Уникальный идентификатор для курса.</span><span class="sxs-lookup"><span data-stu-id="f7a92-154">Unique identifier for the class.</span></span>|
|<span data-ttu-id="f7a92-155">description</span><span class="sxs-lookup"><span data-stu-id="f7a92-155">description</span></span>|<span data-ttu-id="f7a92-156">String</span><span class="sxs-lookup"><span data-stu-id="f7a92-156">String</span></span>| <span data-ttu-id="f7a92-157">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="f7a92-157">Description of the class.</span></span>|
|<span data-ttu-id="f7a92-158">displayName</span><span class="sxs-lookup"><span data-stu-id="f7a92-158">displayName</span></span>|<span data-ttu-id="f7a92-159">Строка</span><span class="sxs-lookup"><span data-stu-id="f7a92-159">String</span></span>| <span data-ttu-id="f7a92-160">Название курса.</span><span class="sxs-lookup"><span data-stu-id="f7a92-160">Name of the class.</span></span>|
|<span data-ttu-id="f7a92-161">mailNickname</span><span class="sxs-lookup"><span data-stu-id="f7a92-161">mailNickname</span></span>|<span data-ttu-id="f7a92-162">String</span><span class="sxs-lookup"><span data-stu-id="f7a92-162">String</span></span>| <span data-ttu-id="f7a92-163">Почтовое имя для отправки почты всем участникам, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="f7a92-163">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="f7a92-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="f7a92-164">createdBy</span></span>|[<span data-ttu-id="f7a92-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="f7a92-165">identitySet</span></span>](identityset.md)| <span data-ttu-id="f7a92-166">Объект, который создал курс.</span><span class="sxs-lookup"><span data-stu-id="f7a92-166">Entity who created the class</span></span> |
|<span data-ttu-id="f7a92-167">classCode</span><span class="sxs-lookup"><span data-stu-id="f7a92-167">classCode</span></span>|<span data-ttu-id="f7a92-168">String</span><span class="sxs-lookup"><span data-stu-id="f7a92-168">String</span></span>| <span data-ttu-id="f7a92-169">Код курса, используемый учебным заведением для идентификации курса.</span><span class="sxs-lookup"><span data-stu-id="f7a92-169">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="f7a92-170">externalId</span><span class="sxs-lookup"><span data-stu-id="f7a92-170">externalId</span></span>|<span data-ttu-id="f7a92-171">String</span><span class="sxs-lookup"><span data-stu-id="f7a92-171">String</span></span>| <span data-ttu-id="f7a92-172">Идентификатор курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f7a92-172">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="f7a92-173">externalName</span><span class="sxs-lookup"><span data-stu-id="f7a92-173">externalName</span></span>|<span data-ttu-id="f7a92-174">String</span><span class="sxs-lookup"><span data-stu-id="f7a92-174">String</span></span>|<span data-ttu-id="f7a92-175">Название курса в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f7a92-175">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="f7a92-176">externalSource</span><span class="sxs-lookup"><span data-stu-id="f7a92-176">externalSource</span></span>|<span data-ttu-id="f7a92-177">Едукатионекстерналсаурце</span><span class="sxs-lookup"><span data-stu-id="f7a92-177">educationExternalSource</span></span>| <span data-ttu-id="f7a92-178">Способ создания этого курса.</span><span class="sxs-lookup"><span data-stu-id="f7a92-178">How this class was created.</span></span> <span data-ttu-id="f7a92-179">Допустимые значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f7a92-179">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f7a92-180">term</span><span class="sxs-lookup"><span data-stu-id="f7a92-180">term</span></span>|[<span data-ttu-id="f7a92-181">educationTerm</span><span class="sxs-lookup"><span data-stu-id="f7a92-181">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="f7a92-182">Срок для этого курса.</span><span class="sxs-lookup"><span data-stu-id="f7a92-182">Term for this class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7a92-183">Отношения</span><span class="sxs-lookup"><span data-stu-id="f7a92-183">Relationships</span></span>
| <span data-ttu-id="f7a92-184">Отношение</span><span class="sxs-lookup"><span data-stu-id="f7a92-184">Relationship</span></span> | <span data-ttu-id="f7a92-185">Тип</span><span class="sxs-lookup"><span data-stu-id="f7a92-185">Type</span></span>   |<span data-ttu-id="f7a92-186">Описание</span><span class="sxs-lookup"><span data-stu-id="f7a92-186">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7a92-187">members</span><span class="sxs-lookup"><span data-stu-id="f7a92-187">members</span></span>|<span data-ttu-id="f7a92-188">Коллекция [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="f7a92-188">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="f7a92-189">Все пользователи для этого курса.</span><span class="sxs-lookup"><span data-stu-id="f7a92-189">All users in the class.</span></span> <span data-ttu-id="f7a92-190">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f7a92-190">Nullable.</span></span>|
|<span data-ttu-id="f7a92-191">schools</span><span class="sxs-lookup"><span data-stu-id="f7a92-191">schools</span></span>|<span data-ttu-id="f7a92-192">Коллекция [educationSchool](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="f7a92-192">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="f7a92-193">Все учебные заведения, с которыми сопоставлен этот курс.</span><span class="sxs-lookup"><span data-stu-id="f7a92-193">All schools that this class is associated with.</span></span> <span data-ttu-id="f7a92-194">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="f7a92-194">Nullable.</span></span>|
|<span data-ttu-id="f7a92-195">teachers</span><span class="sxs-lookup"><span data-stu-id="f7a92-195">teachers</span></span>|<span data-ttu-id="f7a92-196">Коллекция [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="f7a92-196">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="f7a92-197">Все преподаватели для этого курса.</span><span class="sxs-lookup"><span data-stu-id="f7a92-197">All teachers in the class.</span></span> <span data-ttu-id="f7a92-198">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="f7a92-198">Nullable.</span></span>|
|<span data-ttu-id="f7a92-199">group</span><span class="sxs-lookup"><span data-stu-id="f7a92-199">group</span></span>|[<span data-ttu-id="f7a92-200">group</span><span class="sxs-lookup"><span data-stu-id="f7a92-200">group</span></span>](../resources/group.md)| <span data-ttu-id="f7a92-201">Группа каталогов, соответствующая этому классу.</span><span class="sxs-lookup"><span data-stu-id="f7a92-201">The directory group corresponding to this class.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7a92-202">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7a92-202">JSON representation</span></span>

<span data-ttu-id="f7a92-203">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7a92-203">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.educationTerm"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
