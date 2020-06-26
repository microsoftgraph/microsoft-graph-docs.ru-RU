---
title: Тип ресурса educationClass
description: 'Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Microsoft 365 и использует тот же идентификатор. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 78280017d71fe0cbcaa84ec22905da6848f45f98
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897885"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="1e9cf-106">Тип ресурса educationClass</span><span class="sxs-lookup"><span data-stu-id="1e9cf-106">educationClass resource type</span></span>

<span data-ttu-id="1e9cf-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e9cf-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e9cf-108">Представляет курс в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-108">Represents a class within a school.</span></span> <span data-ttu-id="1e9cf-109">Ресурс **educationClass** соответствует группе Microsoft 365 и использует тот же идентификатор.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-109">The **educationClass** resource corresponds to the Microsoft 365 group and shares the same ID.</span></span> <span data-ttu-id="1e9cf-110">Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-110">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="1e9cf-111">Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-111">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="1e9cf-112">Методы</span><span class="sxs-lookup"><span data-stu-id="1e9cf-112">Methods</span></span>

| <span data-ttu-id="1e9cf-113">Метод</span><span class="sxs-lookup"><span data-stu-id="1e9cf-113">Method</span></span>           | <span data-ttu-id="1e9cf-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1e9cf-114">Return Type</span></span>    |<span data-ttu-id="1e9cf-115">Описание</span><span class="sxs-lookup"><span data-stu-id="1e9cf-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1e9cf-116">Получение educationClass</span><span class="sxs-lookup"><span data-stu-id="1e9cf-116">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="1e9cf-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="1e9cf-117">educationClass</span></span>](educationclass.md) |<span data-ttu-id="1e9cf-118">Считывание свойств и связей объекта **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-118">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="1e9cf-119">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="1e9cf-119">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="1e9cf-120">educationUser</span><span class="sxs-lookup"><span data-stu-id="1e9cf-120">educationUser</span></span>](educationuser.md)| <span data-ttu-id="1e9cf-121">Добавление нового объекта **educationUser** для курса путем публикации в свойстве навигации members.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-121">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="1e9cf-122">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="1e9cf-122">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="1e9cf-123">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="1e9cf-123">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="1e9cf-124">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-124">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="1e9cf-125">Удаление учащегося</span><span class="sxs-lookup"><span data-stu-id="1e9cf-125">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="1e9cf-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="1e9cf-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="1e9cf-127">Удаление **educationUser** для курса с использованием свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-127">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="1e9cf-128">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="1e9cf-128">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="1e9cf-129">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="1e9cf-129">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="1e9cf-130">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-130">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="1e9cf-131">Добавление преподавателя</span><span class="sxs-lookup"><span data-stu-id="1e9cf-131">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="1e9cf-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="1e9cf-132">educationUser</span></span>](educationuser.md)| <span data-ttu-id="1e9cf-133">Добавление нового объекта **educationUser** для курса путем публикации в свойстве навигации teachers.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-133">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="1e9cf-134">Перечисление преподавателей</span><span class="sxs-lookup"><span data-stu-id="1e9cf-134">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="1e9cf-135">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="1e9cf-135">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="1e9cf-136">Получение списка преподавателей для курса.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-136">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="1e9cf-137">Удаление преподавателя</span><span class="sxs-lookup"><span data-stu-id="1e9cf-137">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="1e9cf-138">educationUser</span><span class="sxs-lookup"><span data-stu-id="1e9cf-138">educationUser</span></span>](educationuser.md)| <span data-ttu-id="1e9cf-139">Удаление **educationUser** для курса с использованием свойства навигации teachers.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-139">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="1e9cf-140">Получение группы</span><span class="sxs-lookup"><span data-stu-id="1e9cf-140">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="1e9cf-141">group</span><span class="sxs-lookup"><span data-stu-id="1e9cf-141">group</span></span>](group.md)| <span data-ttu-id="1e9cf-142">Получите **группу** Microsoft 365, соответствующую этой **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-142">Get the Microsoft 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="1e9cf-143">Обновление</span><span class="sxs-lookup"><span data-stu-id="1e9cf-143">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="1e9cf-144">educationClass</span><span class="sxs-lookup"><span data-stu-id="1e9cf-144">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="1e9cf-145">Обновление объекта **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-145">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="1e9cf-146">Delete</span><span class="sxs-lookup"><span data-stu-id="1e9cf-146">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="1e9cf-147">Нет</span><span class="sxs-lookup"><span data-stu-id="1e9cf-147">None</span></span> |<span data-ttu-id="1e9cf-148">Удаление объекта **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-148">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1e9cf-149">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e9cf-149">Properties</span></span>
| <span data-ttu-id="1e9cf-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e9cf-150">Property</span></span>     | <span data-ttu-id="1e9cf-151">Тип</span><span class="sxs-lookup"><span data-stu-id="1e9cf-151">Type</span></span>   |<span data-ttu-id="1e9cf-152">Описание</span><span class="sxs-lookup"><span data-stu-id="1e9cf-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e9cf-153">id</span><span class="sxs-lookup"><span data-stu-id="1e9cf-153">id</span></span>| <span data-ttu-id="1e9cf-154">Строка</span><span class="sxs-lookup"><span data-stu-id="1e9cf-154">String</span></span>| <span data-ttu-id="1e9cf-155">Уникальный идентификатор для курса.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-155">Unique identifier for the class.</span></span>|
|<span data-ttu-id="1e9cf-156">description</span><span class="sxs-lookup"><span data-stu-id="1e9cf-156">description</span></span>|<span data-ttu-id="1e9cf-157">String</span><span class="sxs-lookup"><span data-stu-id="1e9cf-157">String</span></span>| <span data-ttu-id="1e9cf-158">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-158">Description of the class.</span></span>|
|<span data-ttu-id="1e9cf-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1e9cf-159">displayName</span></span>|<span data-ttu-id="1e9cf-160">Строка</span><span class="sxs-lookup"><span data-stu-id="1e9cf-160">String</span></span>| <span data-ttu-id="1e9cf-161">Название курса.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-161">Name of the class.</span></span>|
|<span data-ttu-id="1e9cf-162">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1e9cf-162">mailNickname</span></span>|<span data-ttu-id="1e9cf-163">String</span><span class="sxs-lookup"><span data-stu-id="1e9cf-163">String</span></span>| <span data-ttu-id="1e9cf-164">Почтовое имя для отправки почты всем участникам, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-164">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="1e9cf-165">createdBy</span><span class="sxs-lookup"><span data-stu-id="1e9cf-165">createdBy</span></span>|[<span data-ttu-id="1e9cf-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="1e9cf-166">identitySet</span></span>](identityset.md)| <span data-ttu-id="1e9cf-167">Объект, который создал курс.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-167">Entity who created the class</span></span> |
|<span data-ttu-id="1e9cf-168">classCode</span><span class="sxs-lookup"><span data-stu-id="1e9cf-168">classCode</span></span>|<span data-ttu-id="1e9cf-169">String</span><span class="sxs-lookup"><span data-stu-id="1e9cf-169">String</span></span>| <span data-ttu-id="1e9cf-170">Код курса, используемый учебным заведением для идентификации курса.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-170">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="1e9cf-171">externalId</span><span class="sxs-lookup"><span data-stu-id="1e9cf-171">externalId</span></span>|<span data-ttu-id="1e9cf-172">String</span><span class="sxs-lookup"><span data-stu-id="1e9cf-172">String</span></span>| <span data-ttu-id="1e9cf-173">Идентификатор курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-173">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="1e9cf-174">externalName</span><span class="sxs-lookup"><span data-stu-id="1e9cf-174">externalName</span></span>|<span data-ttu-id="1e9cf-175">String</span><span class="sxs-lookup"><span data-stu-id="1e9cf-175">String</span></span>|<span data-ttu-id="1e9cf-176">Название курса в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-176">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="1e9cf-177">externalSource</span><span class="sxs-lookup"><span data-stu-id="1e9cf-177">externalSource</span></span>|<span data-ttu-id="1e9cf-178">едукатионекстерналсаурце</span><span class="sxs-lookup"><span data-stu-id="1e9cf-178">educationExternalSource</span></span>| <span data-ttu-id="1e9cf-179">Способ создания этого курса.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-179">How this class was created.</span></span> <span data-ttu-id="1e9cf-180">Допустимые значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-180">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1e9cf-181">term</span><span class="sxs-lookup"><span data-stu-id="1e9cf-181">term</span></span>|[<span data-ttu-id="1e9cf-182">educationTerm</span><span class="sxs-lookup"><span data-stu-id="1e9cf-182">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="1e9cf-183">Срок для этого курса.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-183">Term for this class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e9cf-184">Связи</span><span class="sxs-lookup"><span data-stu-id="1e9cf-184">Relationships</span></span>
| <span data-ttu-id="1e9cf-185">Связь</span><span class="sxs-lookup"><span data-stu-id="1e9cf-185">Relationship</span></span> | <span data-ttu-id="1e9cf-186">Тип</span><span class="sxs-lookup"><span data-stu-id="1e9cf-186">Type</span></span>   |<span data-ttu-id="1e9cf-187">Описание</span><span class="sxs-lookup"><span data-stu-id="1e9cf-187">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e9cf-188">members</span><span class="sxs-lookup"><span data-stu-id="1e9cf-188">members</span></span>|<span data-ttu-id="1e9cf-189">Коллекция [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="1e9cf-189">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="1e9cf-190">Все пользователи для этого курса.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-190">All users in the class.</span></span> <span data-ttu-id="1e9cf-191">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-191">Nullable.</span></span>|
|<span data-ttu-id="1e9cf-192">schools</span><span class="sxs-lookup"><span data-stu-id="1e9cf-192">schools</span></span>|<span data-ttu-id="1e9cf-193">Коллекция [educationSchool](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="1e9cf-193">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="1e9cf-194">Все учебные заведения, с которыми сопоставлен этот курс.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-194">All schools that this class is associated with.</span></span> <span data-ttu-id="1e9cf-195">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-195">Nullable.</span></span>|
|<span data-ttu-id="1e9cf-196">teachers</span><span class="sxs-lookup"><span data-stu-id="1e9cf-196">teachers</span></span>|<span data-ttu-id="1e9cf-197">Коллекция [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="1e9cf-197">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="1e9cf-198">Все преподаватели для этого курса.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-198">All teachers in the class.</span></span> <span data-ttu-id="1e9cf-199">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-199">Nullable.</span></span>|
|<span data-ttu-id="1e9cf-200">group</span><span class="sxs-lookup"><span data-stu-id="1e9cf-200">group</span></span>|[<span data-ttu-id="1e9cf-201">group</span><span class="sxs-lookup"><span data-stu-id="1e9cf-201">group</span></span>](../resources/group.md)| <span data-ttu-id="1e9cf-202">Группа каталогов, соответствующая этому классу.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-202">The directory group corresponding to this class.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e9cf-203">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1e9cf-203">JSON representation</span></span>

<span data-ttu-id="1e9cf-204">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e9cf-204">The following is a JSON representation of the resource.</span></span>

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
