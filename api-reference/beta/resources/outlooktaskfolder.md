---
title: Тип ресурса outlookTaskFolder
description: 'Папка, содержащая задачи Outlook (коллекцию объектов outlookTask). '
ms.openlocfilehash: e3fb9d73dbd9458048749331d14f933d838d4243
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080321"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="8883c-103">Тип ресурса outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="8883c-103">outlookTaskFolder resource type</span></span>

> <span data-ttu-id="8883c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8883c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8883c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8883c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8883c-106">Папка, содержащая задачи Outlook (коллекцию объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="8883c-106">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="8883c-107">В программе Outlook, группа задач по умолчанию, `My Tasks`, содержащая папки задач по умолчанию, `Tasks`, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="8883c-107">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="8883c-108">Невозможно переименовать или удалить эти группы по умолчанию задач и папки, но можно создать дополнительные группы задач и папок задач.</span><span class="sxs-lookup"><span data-stu-id="8883c-108">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="8883c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="8883c-109">Methods</span></span>

| <span data-ttu-id="8883c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="8883c-110">Method</span></span>           | <span data-ttu-id="8883c-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8883c-111">Return Type</span></span>    |<span data-ttu-id="8883c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8883c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8883c-113">Получение outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="8883c-113">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="8883c-114">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="8883c-114">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="8883c-115">Получите свойства и связи указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="8883c-115">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="8883c-116">Создание outlookTask</span><span class="sxs-lookup"><span data-stu-id="8883c-116">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="8883c-117">outlookTask</span><span class="sxs-lookup"><span data-stu-id="8883c-117">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="8883c-118">Создание задачи Outlook в папке указанной задачи.</span><span class="sxs-lookup"><span data-stu-id="8883c-118">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="8883c-119">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="8883c-119">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="8883c-120">[outlookTask](outlooktask.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8883c-120">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="8883c-121">Получите все задачи Outlook в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="8883c-121">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="8883c-122">Update</span><span class="sxs-lookup"><span data-stu-id="8883c-122">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="8883c-123">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="8883c-123">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="8883c-124">Обновление для записи свойств папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="8883c-124">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="8883c-125">Delete</span><span class="sxs-lookup"><span data-stu-id="8883c-125">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="8883c-126">Нет</span><span class="sxs-lookup"><span data-stu-id="8883c-126">None</span></span> |<span data-ttu-id="8883c-127">Удаление указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="8883c-127">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="8883c-128">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="8883c-128">**Extended properties**</span></span>| | |
|[<span data-ttu-id="8883c-129">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="8883c-129">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="8883c-130">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="8883c-130">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="8883c-131">Создайте один или несколько расширенных свойств одно значение в новую или существующую папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="8883c-131">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="8883c-132">Получение папки задач с одним значением расширенные свойства</span><span class="sxs-lookup"><span data-stu-id="8883c-132">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="8883c-133">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="8883c-133">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="8883c-134">Получение папки задач Outlook, которые содержат одно значение расширенные свойства с помощью `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="8883c-134">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="8883c-135">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="8883c-135">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="8883c-136">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="8883c-136">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="8883c-137">Создайте один или несколько расширенных свойств Многозначный в новую или существующую папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="8883c-137">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="8883c-138">Получение папки задач с несколькими значениями расширенные свойства</span><span class="sxs-lookup"><span data-stu-id="8883c-138">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="8883c-139">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="8883c-139">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="8883c-140">Получение папки задач Outlook, которая содержит свойство расширенного Многозначный с помощью `$expand`.</span><span class="sxs-lookup"><span data-stu-id="8883c-140">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="8883c-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="8883c-141">Properties</span></span>
| <span data-ttu-id="8883c-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="8883c-142">Property</span></span>     | <span data-ttu-id="8883c-143">Тип</span><span class="sxs-lookup"><span data-stu-id="8883c-143">Type</span></span>   |<span data-ttu-id="8883c-144">Описание</span><span class="sxs-lookup"><span data-stu-id="8883c-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8883c-145">changeKey</span><span class="sxs-lookup"><span data-stu-id="8883c-145">changeKey</span></span>|<span data-ttu-id="8883c-146">String</span><span class="sxs-lookup"><span data-stu-id="8883c-146">String</span></span>|<span data-ttu-id="8883c-147">Версия папки задач.</span><span class="sxs-lookup"><span data-stu-id="8883c-147">The version of the task folder.</span></span>|
|<span data-ttu-id="8883c-148">id</span><span class="sxs-lookup"><span data-stu-id="8883c-148">id</span></span>|<span data-ttu-id="8883c-149">String</span><span class="sxs-lookup"><span data-stu-id="8883c-149">String</span></span>|<span data-ttu-id="8883c-150">Идентификатор папки задач, уникальные в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="8883c-150">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="8883c-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8883c-151">Read-only.</span></span>|
|<span data-ttu-id="8883c-152">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="8883c-152">isDefaultFolder</span></span>|<span data-ttu-id="8883c-153">Логический</span><span class="sxs-lookup"><span data-stu-id="8883c-153">Boolean</span></span>|<span data-ttu-id="8883c-154">Значение true, если папка является папки задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8883c-154">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="8883c-155">name</span><span class="sxs-lookup"><span data-stu-id="8883c-155">name</span></span>|<span data-ttu-id="8883c-156">String</span><span class="sxs-lookup"><span data-stu-id="8883c-156">String</span></span>|<span data-ttu-id="8883c-157">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="8883c-157">The name of the task folder.</span></span>|
|<span data-ttu-id="8883c-158">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="8883c-158">parentGroupKey</span></span>|<span data-ttu-id="8883c-159">Guid</span><span class="sxs-lookup"><span data-stu-id="8883c-159">Guid</span></span>|<span data-ttu-id="8883c-160">Уникальный идентификатор GUID для родительской папки задач группы.</span><span class="sxs-lookup"><span data-stu-id="8883c-160">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8883c-161">Связи</span><span class="sxs-lookup"><span data-stu-id="8883c-161">Relationships</span></span>
| <span data-ttu-id="8883c-162">Связь</span><span class="sxs-lookup"><span data-stu-id="8883c-162">Relationship</span></span> | <span data-ttu-id="8883c-163">Тип</span><span class="sxs-lookup"><span data-stu-id="8883c-163">Type</span></span>   |<span data-ttu-id="8883c-164">Description</span><span class="sxs-lookup"><span data-stu-id="8883c-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8883c-165">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="8883c-165">multiValueExtendedProperties</span></span>|<span data-ttu-id="8883c-166">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="8883c-166">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="8883c-167">Коллекция Многозначный расширенные свойства для папки задач.</span><span class="sxs-lookup"><span data-stu-id="8883c-167">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="8883c-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8883c-168">Read-only.</span></span> <span data-ttu-id="8883c-169">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="8883c-169">Nullable.</span></span>|
|<span data-ttu-id="8883c-170">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="8883c-170">singleValueExtendedProperties</span></span>|<span data-ttu-id="8883c-171">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="8883c-171">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="8883c-172">Коллекция расширенные свойства одно значение, определенное для папки задач.</span><span class="sxs-lookup"><span data-stu-id="8883c-172">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="8883c-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8883c-173">Read-only.</span></span> <span data-ttu-id="8883c-174">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="8883c-174">Nullable.</span></span>|
|<span data-ttu-id="8883c-175">tasks</span><span class="sxs-lookup"><span data-stu-id="8883c-175">tasks</span></span>|<span data-ttu-id="8883c-176">[outlookTask](outlooktask.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8883c-176">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="8883c-177">Задачи в этой папке задач.</span><span class="sxs-lookup"><span data-stu-id="8883c-177">The tasks in this task folder.</span></span> <span data-ttu-id="8883c-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8883c-178">Read-only.</span></span> <span data-ttu-id="8883c-179">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="8883c-179">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8883c-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8883c-180">JSON representation</span></span>
<span data-ttu-id="8883c-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8883c-181">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->