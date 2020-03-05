---
title: Тип ресурса outlookTaskFolder
description: 'Папка, содержащая задачи Outlook (Коллекция объектов outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 094c8f9fc6489f081f93d5a6e1ece02857884910
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522083"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="2036e-103">Тип ресурса outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="2036e-103">outlookTaskFolder resource type</span></span>

<span data-ttu-id="2036e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2036e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2036e-105">Папка, содержащая задачи Outlook (Коллекция объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="2036e-105">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="2036e-106">В Outlook группа `My Tasks`задач по умолчанию, которая содержит папку `Tasks`задач по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="2036e-106">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="2036e-107">Вы не можете переименовывать или удалять эти группы задач и папки по умолчанию, но вы можете создавать дополнительные группы задач и папки задач.</span><span class="sxs-lookup"><span data-stu-id="2036e-107">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="2036e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="2036e-108">Methods</span></span>

| <span data-ttu-id="2036e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="2036e-109">Method</span></span>           | <span data-ttu-id="2036e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2036e-110">Return Type</span></span>    |<span data-ttu-id="2036e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2036e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2036e-112">Получение outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="2036e-112">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="2036e-113">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="2036e-113">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="2036e-114">Получение свойств и связей указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="2036e-114">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="2036e-115">Создание объекта outlookTask</span><span class="sxs-lookup"><span data-stu-id="2036e-115">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="2036e-116">outlookTask</span><span class="sxs-lookup"><span data-stu-id="2036e-116">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="2036e-117">Создание задачи Outlook в указанной папке задач.</span><span class="sxs-lookup"><span data-stu-id="2036e-117">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="2036e-118">Список задач</span><span class="sxs-lookup"><span data-stu-id="2036e-118">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="2036e-119">Коллекция объектов [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="2036e-119">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="2036e-120">Получение всех задач Outlook в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="2036e-120">Get all the Outlook tasks in the specified folder.</span></span>|
|<span data-ttu-id="2036e-121">[обновление](../api/outlooktaskfolder-update.md).</span><span class="sxs-lookup"><span data-stu-id="2036e-121">[Update](../api/outlooktaskfolder-update.md)</span></span> | [<span data-ttu-id="2036e-122">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="2036e-122">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="2036e-123">Обновление свойств, доступных для записи, папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="2036e-123">Update the writable properties of an Outlook task folder.</span></span> |
|<span data-ttu-id="2036e-124">[удаление](../api/outlooktaskfolder-delete.md);</span><span class="sxs-lookup"><span data-stu-id="2036e-124">[Delete](../api/outlooktaskfolder-delete.md)</span></span> | <span data-ttu-id="2036e-125">Нет</span><span class="sxs-lookup"><span data-stu-id="2036e-125">None</span></span> |<span data-ttu-id="2036e-126">Удаление указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="2036e-126">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="2036e-127">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="2036e-127">**Extended properties**</span></span>| | |
|[<span data-ttu-id="2036e-128">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="2036e-128">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="2036e-129">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="2036e-129">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="2036e-130">Создайте одно или несколько расширенных свойств с одним значением в новой или существующей папке задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="2036e-130">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="2036e-131">Получение папки задач с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="2036e-131">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="2036e-132">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="2036e-132">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="2036e-133">Получение папок задач Outlook, которые содержат расширенное свойство с одним значением, `$expand` с `$filter`помощью или.</span><span class="sxs-lookup"><span data-stu-id="2036e-133">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="2036e-134">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="2036e-134">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="2036e-135">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="2036e-135">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="2036e-136">Создайте одно или несколько расширенных свойств с несколькими значениями в новой или существующей папке задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="2036e-136">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="2036e-137">Получение папки задач с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="2036e-137">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="2036e-138">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="2036e-138">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="2036e-139">Получение папки задач Outlook, которая содержит расширенное свойство с несколькими значениями, с `$expand`помощью.</span><span class="sxs-lookup"><span data-stu-id="2036e-139">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="2036e-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="2036e-140">Properties</span></span>
| <span data-ttu-id="2036e-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="2036e-141">Property</span></span>     | <span data-ttu-id="2036e-142">Тип</span><span class="sxs-lookup"><span data-stu-id="2036e-142">Type</span></span>   |<span data-ttu-id="2036e-143">Описание</span><span class="sxs-lookup"><span data-stu-id="2036e-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2036e-144">changeKey</span><span class="sxs-lookup"><span data-stu-id="2036e-144">changeKey</span></span>|<span data-ttu-id="2036e-145">String</span><span class="sxs-lookup"><span data-stu-id="2036e-145">String</span></span>|<span data-ttu-id="2036e-146">Версия папки задач.</span><span class="sxs-lookup"><span data-stu-id="2036e-146">The version of the task folder.</span></span>|
|<span data-ttu-id="2036e-147">id</span><span class="sxs-lookup"><span data-stu-id="2036e-147">id</span></span>|<span data-ttu-id="2036e-148">String</span><span class="sxs-lookup"><span data-stu-id="2036e-148">String</span></span>|<span data-ttu-id="2036e-149">Идентификатор папки задач, уникальный в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="2036e-149">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="2036e-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2036e-150">Read-only.</span></span>|
|<span data-ttu-id="2036e-151">исдефаултфолдер</span><span class="sxs-lookup"><span data-stu-id="2036e-151">isDefaultFolder</span></span>|<span data-ttu-id="2036e-152">Логический</span><span class="sxs-lookup"><span data-stu-id="2036e-152">Boolean</span></span>|<span data-ttu-id="2036e-153">Значение true, если папка является папкой задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2036e-153">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="2036e-154">name</span><span class="sxs-lookup"><span data-stu-id="2036e-154">name</span></span>|<span data-ttu-id="2036e-155">String</span><span class="sxs-lookup"><span data-stu-id="2036e-155">String</span></span>|<span data-ttu-id="2036e-156">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="2036e-156">The name of the task folder.</span></span>|
|<span data-ttu-id="2036e-157">парентграупкэй</span><span class="sxs-lookup"><span data-stu-id="2036e-157">parentGroupKey</span></span>|<span data-ttu-id="2036e-158">GUID</span><span class="sxs-lookup"><span data-stu-id="2036e-158">Guid</span></span>|<span data-ttu-id="2036e-159">Уникальный идентификатор GUID родительской группы папок задач.</span><span class="sxs-lookup"><span data-stu-id="2036e-159">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2036e-160">Связи</span><span class="sxs-lookup"><span data-stu-id="2036e-160">Relationships</span></span>
| <span data-ttu-id="2036e-161">Связь</span><span class="sxs-lookup"><span data-stu-id="2036e-161">Relationship</span></span> | <span data-ttu-id="2036e-162">Тип</span><span class="sxs-lookup"><span data-stu-id="2036e-162">Type</span></span>   |<span data-ttu-id="2036e-163">Описание</span><span class="sxs-lookup"><span data-stu-id="2036e-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2036e-164">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="2036e-164">multiValueExtendedProperties</span></span>|<span data-ttu-id="2036e-165">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="2036e-165">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="2036e-166">Коллекция расширенных свойств с несколькими значениями, определенных для папки задач.</span><span class="sxs-lookup"><span data-stu-id="2036e-166">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="2036e-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2036e-167">Read-only.</span></span> <span data-ttu-id="2036e-168">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2036e-168">Nullable.</span></span>|
|<span data-ttu-id="2036e-169">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="2036e-169">singleValueExtendedProperties</span></span>|<span data-ttu-id="2036e-170">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="2036e-170">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="2036e-171">Коллекция расширенных свойств с одним значением, определенных для папки задач.</span><span class="sxs-lookup"><span data-stu-id="2036e-171">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="2036e-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2036e-172">Read-only.</span></span> <span data-ttu-id="2036e-173">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2036e-173">Nullable.</span></span>|
|<span data-ttu-id="2036e-174">tasks</span><span class="sxs-lookup"><span data-stu-id="2036e-174">tasks</span></span>|<span data-ttu-id="2036e-175">Коллекция объектов [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="2036e-175">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="2036e-176">Задачи в этой папке задач.</span><span class="sxs-lookup"><span data-stu-id="2036e-176">The tasks in this task folder.</span></span> <span data-ttu-id="2036e-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2036e-177">Read-only.</span></span> <span data-ttu-id="2036e-178">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2036e-178">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2036e-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2036e-179">JSON representation</span></span>
<span data-ttu-id="2036e-180">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2036e-180">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
  "suppressions": []
}
-->
