---
title: Тип ресурса educationClass
description: 'Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Office 365, для него используется тот же идентификатор. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d767f25fd5d383d297f3765498f3558a162f2716
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531541"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="e32a4-106">Тип ресурса educationClass</span><span class="sxs-lookup"><span data-stu-id="e32a4-106">educationClass resource type</span></span>

<span data-ttu-id="e32a4-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e32a4-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e32a4-108">Представляет курс в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="e32a4-108">Represents a class within a school.</span></span> <span data-ttu-id="e32a4-109">Ресурс **educationClass** соответствует группе Office 365, для него используется тот же идентификатор.</span><span class="sxs-lookup"><span data-stu-id="e32a4-109">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="e32a4-110">Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами.</span><span class="sxs-lookup"><span data-stu-id="e32a4-110">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="e32a4-111">Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.</span><span class="sxs-lookup"><span data-stu-id="e32a4-111">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="e32a4-112">Методы</span><span class="sxs-lookup"><span data-stu-id="e32a4-112">Methods</span></span>

| <span data-ttu-id="e32a4-113">Метод</span><span class="sxs-lookup"><span data-stu-id="e32a4-113">Method</span></span>           | <span data-ttu-id="e32a4-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e32a4-114">Return Type</span></span>    |<span data-ttu-id="e32a4-115">Описание</span><span class="sxs-lookup"><span data-stu-id="e32a4-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e32a4-116">Получение educationClass</span><span class="sxs-lookup"><span data-stu-id="e32a4-116">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="e32a4-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="e32a4-117">educationClass</span></span>](educationclass.md) |<span data-ttu-id="e32a4-118">Считывание свойств и связей объекта **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="e32a4-118">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="e32a4-119">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="e32a4-119">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="e32a4-120">educationUser</span><span class="sxs-lookup"><span data-stu-id="e32a4-120">educationUser</span></span>](educationuser.md)| <span data-ttu-id="e32a4-121">Добавление нового объекта **educationUser** для курса путем публикации в свойстве навигации members.</span><span class="sxs-lookup"><span data-stu-id="e32a4-121">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="e32a4-122">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="e32a4-122">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="e32a4-123">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="e32a4-123">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="e32a4-124">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="e32a4-124">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="e32a4-125">Удаление учащегося</span><span class="sxs-lookup"><span data-stu-id="e32a4-125">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="e32a4-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="e32a4-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="e32a4-127">Удаление **educationUser** для курса с использованием свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="e32a4-127">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="e32a4-128">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="e32a4-128">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="e32a4-129">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="e32a4-129">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="e32a4-130">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="e32a4-130">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="e32a4-131">Добавление преподавателя</span><span class="sxs-lookup"><span data-stu-id="e32a4-131">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="e32a4-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="e32a4-132">educationUser</span></span>](educationuser.md)| <span data-ttu-id="e32a4-133">Добавление нового объекта **educationUser** для курса путем публикации в свойстве навигации teachers.</span><span class="sxs-lookup"><span data-stu-id="e32a4-133">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="e32a4-134">Перечисление преподавателей</span><span class="sxs-lookup"><span data-stu-id="e32a4-134">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="e32a4-135">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="e32a4-135">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="e32a4-136">Получение списка преподавателей для курса.</span><span class="sxs-lookup"><span data-stu-id="e32a4-136">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="e32a4-137">Удаление преподавателя</span><span class="sxs-lookup"><span data-stu-id="e32a4-137">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="e32a4-138">educationUser</span><span class="sxs-lookup"><span data-stu-id="e32a4-138">educationUser</span></span>](educationuser.md)| <span data-ttu-id="e32a4-139">Удаление **educationUser** для курса с использованием свойства навигации teachers.</span><span class="sxs-lookup"><span data-stu-id="e32a4-139">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="e32a4-140">Получение группы</span><span class="sxs-lookup"><span data-stu-id="e32a4-140">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="e32a4-141">group</span><span class="sxs-lookup"><span data-stu-id="e32a4-141">group</span></span>](group.md)| <span data-ttu-id="e32a4-142">Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="e32a4-142">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="e32a4-143">Обновление</span><span class="sxs-lookup"><span data-stu-id="e32a4-143">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="e32a4-144">educationClass</span><span class="sxs-lookup"><span data-stu-id="e32a4-144">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="e32a4-145">Обновление объекта **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="e32a4-145">Update **educationClass** object.</span></span> |
|<span data-ttu-id="e32a4-146">[удаление](../api/educationclass-delete.md);</span><span class="sxs-lookup"><span data-stu-id="e32a4-146">[Delete](../api/educationclass-delete.md)</span></span> | <span data-ttu-id="e32a4-147">Нет</span><span class="sxs-lookup"><span data-stu-id="e32a4-147">None</span></span> |<span data-ttu-id="e32a4-148">Удаление объекта **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="e32a4-148">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e32a4-149">Свойства</span><span class="sxs-lookup"><span data-stu-id="e32a4-149">Properties</span></span>
| <span data-ttu-id="e32a4-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="e32a4-150">Property</span></span>     | <span data-ttu-id="e32a4-151">Тип</span><span class="sxs-lookup"><span data-stu-id="e32a4-151">Type</span></span>   |<span data-ttu-id="e32a4-152">Описание</span><span class="sxs-lookup"><span data-stu-id="e32a4-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e32a4-153">id</span><span class="sxs-lookup"><span data-stu-id="e32a4-153">id</span></span>| <span data-ttu-id="e32a4-154">Строка</span><span class="sxs-lookup"><span data-stu-id="e32a4-154">String</span></span>| <span data-ttu-id="e32a4-155">Уникальный идентификатор для курса.</span><span class="sxs-lookup"><span data-stu-id="e32a4-155">Unique identifier for the class.</span></span>|
|<span data-ttu-id="e32a4-156">description</span><span class="sxs-lookup"><span data-stu-id="e32a4-156">description</span></span>|<span data-ttu-id="e32a4-157">String</span><span class="sxs-lookup"><span data-stu-id="e32a4-157">String</span></span>| <span data-ttu-id="e32a4-158">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="e32a4-158">Description of the class.</span></span>|
|<span data-ttu-id="e32a4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e32a4-159">displayName</span></span>|<span data-ttu-id="e32a4-160">Строка</span><span class="sxs-lookup"><span data-stu-id="e32a4-160">String</span></span>| <span data-ttu-id="e32a4-161">Название курса.</span><span class="sxs-lookup"><span data-stu-id="e32a4-161">Name of the class.</span></span>|
|<span data-ttu-id="e32a4-162">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e32a4-162">mailNickname</span></span>|<span data-ttu-id="e32a4-163">String</span><span class="sxs-lookup"><span data-stu-id="e32a4-163">String</span></span>| <span data-ttu-id="e32a4-164">Почтовое имя для отправки почты всем участникам, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="e32a4-164">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="e32a4-165">createdBy</span><span class="sxs-lookup"><span data-stu-id="e32a4-165">createdBy</span></span>|[<span data-ttu-id="e32a4-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="e32a4-166">identitySet</span></span>](identityset.md)| <span data-ttu-id="e32a4-167">Объект, который создал курс.</span><span class="sxs-lookup"><span data-stu-id="e32a4-167">Entity who created the class</span></span> |
|<span data-ttu-id="e32a4-168">classCode</span><span class="sxs-lookup"><span data-stu-id="e32a4-168">classCode</span></span>|<span data-ttu-id="e32a4-169">String</span><span class="sxs-lookup"><span data-stu-id="e32a4-169">String</span></span>| <span data-ttu-id="e32a4-170">Код курса, используемый учебным заведением для идентификации курса.</span><span class="sxs-lookup"><span data-stu-id="e32a4-170">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="e32a4-171">externalId</span><span class="sxs-lookup"><span data-stu-id="e32a4-171">externalId</span></span>|<span data-ttu-id="e32a4-172">String</span><span class="sxs-lookup"><span data-stu-id="e32a4-172">String</span></span>| <span data-ttu-id="e32a4-173">Идентификатор курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e32a4-173">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="e32a4-174">externalName</span><span class="sxs-lookup"><span data-stu-id="e32a4-174">externalName</span></span>|<span data-ttu-id="e32a4-175">String</span><span class="sxs-lookup"><span data-stu-id="e32a4-175">String</span></span>|<span data-ttu-id="e32a4-176">Название курса в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e32a4-176">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="e32a4-177">externalSource</span><span class="sxs-lookup"><span data-stu-id="e32a4-177">externalSource</span></span>|<span data-ttu-id="e32a4-178">едукатионекстерналсаурце</span><span class="sxs-lookup"><span data-stu-id="e32a4-178">educationExternalSource</span></span>| <span data-ttu-id="e32a4-179">Способ создания этого курса.</span><span class="sxs-lookup"><span data-stu-id="e32a4-179">How this class was created.</span></span> <span data-ttu-id="e32a4-180">Допустимые значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e32a4-180">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e32a4-181">term</span><span class="sxs-lookup"><span data-stu-id="e32a4-181">term</span></span>|[<span data-ttu-id="e32a4-182">educationTerm</span><span class="sxs-lookup"><span data-stu-id="e32a4-182">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="e32a4-183">Срок для этого курса.</span><span class="sxs-lookup"><span data-stu-id="e32a4-183">Term for this class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e32a4-184">Связи</span><span class="sxs-lookup"><span data-stu-id="e32a4-184">Relationships</span></span>
| <span data-ttu-id="e32a4-185">Связь</span><span class="sxs-lookup"><span data-stu-id="e32a4-185">Relationship</span></span> | <span data-ttu-id="e32a4-186">Тип</span><span class="sxs-lookup"><span data-stu-id="e32a4-186">Type</span></span>   |<span data-ttu-id="e32a4-187">Описание</span><span class="sxs-lookup"><span data-stu-id="e32a4-187">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e32a4-188">members</span><span class="sxs-lookup"><span data-stu-id="e32a4-188">members</span></span>|<span data-ttu-id="e32a4-189">Коллекция [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="e32a4-189">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="e32a4-190">Все пользователи для этого курса.</span><span class="sxs-lookup"><span data-stu-id="e32a4-190">All users in the class.</span></span> <span data-ttu-id="e32a4-191">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e32a4-191">Nullable.</span></span>|
|<span data-ttu-id="e32a4-192">schools</span><span class="sxs-lookup"><span data-stu-id="e32a4-192">schools</span></span>|<span data-ttu-id="e32a4-193">Коллекция [educationSchool](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="e32a4-193">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="e32a4-194">Все учебные заведения, с которыми сопоставлен этот курс.</span><span class="sxs-lookup"><span data-stu-id="e32a4-194">All schools that this class is associated with.</span></span> <span data-ttu-id="e32a4-195">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="e32a4-195">Nullable.</span></span>|
|<span data-ttu-id="e32a4-196">teachers</span><span class="sxs-lookup"><span data-stu-id="e32a4-196">teachers</span></span>|<span data-ttu-id="e32a4-197">Коллекция [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="e32a4-197">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="e32a4-198">Все преподаватели для этого курса.</span><span class="sxs-lookup"><span data-stu-id="e32a4-198">All teachers in the class.</span></span> <span data-ttu-id="e32a4-199">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="e32a4-199">Nullable.</span></span>|
|<span data-ttu-id="e32a4-200">group</span><span class="sxs-lookup"><span data-stu-id="e32a4-200">group</span></span>|[<span data-ttu-id="e32a4-201">group</span><span class="sxs-lookup"><span data-stu-id="e32a4-201">group</span></span>](../resources/group.md)| <span data-ttu-id="e32a4-202">Группа каталогов, соответствующая этому классу.</span><span class="sxs-lookup"><span data-stu-id="e32a4-202">The directory group corresponding to this class.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e32a4-203">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e32a4-203">JSON representation</span></span>

<span data-ttu-id="e32a4-204">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e32a4-204">The following is a JSON representation of the resource.</span></span>

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
