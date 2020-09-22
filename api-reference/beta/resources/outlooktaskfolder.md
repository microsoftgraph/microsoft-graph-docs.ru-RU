---
title: Тип ресурса outlookTaskFolder
description: 'Папка, содержащая задачи Outlook (Коллекция объектов outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c9f9958750cca1aaa40ba9394832e5974bed8cc3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998364"
---
# <a name="outlooktaskfolder-resource-type-deprecated"></a><span data-ttu-id="7f480-103">Тип ресурса outlookTaskFolder (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="7f480-103">outlookTaskFolder resource type (deprecated)</span></span>

<span data-ttu-id="7f480-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f480-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="7f480-105">Папка, содержащая задачи Outlook (Коллекция объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="7f480-105">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="7f480-106">В Outlook группа задач по умолчанию, `My Tasks` которая содержит папку задач по умолчанию, `Tasks` для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="7f480-106">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="7f480-107">Вы не можете переименовывать или удалять эти группы задач и папки по умолчанию, но вы можете создавать дополнительные группы задач и папки задач.</span><span class="sxs-lookup"><span data-stu-id="7f480-107">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="7f480-108">Методы</span><span class="sxs-lookup"><span data-stu-id="7f480-108">Methods</span></span>

| <span data-ttu-id="7f480-109">Метод</span><span class="sxs-lookup"><span data-stu-id="7f480-109">Method</span></span>           | <span data-ttu-id="7f480-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7f480-110">Return Type</span></span>    |<span data-ttu-id="7f480-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7f480-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f480-112">Получение outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="7f480-112">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="7f480-113">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="7f480-113">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="7f480-114">Получение свойств и связей указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="7f480-114">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="7f480-115">Создание объекта outlookTask</span><span class="sxs-lookup"><span data-stu-id="7f480-115">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="7f480-116">outlookTask</span><span class="sxs-lookup"><span data-stu-id="7f480-116">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="7f480-117">Создание задачи Outlook в указанной папке задач.</span><span class="sxs-lookup"><span data-stu-id="7f480-117">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="7f480-118">Список задач</span><span class="sxs-lookup"><span data-stu-id="7f480-118">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="7f480-119">Коллекция объектов [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="7f480-119">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="7f480-120">Получение всех задач Outlook в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="7f480-120">Get all the Outlook tasks in the specified folder.</span></span>|
|<span data-ttu-id="7f480-121">[обновление](../api/outlooktaskfolder-update.md).</span><span class="sxs-lookup"><span data-stu-id="7f480-121">[Update](../api/outlooktaskfolder-update.md)</span></span> | [<span data-ttu-id="7f480-122">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="7f480-122">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="7f480-123">Обновление свойств, доступных для записи, папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="7f480-123">Update the writable properties of an Outlook task folder.</span></span> |
|<span data-ttu-id="7f480-124">[удаление](../api/outlooktaskfolder-delete.md);</span><span class="sxs-lookup"><span data-stu-id="7f480-124">[Delete](../api/outlooktaskfolder-delete.md)</span></span> | <span data-ttu-id="7f480-125">Нет</span><span class="sxs-lookup"><span data-stu-id="7f480-125">None</span></span> |<span data-ttu-id="7f480-126">Удаление указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="7f480-126">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="7f480-127">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="7f480-127">**Extended properties**</span></span>| | |
|[<span data-ttu-id="7f480-128">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="7f480-128">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="7f480-129">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="7f480-129">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="7f480-130">Создайте одно или несколько расширенных свойств с одним значением в новой или существующей папке задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="7f480-130">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="7f480-131">Получение папки задач с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="7f480-131">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="7f480-132">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="7f480-132">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="7f480-133">Получение папок задач Outlook, которые содержат расширенное свойство с одним значением, с помощью `$expand` или `$filter` .</span><span class="sxs-lookup"><span data-stu-id="7f480-133">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="7f480-134">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="7f480-134">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="7f480-135">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="7f480-135">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="7f480-136">Создайте одно или несколько расширенных свойств с несколькими значениями в новой или существующей папке задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="7f480-136">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="7f480-137">Получение папки задач с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="7f480-137">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="7f480-138">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="7f480-138">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="7f480-139">Получение папки задач Outlook, которая содержит расширенное свойство с несколькими значениями, с помощью `$expand` .</span><span class="sxs-lookup"><span data-stu-id="7f480-139">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="7f480-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f480-140">Properties</span></span>
| <span data-ttu-id="7f480-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f480-141">Property</span></span>     | <span data-ttu-id="7f480-142">Тип</span><span class="sxs-lookup"><span data-stu-id="7f480-142">Type</span></span>   |<span data-ttu-id="7f480-143">Описание</span><span class="sxs-lookup"><span data-stu-id="7f480-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f480-144">changeKey</span><span class="sxs-lookup"><span data-stu-id="7f480-144">changeKey</span></span>|<span data-ttu-id="7f480-145">String</span><span class="sxs-lookup"><span data-stu-id="7f480-145">String</span></span>|<span data-ttu-id="7f480-146">Версия папки задач.</span><span class="sxs-lookup"><span data-stu-id="7f480-146">The version of the task folder.</span></span>|
|<span data-ttu-id="7f480-147">id</span><span class="sxs-lookup"><span data-stu-id="7f480-147">id</span></span>|<span data-ttu-id="7f480-148">String</span><span class="sxs-lookup"><span data-stu-id="7f480-148">String</span></span>|<span data-ttu-id="7f480-149">Идентификатор папки задач, уникальный в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="7f480-149">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="7f480-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f480-150">Read-only.</span></span>|
|<span data-ttu-id="7f480-151">исдефаултфолдер</span><span class="sxs-lookup"><span data-stu-id="7f480-151">isDefaultFolder</span></span>|<span data-ttu-id="7f480-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f480-152">Boolean</span></span>|<span data-ttu-id="7f480-153">Значение true, если папка является папкой задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7f480-153">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="7f480-154">name</span><span class="sxs-lookup"><span data-stu-id="7f480-154">name</span></span>|<span data-ttu-id="7f480-155">String</span><span class="sxs-lookup"><span data-stu-id="7f480-155">String</span></span>|<span data-ttu-id="7f480-156">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="7f480-156">The name of the task folder.</span></span>|
|<span data-ttu-id="7f480-157">парентграупкэй</span><span class="sxs-lookup"><span data-stu-id="7f480-157">parentGroupKey</span></span>|<span data-ttu-id="7f480-158">Guid</span><span class="sxs-lookup"><span data-stu-id="7f480-158">Guid</span></span>|<span data-ttu-id="7f480-159">Уникальный идентификатор GUID родительской группы папок задач.</span><span class="sxs-lookup"><span data-stu-id="7f480-159">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f480-160">Связи</span><span class="sxs-lookup"><span data-stu-id="7f480-160">Relationships</span></span>
| <span data-ttu-id="7f480-161">Связь</span><span class="sxs-lookup"><span data-stu-id="7f480-161">Relationship</span></span> | <span data-ttu-id="7f480-162">Тип</span><span class="sxs-lookup"><span data-stu-id="7f480-162">Type</span></span>   |<span data-ttu-id="7f480-163">Описание</span><span class="sxs-lookup"><span data-stu-id="7f480-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f480-164">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="7f480-164">multiValueExtendedProperties</span></span>|<span data-ttu-id="7f480-165">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="7f480-165">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="7f480-166">Коллекция расширенных свойств с несколькими значениями, определенных для папки задач.</span><span class="sxs-lookup"><span data-stu-id="7f480-166">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="7f480-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f480-167">Read-only.</span></span> <span data-ttu-id="7f480-168">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7f480-168">Nullable.</span></span>|
|<span data-ttu-id="7f480-169">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="7f480-169">singleValueExtendedProperties</span></span>|<span data-ttu-id="7f480-170">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="7f480-170">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="7f480-171">Коллекция расширенных свойств с одним значением, определенных для папки задач.</span><span class="sxs-lookup"><span data-stu-id="7f480-171">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="7f480-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f480-172">Read-only.</span></span> <span data-ttu-id="7f480-173">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7f480-173">Nullable.</span></span>|
|<span data-ttu-id="7f480-174">tasks</span><span class="sxs-lookup"><span data-stu-id="7f480-174">tasks</span></span>|<span data-ttu-id="7f480-175">Коллекция объектов [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="7f480-175">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="7f480-176">Задачи в этой папке задач.</span><span class="sxs-lookup"><span data-stu-id="7f480-176">The tasks in this task folder.</span></span> <span data-ttu-id="7f480-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f480-177">Read-only.</span></span> <span data-ttu-id="7f480-178">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7f480-178">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f480-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f480-179">JSON representation</span></span>
<span data-ttu-id="7f480-180">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f480-180">Here is a JSON representation of the resource.</span></span>

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


