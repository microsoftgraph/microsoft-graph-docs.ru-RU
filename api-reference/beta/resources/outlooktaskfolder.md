---
title: Тип ресурса outlookTaskFolder
description: 'Папка, содержащая задачи Outlook (Коллекция объектов outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: eb61936b9ede67d35127db07c92ba8b7517fe623
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568621"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="497e0-103">Тип ресурса outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="497e0-103">outlookTaskFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="497e0-104">Папка, содержащая задачи Outlook (Коллекция объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="497e0-104">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="497e0-105">В Outlook группа `My Tasks`задач по умолчанию, которая содержит папку `Tasks`задач по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="497e0-105">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="497e0-106">Вы не можете переименовывать или удалять эти группы задач и папки по умолчанию, но вы можете создавать дополнительные группы задач и папки задач.</span><span class="sxs-lookup"><span data-stu-id="497e0-106">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="497e0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="497e0-107">Methods</span></span>

| <span data-ttu-id="497e0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="497e0-108">Method</span></span>           | <span data-ttu-id="497e0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="497e0-109">Return Type</span></span>    |<span data-ttu-id="497e0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="497e0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="497e0-111">Получение outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="497e0-111">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="497e0-112">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="497e0-112">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="497e0-113">Получение свойств и связей указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="497e0-113">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="497e0-114">Создание outlookTask</span><span class="sxs-lookup"><span data-stu-id="497e0-114">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="497e0-115">outlookTask</span><span class="sxs-lookup"><span data-stu-id="497e0-115">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="497e0-116">Создание задачи Outlook в указанной папке задач.</span><span class="sxs-lookup"><span data-stu-id="497e0-116">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="497e0-117">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="497e0-117">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="497e0-118">Коллекция [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="497e0-118">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="497e0-119">Получение всех задач Outlook в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="497e0-119">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="497e0-120">Обновление</span><span class="sxs-lookup"><span data-stu-id="497e0-120">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="497e0-121">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="497e0-121">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="497e0-122">Обновление свойств, доступных для записи, папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="497e0-122">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="497e0-123">Удаление</span><span class="sxs-lookup"><span data-stu-id="497e0-123">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="497e0-124">Нет</span><span class="sxs-lookup"><span data-stu-id="497e0-124">None</span></span> |<span data-ttu-id="497e0-125">Удаление указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="497e0-125">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="497e0-126">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="497e0-126">**Extended properties**</span></span>| | |
|[<span data-ttu-id="497e0-127">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="497e0-127">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="497e0-128">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="497e0-128">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="497e0-129">Создайте одно или несколько расширенных свойств с одним значением в новой или существующей папке задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="497e0-129">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="497e0-130">Получение папки задач с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="497e0-130">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="497e0-131">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="497e0-131">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="497e0-132">Получение папок задач Outlook, которые содержат расширенное свойство с одним значением, `$expand` с `$filter`помощью или.</span><span class="sxs-lookup"><span data-stu-id="497e0-132">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="497e0-133">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="497e0-133">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="497e0-134">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="497e0-134">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="497e0-135">Создайте одно или несколько расширенных свойств с несколькими значениями в новой или существующей папке задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="497e0-135">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="497e0-136">Получение папки задач с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="497e0-136">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="497e0-137">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="497e0-137">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="497e0-138">Получение папки задач Outlook, которая содержит расширенное свойство с несколькими значениями, с `$expand`помощью.</span><span class="sxs-lookup"><span data-stu-id="497e0-138">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="497e0-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="497e0-139">Properties</span></span>
| <span data-ttu-id="497e0-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="497e0-140">Property</span></span>     | <span data-ttu-id="497e0-141">Тип</span><span class="sxs-lookup"><span data-stu-id="497e0-141">Type</span></span>   |<span data-ttu-id="497e0-142">Описание</span><span class="sxs-lookup"><span data-stu-id="497e0-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="497e0-143">changeKey</span><span class="sxs-lookup"><span data-stu-id="497e0-143">changeKey</span></span>|<span data-ttu-id="497e0-144">String</span><span class="sxs-lookup"><span data-stu-id="497e0-144">String</span></span>|<span data-ttu-id="497e0-145">Версия папки задач.</span><span class="sxs-lookup"><span data-stu-id="497e0-145">The version of the task folder.</span></span>|
|<span data-ttu-id="497e0-146">id</span><span class="sxs-lookup"><span data-stu-id="497e0-146">id</span></span>|<span data-ttu-id="497e0-147">Строка</span><span class="sxs-lookup"><span data-stu-id="497e0-147">String</span></span>|<span data-ttu-id="497e0-148">Идентификатор папки задач, уникальный в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="497e0-148">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="497e0-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="497e0-149">Read-only.</span></span>|
|<span data-ttu-id="497e0-150">Исдефаултфолдер</span><span class="sxs-lookup"><span data-stu-id="497e0-150">isDefaultFolder</span></span>|<span data-ttu-id="497e0-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="497e0-151">Boolean</span></span>|<span data-ttu-id="497e0-152">Значение true, если папка является папкой задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="497e0-152">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="497e0-153">name</span><span class="sxs-lookup"><span data-stu-id="497e0-153">name</span></span>|<span data-ttu-id="497e0-154">String</span><span class="sxs-lookup"><span data-stu-id="497e0-154">String</span></span>|<span data-ttu-id="497e0-155">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="497e0-155">The name of the task folder.</span></span>|
|<span data-ttu-id="497e0-156">Парентграупкэй</span><span class="sxs-lookup"><span data-stu-id="497e0-156">parentGroupKey</span></span>|<span data-ttu-id="497e0-157">Guid</span><span class="sxs-lookup"><span data-stu-id="497e0-157">Guid</span></span>|<span data-ttu-id="497e0-158">Уникальный идентификатор GUID родительской группы папок задач.</span><span class="sxs-lookup"><span data-stu-id="497e0-158">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="497e0-159">Связи</span><span class="sxs-lookup"><span data-stu-id="497e0-159">Relationships</span></span>
| <span data-ttu-id="497e0-160">Отношение</span><span class="sxs-lookup"><span data-stu-id="497e0-160">Relationship</span></span> | <span data-ttu-id="497e0-161">Тип</span><span class="sxs-lookup"><span data-stu-id="497e0-161">Type</span></span>   |<span data-ttu-id="497e0-162">Описание</span><span class="sxs-lookup"><span data-stu-id="497e0-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="497e0-163">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="497e0-163">multiValueExtendedProperties</span></span>|<span data-ttu-id="497e0-164">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="497e0-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="497e0-165">Коллекция расширенных свойств с несколькими значениями, определенных для папки задач.</span><span class="sxs-lookup"><span data-stu-id="497e0-165">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="497e0-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="497e0-166">Read-only.</span></span> <span data-ttu-id="497e0-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="497e0-167">Nullable.</span></span>|
|<span data-ttu-id="497e0-168">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="497e0-168">singleValueExtendedProperties</span></span>|<span data-ttu-id="497e0-169">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="497e0-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="497e0-170">Коллекция расширенных свойств с одним значением, определенных для папки задач.</span><span class="sxs-lookup"><span data-stu-id="497e0-170">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="497e0-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="497e0-171">Read-only.</span></span> <span data-ttu-id="497e0-172">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="497e0-172">Nullable.</span></span>|
|<span data-ttu-id="497e0-173">tasks</span><span class="sxs-lookup"><span data-stu-id="497e0-173">tasks</span></span>|<span data-ttu-id="497e0-174">Коллекция [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="497e0-174">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="497e0-175">Задачи в этой папке задач.</span><span class="sxs-lookup"><span data-stu-id="497e0-175">The tasks in this task folder.</span></span> <span data-ttu-id="497e0-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="497e0-176">Read-only.</span></span> <span data-ttu-id="497e0-177">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="497e0-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="497e0-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="497e0-178">JSON representation</span></span>
<span data-ttu-id="497e0-179">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="497e0-179">Here is a JSON representation of the resource.</span></span>

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
