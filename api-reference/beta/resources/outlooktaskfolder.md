---
title: Тип ресурса outlookTaskFolder
description: 'Папка, содержащая задачи Outlook (коллекцию объектов outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a117e14ea1cfe4b69cbbf69720a22a0094fb0b72
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575669"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="4f20a-103">Тип ресурса outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="4f20a-103">outlookTaskFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f20a-104">Папка, содержащая задачи Outlook (коллекцию объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="4f20a-104">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="4f20a-105">В программе Outlook, группа задач по умолчанию, `My Tasks`, содержащая папки задач по умолчанию, `Tasks`, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f20a-105">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="4f20a-106">Невозможно переименовать или удалить эти группы по умолчанию задач и папки, но можно создать дополнительные группы задач и папок задач.</span><span class="sxs-lookup"><span data-stu-id="4f20a-106">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="4f20a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="4f20a-107">Methods</span></span>

| <span data-ttu-id="4f20a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="4f20a-108">Method</span></span>           | <span data-ttu-id="4f20a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4f20a-109">Return Type</span></span>    |<span data-ttu-id="4f20a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4f20a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4f20a-111">Получение outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="4f20a-111">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="4f20a-112">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="4f20a-112">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="4f20a-113">Получите свойства и связи указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="4f20a-113">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="4f20a-114">Создание outlookTask</span><span class="sxs-lookup"><span data-stu-id="4f20a-114">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="4f20a-115">outlookTask</span><span class="sxs-lookup"><span data-stu-id="4f20a-115">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="4f20a-116">Создание задачи Outlook в папке указанной задачи.</span><span class="sxs-lookup"><span data-stu-id="4f20a-116">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="4f20a-117">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="4f20a-117">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="4f20a-118">[outlookTask](outlooktask.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4f20a-118">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="4f20a-119">Получите все задачи Outlook в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="4f20a-119">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="4f20a-120">Update</span><span class="sxs-lookup"><span data-stu-id="4f20a-120">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="4f20a-121">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="4f20a-121">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="4f20a-122">Обновление для записи свойств папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="4f20a-122">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="4f20a-123">Delete</span><span class="sxs-lookup"><span data-stu-id="4f20a-123">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="4f20a-124">Нет</span><span class="sxs-lookup"><span data-stu-id="4f20a-124">None</span></span> |<span data-ttu-id="4f20a-125">Удаление указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="4f20a-125">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="4f20a-126">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="4f20a-126">**Extended properties**</span></span>| | |
|[<span data-ttu-id="4f20a-127">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="4f20a-127">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="4f20a-128">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="4f20a-128">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="4f20a-129">Создайте один или несколько расширенных свойств одно значение в новую или существующую папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="4f20a-129">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="4f20a-130">Получение папки задач с одним значением расширенные свойства</span><span class="sxs-lookup"><span data-stu-id="4f20a-130">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="4f20a-131">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="4f20a-131">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="4f20a-132">Получение папки задач Outlook, которые содержат одно значение расширенные свойства с помощью `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="4f20a-132">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="4f20a-133">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="4f20a-133">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="4f20a-134">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="4f20a-134">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="4f20a-135">Создайте один или несколько расширенных свойств Многозначный в новую или существующую папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="4f20a-135">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="4f20a-136">Получение папки задач с несколькими значениями расширенные свойства</span><span class="sxs-lookup"><span data-stu-id="4f20a-136">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="4f20a-137">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="4f20a-137">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="4f20a-138">Получение папки задач Outlook, которая содержит свойство расширенного Многозначный с помощью `$expand`.</span><span class="sxs-lookup"><span data-stu-id="4f20a-138">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="4f20a-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f20a-139">Properties</span></span>
| <span data-ttu-id="4f20a-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f20a-140">Property</span></span>     | <span data-ttu-id="4f20a-141">Тип</span><span class="sxs-lookup"><span data-stu-id="4f20a-141">Type</span></span>   |<span data-ttu-id="4f20a-142">Описание</span><span class="sxs-lookup"><span data-stu-id="4f20a-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f20a-143">changeKey</span><span class="sxs-lookup"><span data-stu-id="4f20a-143">changeKey</span></span>|<span data-ttu-id="4f20a-144">Строка</span><span class="sxs-lookup"><span data-stu-id="4f20a-144">String</span></span>|<span data-ttu-id="4f20a-145">Версия папки задач.</span><span class="sxs-lookup"><span data-stu-id="4f20a-145">The version of the task folder.</span></span>|
|<span data-ttu-id="4f20a-146">id</span><span class="sxs-lookup"><span data-stu-id="4f20a-146">id</span></span>|<span data-ttu-id="4f20a-147">Строка</span><span class="sxs-lookup"><span data-stu-id="4f20a-147">String</span></span>|<span data-ttu-id="4f20a-148">Идентификатор папки задач, уникальные в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f20a-148">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="4f20a-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f20a-149">Read-only.</span></span>|
|<span data-ttu-id="4f20a-150">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="4f20a-150">isDefaultFolder</span></span>|<span data-ttu-id="4f20a-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f20a-151">Boolean</span></span>|<span data-ttu-id="4f20a-152">Значение true, если папка является папки задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4f20a-152">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="4f20a-153">name</span><span class="sxs-lookup"><span data-stu-id="4f20a-153">name</span></span>|<span data-ttu-id="4f20a-154">Строка</span><span class="sxs-lookup"><span data-stu-id="4f20a-154">String</span></span>|<span data-ttu-id="4f20a-155">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="4f20a-155">The name of the task folder.</span></span>|
|<span data-ttu-id="4f20a-156">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="4f20a-156">parentGroupKey</span></span>|<span data-ttu-id="4f20a-157">Guid</span><span class="sxs-lookup"><span data-stu-id="4f20a-157">Guid</span></span>|<span data-ttu-id="4f20a-158">Уникальный идентификатор GUID для родительской папки задач группы.</span><span class="sxs-lookup"><span data-stu-id="4f20a-158">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f20a-159">Связи</span><span class="sxs-lookup"><span data-stu-id="4f20a-159">Relationships</span></span>
| <span data-ttu-id="4f20a-160">Связь</span><span class="sxs-lookup"><span data-stu-id="4f20a-160">Relationship</span></span> | <span data-ttu-id="4f20a-161">Тип</span><span class="sxs-lookup"><span data-stu-id="4f20a-161">Type</span></span>   |<span data-ttu-id="4f20a-162">Описание</span><span class="sxs-lookup"><span data-stu-id="4f20a-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f20a-163">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="4f20a-163">multiValueLegacyExtendedProperty</span></span>|<span data-ttu-id="4f20a-164">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="4f20a-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="4f20a-165">Коллекция Многозначный расширенные свойства для папки задач.</span><span class="sxs-lookup"><span data-stu-id="4f20a-165">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="4f20a-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f20a-166">Read-only.</span></span> <span data-ttu-id="4f20a-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4f20a-167">Nullable.</span></span>|
|<span data-ttu-id="4f20a-168">singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="4f20a-168">singleValueLegacyExtendedProperty</span></span>|<span data-ttu-id="4f20a-169">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="4f20a-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="4f20a-170">Коллекция расширенные свойства одно значение, определенное для папки задач.</span><span class="sxs-lookup"><span data-stu-id="4f20a-170">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="4f20a-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f20a-171">Read-only.</span></span> <span data-ttu-id="4f20a-172">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4f20a-172">Nullable.</span></span>|
|<span data-ttu-id="4f20a-173">tasks</span><span class="sxs-lookup"><span data-stu-id="4f20a-173">tasks</span></span>|<span data-ttu-id="4f20a-174">[outlookTask](outlooktask.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4f20a-174">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="4f20a-175">Задачи в этой папке задач.</span><span class="sxs-lookup"><span data-stu-id="4f20a-175">The tasks in this task folder.</span></span> <span data-ttu-id="4f20a-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f20a-176">Read-only.</span></span> <span data-ttu-id="4f20a-177">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4f20a-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f20a-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f20a-178">JSON representation</span></span>
<span data-ttu-id="4f20a-179">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f20a-179">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueLegacyExtendedProperty",
    "singleValueLegacyExtendedProperty",
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
