---
title: Тип ресурса outlookTaskFolder
description: 'Папка, содержащая задачи Outlook (коллекцию объектов outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: eb61936b9ede67d35127db07c92ba8b7517fe623
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515302"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="69492-103">Тип ресурса outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="69492-103">outlookTaskFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69492-104">Папка, содержащая задачи Outlook (коллекцию объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="69492-104">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="69492-105">В программе Outlook, группа задач по умолчанию, `My Tasks`, содержащая папки задач по умолчанию, `Tasks`, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="69492-105">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="69492-106">Невозможно переименовать или удалить эти группы по умолчанию задач и папки, но можно создать дополнительные группы задач и папок задач.</span><span class="sxs-lookup"><span data-stu-id="69492-106">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="69492-107">Методы</span><span class="sxs-lookup"><span data-stu-id="69492-107">Methods</span></span>

| <span data-ttu-id="69492-108">Метод</span><span class="sxs-lookup"><span data-stu-id="69492-108">Method</span></span>           | <span data-ttu-id="69492-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="69492-109">Return Type</span></span>    |<span data-ttu-id="69492-110">Описание</span><span class="sxs-lookup"><span data-stu-id="69492-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69492-111">Получение outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="69492-111">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="69492-112">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="69492-112">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="69492-113">Получите свойства и связи указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="69492-113">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="69492-114">Создание outlookTask</span><span class="sxs-lookup"><span data-stu-id="69492-114">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="69492-115">outlookTask</span><span class="sxs-lookup"><span data-stu-id="69492-115">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="69492-116">Создание задачи Outlook в папке указанной задачи.</span><span class="sxs-lookup"><span data-stu-id="69492-116">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="69492-117">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="69492-117">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="69492-118">[outlookTask](outlooktask.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="69492-118">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="69492-119">Получите все задачи Outlook в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="69492-119">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="69492-120">Update</span><span class="sxs-lookup"><span data-stu-id="69492-120">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="69492-121">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="69492-121">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="69492-122">Обновление для записи свойств папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="69492-122">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="69492-123">Delete</span><span class="sxs-lookup"><span data-stu-id="69492-123">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="69492-124">Нет</span><span class="sxs-lookup"><span data-stu-id="69492-124">None</span></span> |<span data-ttu-id="69492-125">Удаление указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="69492-125">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="69492-126">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="69492-126">**Extended properties**</span></span>| | |
|[<span data-ttu-id="69492-127">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="69492-127">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="69492-128">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="69492-128">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="69492-129">Создайте один или несколько расширенных свойств одно значение в новую или существующую папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="69492-129">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="69492-130">Получение папки задач с одним значением расширенные свойства</span><span class="sxs-lookup"><span data-stu-id="69492-130">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="69492-131">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="69492-131">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="69492-132">Получение папки задач Outlook, которые содержат одно значение расширенные свойства с помощью `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="69492-132">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="69492-133">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="69492-133">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="69492-134">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="69492-134">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="69492-135">Создайте один или несколько расширенных свойств Многозначный в новую или существующую папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="69492-135">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="69492-136">Получение папки задач с несколькими значениями расширенные свойства</span><span class="sxs-lookup"><span data-stu-id="69492-136">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="69492-137">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="69492-137">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="69492-138">Получение папки задач Outlook, которая содержит свойство расширенного Многозначный с помощью `$expand`.</span><span class="sxs-lookup"><span data-stu-id="69492-138">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="69492-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="69492-139">Properties</span></span>
| <span data-ttu-id="69492-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="69492-140">Property</span></span>     | <span data-ttu-id="69492-141">Тип</span><span class="sxs-lookup"><span data-stu-id="69492-141">Type</span></span>   |<span data-ttu-id="69492-142">Описание</span><span class="sxs-lookup"><span data-stu-id="69492-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69492-143">changeKey</span><span class="sxs-lookup"><span data-stu-id="69492-143">changeKey</span></span>|<span data-ttu-id="69492-144">String</span><span class="sxs-lookup"><span data-stu-id="69492-144">String</span></span>|<span data-ttu-id="69492-145">Версия папки задач.</span><span class="sxs-lookup"><span data-stu-id="69492-145">The version of the task folder.</span></span>|
|<span data-ttu-id="69492-146">id</span><span class="sxs-lookup"><span data-stu-id="69492-146">id</span></span>|<span data-ttu-id="69492-147">String</span><span class="sxs-lookup"><span data-stu-id="69492-147">String</span></span>|<span data-ttu-id="69492-148">Идентификатор папки задач, уникальные в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="69492-148">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="69492-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69492-149">Read-only.</span></span>|
|<span data-ttu-id="69492-150">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="69492-150">isDefaultFolder</span></span>|<span data-ttu-id="69492-151">Логическое</span><span class="sxs-lookup"><span data-stu-id="69492-151">Boolean</span></span>|<span data-ttu-id="69492-152">Значение true, если папка является папки задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="69492-152">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="69492-153">name</span><span class="sxs-lookup"><span data-stu-id="69492-153">name</span></span>|<span data-ttu-id="69492-154">String</span><span class="sxs-lookup"><span data-stu-id="69492-154">String</span></span>|<span data-ttu-id="69492-155">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="69492-155">The name of the task folder.</span></span>|
|<span data-ttu-id="69492-156">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="69492-156">parentGroupKey</span></span>|<span data-ttu-id="69492-157">Guid</span><span class="sxs-lookup"><span data-stu-id="69492-157">Guid</span></span>|<span data-ttu-id="69492-158">Уникальный идентификатор GUID для родительской папки задач группы.</span><span class="sxs-lookup"><span data-stu-id="69492-158">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69492-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="69492-159">Relationships</span></span>
| <span data-ttu-id="69492-160">Связь</span><span class="sxs-lookup"><span data-stu-id="69492-160">Relationship</span></span> | <span data-ttu-id="69492-161">Тип</span><span class="sxs-lookup"><span data-stu-id="69492-161">Type</span></span>   |<span data-ttu-id="69492-162">Описание</span><span class="sxs-lookup"><span data-stu-id="69492-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69492-163">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="69492-163">multiValueExtendedProperties</span></span>|<span data-ttu-id="69492-164">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="69492-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="69492-165">Коллекция Многозначный расширенные свойства для папки задач.</span><span class="sxs-lookup"><span data-stu-id="69492-165">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="69492-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69492-166">Read-only.</span></span> <span data-ttu-id="69492-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="69492-167">Nullable.</span></span>|
|<span data-ttu-id="69492-168">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="69492-168">singleValueExtendedProperties</span></span>|<span data-ttu-id="69492-169">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="69492-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="69492-170">Коллекция расширенные свойства одно значение, определенное для папки задач.</span><span class="sxs-lookup"><span data-stu-id="69492-170">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="69492-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69492-171">Read-only.</span></span> <span data-ttu-id="69492-172">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="69492-172">Nullable.</span></span>|
|<span data-ttu-id="69492-173">tasks</span><span class="sxs-lookup"><span data-stu-id="69492-173">tasks</span></span>|<span data-ttu-id="69492-174">[outlookTask](outlooktask.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="69492-174">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="69492-175">Задачи в этой папке задач.</span><span class="sxs-lookup"><span data-stu-id="69492-175">The tasks in this task folder.</span></span> <span data-ttu-id="69492-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69492-176">Read-only.</span></span> <span data-ttu-id="69492-177">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="69492-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69492-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69492-178">JSON representation</span></span>
<span data-ttu-id="69492-179">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69492-179">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
  "@odata.type": "microsoft.graph.outlookTaskFolder"
}-->

```json
{
  "changeKey": "String",
  "id": "String (identifier)",
  "isDefaultFolder": true,
  "name": "String",
  "parentGroupKey": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktaskfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
