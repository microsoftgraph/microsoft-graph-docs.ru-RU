---
title: Тип ресурса educationClass
description: 'Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Office 365, для него используется тот же идентификатор. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5a4bbc0560f2a40b5a438ec8276bbcf984a22721
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526734"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="9e992-106">Тип ресурса educationClass</span><span class="sxs-lookup"><span data-stu-id="9e992-106">educationClass resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e992-107">Представляет курс в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="9e992-107">Represents a class within a school.</span></span> <span data-ttu-id="9e992-108">Ресурс **educationClass** соответствует группе Office 365, для него используется тот же идентификатор.</span><span class="sxs-lookup"><span data-stu-id="9e992-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="9e992-109">Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами.</span><span class="sxs-lookup"><span data-stu-id="9e992-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="9e992-110">Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.</span><span class="sxs-lookup"><span data-stu-id="9e992-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="9e992-111">Методы</span><span class="sxs-lookup"><span data-stu-id="9e992-111">Methods</span></span>

| <span data-ttu-id="9e992-112">Метод</span><span class="sxs-lookup"><span data-stu-id="9e992-112">Method</span></span>           | <span data-ttu-id="9e992-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9e992-113">Return Type</span></span>    |<span data-ttu-id="9e992-114">Описание</span><span class="sxs-lookup"><span data-stu-id="9e992-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9e992-115">Получение educationClass</span><span class="sxs-lookup"><span data-stu-id="9e992-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="9e992-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="9e992-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="9e992-117">Считывание свойств и связей объекта **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="9e992-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="9e992-118">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="9e992-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="9e992-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="9e992-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="9e992-120">Добавление нового объекта **educationUser** для курса путем публикации в свойстве навигации members.</span><span class="sxs-lookup"><span data-stu-id="9e992-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="9e992-121">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="9e992-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="9e992-122">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="9e992-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="9e992-123">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="9e992-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="9e992-124">Удаление учащегося</span><span class="sxs-lookup"><span data-stu-id="9e992-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="9e992-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="9e992-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="9e992-126">Удаление **educationUser** для курса с использованием свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="9e992-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="9e992-127">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="9e992-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="9e992-128">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="9e992-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="9e992-129">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="9e992-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="9e992-130">Добавление преподавателя</span><span class="sxs-lookup"><span data-stu-id="9e992-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="9e992-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="9e992-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="9e992-132">Добавление нового объекта **educationUser** для курса путем публикации в свойстве навигации teachers.</span><span class="sxs-lookup"><span data-stu-id="9e992-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="9e992-133">Перечисление преподавателей</span><span class="sxs-lookup"><span data-stu-id="9e992-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="9e992-134">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="9e992-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="9e992-135">Получение списка преподавателей для курса.</span><span class="sxs-lookup"><span data-stu-id="9e992-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="9e992-136">Удаление преподавателя</span><span class="sxs-lookup"><span data-stu-id="9e992-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="9e992-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="9e992-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="9e992-138">Удаление **educationUser** для курса с использованием свойства навигации teachers.</span><span class="sxs-lookup"><span data-stu-id="9e992-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="9e992-139">Создание educationAssignment</span><span class="sxs-lookup"><span data-stu-id="9e992-139">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) |[<span data-ttu-id="9e992-140">educationAssignment</span><span class="sxs-lookup"><span data-stu-id="9e992-140">educationAssignment</span></span>](../resources/educationassignment.md)| <span data-ttu-id="9e992-141">Создайте новый **educationAssignment** , отправку сообщений семейства назначений.</span><span class="sxs-lookup"><span data-stu-id="9e992-141">Create a new **educationAssignment** by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="9e992-142">Список назначений</span><span class="sxs-lookup"><span data-stu-id="9e992-142">List assignments</span></span>](../api/educationclass-list-assignments.md) |<span data-ttu-id="9e992-143">[educationAssignment](../resources/educationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9e992-143">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="9e992-144">Получение коллекции объектов **educationAssignment** .</span><span class="sxs-lookup"><span data-stu-id="9e992-144">Get an **educationAssignment** object collection.</span></span>|
|[<span data-ttu-id="9e992-145">Получение группы</span><span class="sxs-lookup"><span data-stu-id="9e992-145">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="9e992-146">group</span><span class="sxs-lookup"><span data-stu-id="9e992-146">group</span></span>](group.md)| <span data-ttu-id="9e992-147">Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="9e992-147">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="9e992-148">Обновление</span><span class="sxs-lookup"><span data-stu-id="9e992-148">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="9e992-149">educationClass</span><span class="sxs-lookup"><span data-stu-id="9e992-149">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="9e992-150">Обновление объекта **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="9e992-150">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="9e992-151">Удаление</span><span class="sxs-lookup"><span data-stu-id="9e992-151">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="9e992-152">Нет</span><span class="sxs-lookup"><span data-stu-id="9e992-152">None</span></span> |<span data-ttu-id="9e992-153">Удаление объекта **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="9e992-153">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9e992-154">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e992-154">Properties</span></span>
| <span data-ttu-id="9e992-155">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e992-155">Property</span></span>     | <span data-ttu-id="9e992-156">Тип</span><span class="sxs-lookup"><span data-stu-id="9e992-156">Type</span></span>   |<span data-ttu-id="9e992-157">Описание</span><span class="sxs-lookup"><span data-stu-id="9e992-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e992-158">id</span><span class="sxs-lookup"><span data-stu-id="9e992-158">id</span></span>| <span data-ttu-id="9e992-159">String</span><span class="sxs-lookup"><span data-stu-id="9e992-159">String</span></span>| <span data-ttu-id="9e992-160">Уникальный идентификатор для курса.</span><span class="sxs-lookup"><span data-stu-id="9e992-160">Unique identifier for the class.</span></span>|
|<span data-ttu-id="9e992-161">description</span><span class="sxs-lookup"><span data-stu-id="9e992-161">description</span></span>|<span data-ttu-id="9e992-162">Строка</span><span class="sxs-lookup"><span data-stu-id="9e992-162">String</span></span>| <span data-ttu-id="9e992-163">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="9e992-163">Description of the class.</span></span>|
|<span data-ttu-id="9e992-164">displayName</span><span class="sxs-lookup"><span data-stu-id="9e992-164">displayName</span></span>|<span data-ttu-id="9e992-165">String</span><span class="sxs-lookup"><span data-stu-id="9e992-165">String</span></span>| <span data-ttu-id="9e992-166">Название курса.</span><span class="sxs-lookup"><span data-stu-id="9e992-166">Name of the class.</span></span>|
|<span data-ttu-id="9e992-167">mailNickname</span><span class="sxs-lookup"><span data-stu-id="9e992-167">mailNickname</span></span>|<span data-ttu-id="9e992-168">String</span><span class="sxs-lookup"><span data-stu-id="9e992-168">String</span></span>| <span data-ttu-id="9e992-169">Почтовое имя для отправки почты всем участникам, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="9e992-169">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="9e992-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="9e992-170">createdBy</span></span>|[<span data-ttu-id="9e992-171">identitySet</span><span class="sxs-lookup"><span data-stu-id="9e992-171">identitySet</span></span>](identityset.md)| <span data-ttu-id="9e992-172">Объект, который создал курс.</span><span class="sxs-lookup"><span data-stu-id="9e992-172">Entity who created the class</span></span> |
|<span data-ttu-id="9e992-173">classCode</span><span class="sxs-lookup"><span data-stu-id="9e992-173">classCode</span></span>|<span data-ttu-id="9e992-174">String</span><span class="sxs-lookup"><span data-stu-id="9e992-174">String</span></span>| <span data-ttu-id="9e992-175">Код курса, используемый учебным заведением для идентификации курса.</span><span class="sxs-lookup"><span data-stu-id="9e992-175">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="9e992-176">externalId</span><span class="sxs-lookup"><span data-stu-id="9e992-176">externalId</span></span>|<span data-ttu-id="9e992-177">String</span><span class="sxs-lookup"><span data-stu-id="9e992-177">String</span></span>| <span data-ttu-id="9e992-178">Идентификатор курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="9e992-178">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="9e992-179">externalName</span><span class="sxs-lookup"><span data-stu-id="9e992-179">externalName</span></span>|<span data-ttu-id="9e992-180">String</span><span class="sxs-lookup"><span data-stu-id="9e992-180">String</span></span>|<span data-ttu-id="9e992-181">Название курса в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="9e992-181">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="9e992-182">externalSource</span><span class="sxs-lookup"><span data-stu-id="9e992-182">externalSource</span></span>|<span data-ttu-id="9e992-183">string</span><span class="sxs-lookup"><span data-stu-id="9e992-183">string</span></span>| <span data-ttu-id="9e992-184">Способ создания этого курса.</span><span class="sxs-lookup"><span data-stu-id="9e992-184">How this class was created.</span></span> <span data-ttu-id="9e992-185">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9e992-185">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9e992-186">term</span><span class="sxs-lookup"><span data-stu-id="9e992-186">term</span></span>|[<span data-ttu-id="9e992-187">educationTerm</span><span class="sxs-lookup"><span data-stu-id="9e992-187">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="9e992-188">Срок для этого курса.</span><span class="sxs-lookup"><span data-stu-id="9e992-188">Term for this class.</span></span>|


## <a name="relationships"></a><span data-ttu-id="9e992-189">Связи</span><span class="sxs-lookup"><span data-stu-id="9e992-189">Relationships</span></span>
| <span data-ttu-id="9e992-190">Связь</span><span class="sxs-lookup"><span data-stu-id="9e992-190">Relationship</span></span> | <span data-ttu-id="9e992-191">Тип</span><span class="sxs-lookup"><span data-stu-id="9e992-191">Type</span></span>   |<span data-ttu-id="9e992-192">Описание</span><span class="sxs-lookup"><span data-stu-id="9e992-192">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e992-193">members</span><span class="sxs-lookup"><span data-stu-id="9e992-193">members</span></span>|<span data-ttu-id="9e992-194">Коллекция [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="9e992-194">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="9e992-195">Все пользователи для этого курса.</span><span class="sxs-lookup"><span data-stu-id="9e992-195">All users in the class.</span></span> <span data-ttu-id="9e992-196">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9e992-196">Nullable.</span></span>|
|<span data-ttu-id="9e992-197">schools</span><span class="sxs-lookup"><span data-stu-id="9e992-197">schools</span></span>|<span data-ttu-id="9e992-198">Коллекция [educationSchool](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="9e992-198">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="9e992-199">Все учебные заведения, с которыми сопоставлен этот курс.</span><span class="sxs-lookup"><span data-stu-id="9e992-199">All schools that this class is associated with.</span></span> <span data-ttu-id="9e992-200">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9e992-200">Nullable.</span></span>|
|<span data-ttu-id="9e992-201">teachers</span><span class="sxs-lookup"><span data-stu-id="9e992-201">teachers</span></span>|<span data-ttu-id="9e992-202">Коллекция [educationUser](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="9e992-202">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="9e992-203">Все преподаватели для этого курса.</span><span class="sxs-lookup"><span data-stu-id="9e992-203">All teachers in the class.</span></span> <span data-ttu-id="9e992-204">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="9e992-204">Nullable.</span></span>|
|<span data-ttu-id="9e992-205">assignments</span><span class="sxs-lookup"><span data-stu-id="9e992-205">assignments</span></span>|<span data-ttu-id="9e992-206">[educationAssignment](../resources/educationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9e992-206">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="9e992-207">Все назначения, связанных с этим классом.</span><span class="sxs-lookup"><span data-stu-id="9e992-207">All assignments associated with this class.</span></span> <span data-ttu-id="9e992-208">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9e992-208">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e992-209">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e992-209">JSON representation</span></span>

<span data-ttu-id="9e992-210">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e992-210">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationclass.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
