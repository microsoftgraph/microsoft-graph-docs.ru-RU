---
title: Тип ресурса outlookUser
description: Представляет службы Outlook, доступные пользователю.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d4b83144384eb265c08f3586a0b3a573375248c3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463205"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="4f80b-103">Тип ресурса outlookUser</span><span class="sxs-lookup"><span data-stu-id="4f80b-103">outlookUser resource type</span></span>

<span data-ttu-id="4f80b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f80b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f80b-105">Представляет службы Outlook, доступные пользователю.</span><span class="sxs-lookup"><span data-stu-id="4f80b-105">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="4f80b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4f80b-106">Methods</span></span>

| <span data-ttu-id="4f80b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4f80b-107">Method</span></span>           | <span data-ttu-id="4f80b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4f80b-108">Return Type</span></span>    |<span data-ttu-id="4f80b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4f80b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4f80b-110">Создание категории</span><span class="sxs-lookup"><span data-stu-id="4f80b-110">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="4f80b-111">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="4f80b-111">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="4f80b-112">Создание объекта **outlookCategory** в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-112">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="4f80b-113">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="4f80b-113">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="4f80b-114">Коллекция [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="4f80b-114">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="4f80b-115">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-115">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="4f80b-116">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="4f80b-116">Create outlookTaskFolder</span></span>](../api/outlookuser-post-taskfolders.md) |[<span data-ttu-id="4f80b-117">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="4f80b-117">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="4f80b-118">Создайте папку задач в группе задач по умолчанию (`My Tasks`) почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-118">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|[<span data-ttu-id="4f80b-119">Список Таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="4f80b-119">List taskFolders</span></span>](../api/outlookuser-list-taskfolders.md) |<span data-ttu-id="4f80b-120">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="4f80b-120">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="4f80b-121">Получение всех папок задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-121">Get all the Outlook task folders in the user's mailbox.</span></span>|
|[<span data-ttu-id="4f80b-122">Создание outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="4f80b-122">Create outlookTaskGroup</span></span>](../api/outlookuser-post-taskgroups.md) |[<span data-ttu-id="4f80b-123">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="4f80b-123">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="4f80b-124">Создайте группу задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-124">Create an Outlook task group in the user's mailbox.</span></span>|
|[<span data-ttu-id="4f80b-125">Список taskGroups</span><span class="sxs-lookup"><span data-stu-id="4f80b-125">List taskGroups</span></span>](../api/outlookuser-list-taskgroups.md) |<span data-ttu-id="4f80b-126">Коллекция [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="4f80b-126">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="4f80b-127">Получение всех групп задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-127">Get all the Outlook task groups in the user's mailbox.</span></span>|
|[<span data-ttu-id="4f80b-128">Создание объекта outlookTask</span><span class="sxs-lookup"><span data-stu-id="4f80b-128">Create outlookTask</span></span>](../api/outlookuser-post-tasks.md) |[<span data-ttu-id="4f80b-129">outlookTask</span><span class="sxs-lookup"><span data-stu-id="4f80b-129">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="4f80b-130">Создайте задачу Outlook в группе задач по умолчанию (`My Tasks`) и папке задач по умолчанию (`Tasks`) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-130">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|[<span data-ttu-id="4f80b-131">Список задач</span><span class="sxs-lookup"><span data-stu-id="4f80b-131">List tasks</span></span>](../api/outlookuser-list-tasks.md) |<span data-ttu-id="4f80b-132">Коллекция объектов [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="4f80b-132">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="4f80b-133">Получение всех задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-133">Get all the Outlook tasks in the user's mailbox.</span></span>|
|[<span data-ttu-id="4f80b-134">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="4f80b-134">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="4f80b-135">Коллекция [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="4f80b-135">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="4f80b-136">Получение списка языковых стандартов и языков, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-136">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="4f80b-137">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="4f80b-137">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="4f80b-138">Коллекция [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="4f80b-138">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="4f80b-139">Получение списка часовых поясов, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-139">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="4f80b-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f80b-140">Properties</span></span>
<span data-ttu-id="4f80b-141">Нет</span><span class="sxs-lookup"><span data-stu-id="4f80b-141">None</span></span>

## <a name="relationships"></a><span data-ttu-id="4f80b-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="4f80b-142">Relationships</span></span>
| <span data-ttu-id="4f80b-143">Связь</span><span class="sxs-lookup"><span data-stu-id="4f80b-143">Relationship</span></span> | <span data-ttu-id="4f80b-144">Тип</span><span class="sxs-lookup"><span data-stu-id="4f80b-144">Type</span></span>   |<span data-ttu-id="4f80b-145">Описание</span><span class="sxs-lookup"><span data-stu-id="4f80b-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f80b-146">masterCategories</span><span class="sxs-lookup"><span data-stu-id="4f80b-146">masterCategories</span></span>|<span data-ttu-id="4f80b-147">Коллекция [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="4f80b-147">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="4f80b-148">Список категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-148">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="4f80b-149">таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="4f80b-149">taskFolders</span></span>|<span data-ttu-id="4f80b-150">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="4f80b-150">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="4f80b-151">Папки задач Outlook пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-151">The user's Outlook task folders.</span></span> <span data-ttu-id="4f80b-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f80b-152">Read-only.</span></span> <span data-ttu-id="4f80b-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4f80b-153">Nullable.</span></span>|
|<span data-ttu-id="4f80b-154">taskGroups</span><span class="sxs-lookup"><span data-stu-id="4f80b-154">taskGroups</span></span>|<span data-ttu-id="4f80b-155">Коллекция [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="4f80b-155">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="4f80b-156">Группы задач Outlook пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-156">The user's Outlook task groups.</span></span> <span data-ttu-id="4f80b-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f80b-157">Read-only.</span></span> <span data-ttu-id="4f80b-158">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4f80b-158">Nullable.</span></span>|
|<span data-ttu-id="4f80b-159">tasks</span><span class="sxs-lookup"><span data-stu-id="4f80b-159">tasks</span></span>|<span data-ttu-id="4f80b-160">Коллекция объектов [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="4f80b-160">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="4f80b-161">Задачи Outlook пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f80b-161">The user's Outlook tasks.</span></span> <span data-ttu-id="4f80b-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f80b-162">Read-only.</span></span> <span data-ttu-id="4f80b-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4f80b-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f80b-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f80b-164">JSON representation</span></span>

<span data-ttu-id="4f80b-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f80b-165">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookUser"
}-->
```json
{  
    "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
