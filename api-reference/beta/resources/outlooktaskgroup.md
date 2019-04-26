---
title: Тип ресурса outlookTaskGroup
description: 'Группа папок (outlookTaskFolder), которая содержит задачи Outlook (Коллекция объектов outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 486261d80b8faad7a5969f8f1ce198479e39583c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568618"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="dad15-103">Тип ресурса outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="dad15-103">outlookTaskGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dad15-104">Группа папок ([outlookTaskFolder](outlooktaskfolder.md)), которая содержит задачи Outlook (Коллекция объектов [outlookTask](outlooktask.md) ).</span><span class="sxs-lookup"><span data-stu-id="dad15-104">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="dad15-105">В Outlook существует группа `My Tasks` задач по умолчанию, которую нельзя переименовать или удалить.</span><span class="sxs-lookup"><span data-stu-id="dad15-105">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="dad15-106">Тем не менее, вы можете создать дополнительные группы задач.</span><span class="sxs-lookup"><span data-stu-id="dad15-106">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="dad15-107">Методы</span><span class="sxs-lookup"><span data-stu-id="dad15-107">Methods</span></span>

| <span data-ttu-id="dad15-108">Метод</span><span class="sxs-lookup"><span data-stu-id="dad15-108">Method</span></span>           | <span data-ttu-id="dad15-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dad15-109">Return Type</span></span>    |<span data-ttu-id="dad15-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dad15-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dad15-111">Получение outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="dad15-111">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="dad15-112">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="dad15-112">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="dad15-113">Получение свойств и связей указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="dad15-113">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="dad15-114">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="dad15-114">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="dad15-115">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="dad15-115">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="dad15-116">Создайте папку задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="dad15-116">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="dad15-117">Список Таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="dad15-117">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="dad15-118">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="dad15-118">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="dad15-119">Получение коллекции папок задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="dad15-119">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="dad15-120">Обновление</span><span class="sxs-lookup"><span data-stu-id="dad15-120">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="dad15-121">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="dad15-121">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="dad15-122">Обновление свойств, доступных для записи, для группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="dad15-122">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="dad15-123">Удаление</span><span class="sxs-lookup"><span data-stu-id="dad15-123">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="dad15-124">Нет</span><span class="sxs-lookup"><span data-stu-id="dad15-124">None</span></span> |<span data-ttu-id="dad15-125">Удаление указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="dad15-125">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="dad15-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="dad15-126">Properties</span></span>
| <span data-ttu-id="dad15-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="dad15-127">Property</span></span>     | <span data-ttu-id="dad15-128">Тип</span><span class="sxs-lookup"><span data-stu-id="dad15-128">Type</span></span>   |<span data-ttu-id="dad15-129">Описание</span><span class="sxs-lookup"><span data-stu-id="dad15-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dad15-130">changeKey</span><span class="sxs-lookup"><span data-stu-id="dad15-130">changeKey</span></span>|<span data-ttu-id="dad15-131">String</span><span class="sxs-lookup"><span data-stu-id="dad15-131">String</span></span>|<span data-ttu-id="dad15-132">Версия группы задач.</span><span class="sxs-lookup"><span data-stu-id="dad15-132">The version of the task group.</span></span>|
|<span data-ttu-id="dad15-133">Граупкэй</span><span class="sxs-lookup"><span data-stu-id="dad15-133">groupKey</span></span>|<span data-ttu-id="dad15-134">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="dad15-134">Edm.Guid</span></span>|<span data-ttu-id="dad15-135">Уникальный идентификатор GUID для группы задач.</span><span class="sxs-lookup"><span data-stu-id="dad15-135">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="dad15-136">id</span><span class="sxs-lookup"><span data-stu-id="dad15-136">id</span></span>|<span data-ttu-id="dad15-137">Строка</span><span class="sxs-lookup"><span data-stu-id="dad15-137">String</span></span>|<span data-ttu-id="dad15-138">Уникальный строковый идентификатор группы задач.</span><span class="sxs-lookup"><span data-stu-id="dad15-138">The unique string identifier of the task group.</span></span> <span data-ttu-id="dad15-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dad15-139">Read-only.</span></span>|
|<span data-ttu-id="dad15-140">Исдефаултграуп</span><span class="sxs-lookup"><span data-stu-id="dad15-140">isDefaultGroup</span></span>|<span data-ttu-id="dad15-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="dad15-141">Boolean</span></span>|<span data-ttu-id="dad15-142">Значение true, если группа задач является группой задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dad15-142">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="dad15-143">name</span><span class="sxs-lookup"><span data-stu-id="dad15-143">name</span></span>|<span data-ttu-id="dad15-144">String</span><span class="sxs-lookup"><span data-stu-id="dad15-144">String</span></span>|<span data-ttu-id="dad15-145">Имя группы задач.</span><span class="sxs-lookup"><span data-stu-id="dad15-145">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dad15-146">Связи</span><span class="sxs-lookup"><span data-stu-id="dad15-146">Relationships</span></span>
| <span data-ttu-id="dad15-147">Отношение</span><span class="sxs-lookup"><span data-stu-id="dad15-147">Relationship</span></span> | <span data-ttu-id="dad15-148">Тип</span><span class="sxs-lookup"><span data-stu-id="dad15-148">Type</span></span>   |<span data-ttu-id="dad15-149">Описание</span><span class="sxs-lookup"><span data-stu-id="dad15-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dad15-150">Таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="dad15-150">taskFolders</span></span>|<span data-ttu-id="dad15-151">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="dad15-151">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="dad15-152">Коллекция папок задач в группе задач.</span><span class="sxs-lookup"><span data-stu-id="dad15-152">The collection of task folders in the task group.</span></span> <span data-ttu-id="dad15-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dad15-153">Read-only.</span></span> <span data-ttu-id="dad15-154">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="dad15-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dad15-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dad15-155">JSON representation</span></span>
<span data-ttu-id="dad15-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dad15-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookTaskGroup"
}-->

```json
{
  "changeKey": "String",
  "groupKey": "Guid",
  "id": "String (identifier)",
  "isDefaultGroup": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
