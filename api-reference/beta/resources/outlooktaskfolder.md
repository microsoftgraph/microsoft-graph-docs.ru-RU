---
title: Тип ресурса outlookTaskFolder
description: 'Папка, содержащая задачи Outlook (коллекцию объектов outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 4b4c4bade46022b30c6e4e1f50aae58d32656f0b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882931"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="1d458-103">Тип ресурса outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1d458-103">outlookTaskFolder resource type</span></span>

> <span data-ttu-id="1d458-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1d458-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d458-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d458-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d458-106">Папка, содержащая задачи Outlook (коллекцию объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="1d458-106">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="1d458-107">В программе Outlook, группа задач по умолчанию, `My Tasks`, содержащая папки задач по умолчанию, `Tasks`, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d458-107">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="1d458-108">Невозможно переименовать или удалить эти группы по умолчанию задач и папки, но можно создать дополнительные группы задач и папок задач.</span><span class="sxs-lookup"><span data-stu-id="1d458-108">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="1d458-109">Методы</span><span class="sxs-lookup"><span data-stu-id="1d458-109">Methods</span></span>

| <span data-ttu-id="1d458-110">Метод</span><span class="sxs-lookup"><span data-stu-id="1d458-110">Method</span></span>           | <span data-ttu-id="1d458-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1d458-111">Return Type</span></span>    |<span data-ttu-id="1d458-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1d458-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d458-113">Получение outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1d458-113">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="1d458-114">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1d458-114">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="1d458-115">Получите свойства и связи указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="1d458-115">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="1d458-116">Создание outlookTask</span><span class="sxs-lookup"><span data-stu-id="1d458-116">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="1d458-117">outlookTask</span><span class="sxs-lookup"><span data-stu-id="1d458-117">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="1d458-118">Создание задачи Outlook в папке указанной задачи.</span><span class="sxs-lookup"><span data-stu-id="1d458-118">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="1d458-119">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="1d458-119">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="1d458-120">[outlookTask](outlooktask.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1d458-120">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="1d458-121">Получите все задачи Outlook в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="1d458-121">Get all the Outlook tasks in the specified folder.</span></span>|
|<span data-ttu-id="1d458-122">[обновление](../api/outlooktaskfolder-update.md).</span><span class="sxs-lookup"><span data-stu-id="1d458-122">[Update](../api/outlooktaskfolder-update.md)</span></span> | [<span data-ttu-id="1d458-123">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1d458-123">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="1d458-124">Обновление для записи свойств папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="1d458-124">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="1d458-125">Delete</span><span class="sxs-lookup"><span data-stu-id="1d458-125">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="1d458-126">Нет</span><span class="sxs-lookup"><span data-stu-id="1d458-126">None</span></span> |<span data-ttu-id="1d458-127">Удаление указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="1d458-127">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="1d458-128">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="1d458-128">**Extended properties**</span></span>| | |
|[<span data-ttu-id="1d458-129">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="1d458-129">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="1d458-130">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1d458-130">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="1d458-131">Создайте один или несколько расширенных свойств одно значение в новую или существующую папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="1d458-131">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="1d458-132">Получение папки задач с одним значением расширенные свойства</span><span class="sxs-lookup"><span data-stu-id="1d458-132">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="1d458-133">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1d458-133">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="1d458-134">Получение папки задач Outlook, которые содержат одно значение расширенные свойства с помощью `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="1d458-134">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="1d458-135">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="1d458-135">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="1d458-136">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1d458-136">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="1d458-137">Создайте один или несколько расширенных свойств Многозначный в новую или существующую папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="1d458-137">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="1d458-138">Получение папки задач с несколькими значениями расширенные свойства</span><span class="sxs-lookup"><span data-stu-id="1d458-138">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="1d458-139">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1d458-139">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="1d458-140">Получение папки задач Outlook, которая содержит свойство расширенного Многозначный с помощью `$expand`.</span><span class="sxs-lookup"><span data-stu-id="1d458-140">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="1d458-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d458-141">Properties</span></span>
| <span data-ttu-id="1d458-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d458-142">Property</span></span>     | <span data-ttu-id="1d458-143">Тип</span><span class="sxs-lookup"><span data-stu-id="1d458-143">Type</span></span>   |<span data-ttu-id="1d458-144">Описание</span><span class="sxs-lookup"><span data-stu-id="1d458-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d458-145">changeKey</span><span class="sxs-lookup"><span data-stu-id="1d458-145">changeKey</span></span>|<span data-ttu-id="1d458-146">Строка</span><span class="sxs-lookup"><span data-stu-id="1d458-146">String</span></span>|<span data-ttu-id="1d458-147">Версия папки задач.</span><span class="sxs-lookup"><span data-stu-id="1d458-147">The version of the task folder.</span></span>|
|<span data-ttu-id="1d458-148">id</span><span class="sxs-lookup"><span data-stu-id="1d458-148">id</span></span>|<span data-ttu-id="1d458-149">Строка</span><span class="sxs-lookup"><span data-stu-id="1d458-149">String</span></span>|<span data-ttu-id="1d458-150">Идентификатор папки задач, уникальные в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d458-150">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="1d458-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d458-151">Read-only.</span></span>|
|<span data-ttu-id="1d458-152">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="1d458-152">isDefaultFolder</span></span>|<span data-ttu-id="1d458-153">Логический</span><span class="sxs-lookup"><span data-stu-id="1d458-153">Boolean</span></span>|<span data-ttu-id="1d458-154">Значение true, если папка является папки задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1d458-154">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="1d458-155">name</span><span class="sxs-lookup"><span data-stu-id="1d458-155">name</span></span>|<span data-ttu-id="1d458-156">Строка</span><span class="sxs-lookup"><span data-stu-id="1d458-156">String</span></span>|<span data-ttu-id="1d458-157">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="1d458-157">The name of the task folder.</span></span>|
|<span data-ttu-id="1d458-158">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="1d458-158">parentGroupKey</span></span>|<span data-ttu-id="1d458-159">Guid</span><span class="sxs-lookup"><span data-stu-id="1d458-159">Guid</span></span>|<span data-ttu-id="1d458-160">Уникальный идентификатор GUID для родительской папки задач группы.</span><span class="sxs-lookup"><span data-stu-id="1d458-160">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d458-161">Связи</span><span class="sxs-lookup"><span data-stu-id="1d458-161">Relationships</span></span>
| <span data-ttu-id="1d458-162">Связь</span><span class="sxs-lookup"><span data-stu-id="1d458-162">Relationship</span></span> | <span data-ttu-id="1d458-163">Тип</span><span class="sxs-lookup"><span data-stu-id="1d458-163">Type</span></span>   |<span data-ttu-id="1d458-164">Описание</span><span class="sxs-lookup"><span data-stu-id="1d458-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d458-165">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="1d458-165">multiValueExtendedProperties</span></span>|<span data-ttu-id="1d458-166">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="1d458-166">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="1d458-167">Коллекция Многозначный расширенные свойства для папки задач.</span><span class="sxs-lookup"><span data-stu-id="1d458-167">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="1d458-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d458-168">Read-only.</span></span> <span data-ttu-id="1d458-169">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1d458-169">Nullable.</span></span>|
|<span data-ttu-id="1d458-170">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="1d458-170">singleValueExtendedProperties</span></span>|<span data-ttu-id="1d458-171">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="1d458-171">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="1d458-172">Коллекция расширенные свойства одно значение, определенное для папки задач.</span><span class="sxs-lookup"><span data-stu-id="1d458-172">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="1d458-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d458-173">Read-only.</span></span> <span data-ttu-id="1d458-174">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1d458-174">Nullable.</span></span>|
|<span data-ttu-id="1d458-175">tasks</span><span class="sxs-lookup"><span data-stu-id="1d458-175">tasks</span></span>|<span data-ttu-id="1d458-176">[outlookTask](outlooktask.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1d458-176">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="1d458-177">Задачи в этой папке задач.</span><span class="sxs-lookup"><span data-stu-id="1d458-177">The tasks in this task folder.</span></span> <span data-ttu-id="1d458-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d458-178">Read-only.</span></span> <span data-ttu-id="1d458-179">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1d458-179">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d458-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d458-180">JSON representation</span></span>
<span data-ttu-id="1d458-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d458-181">Here is a JSON representation of the resource.</span></span>

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
