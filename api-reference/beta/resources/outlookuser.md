---
title: Тип ресурса outlookUser
description: Представляет службы Outlook, доступные пользователю.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2c23cccabcea33b8cdaacba6ae9abede456c5c99
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009267"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="71037-103">Тип ресурса outlookUser</span><span class="sxs-lookup"><span data-stu-id="71037-103">outlookUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71037-104">Представляет службы Outlook, доступные пользователю.</span><span class="sxs-lookup"><span data-stu-id="71037-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="71037-105">Методы</span><span class="sxs-lookup"><span data-stu-id="71037-105">Methods</span></span>

| <span data-ttu-id="71037-106">Метод</span><span class="sxs-lookup"><span data-stu-id="71037-106">Method</span></span>           | <span data-ttu-id="71037-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="71037-107">Return Type</span></span>    |<span data-ttu-id="71037-108">Описание</span><span class="sxs-lookup"><span data-stu-id="71037-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="71037-109">Создание категории</span><span class="sxs-lookup"><span data-stu-id="71037-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="71037-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="71037-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="71037-111">Создание объекта **outlookCategory** в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="71037-112">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="71037-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="71037-113">Коллекция [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="71037-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="71037-114">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="71037-115">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="71037-115">Create outlookTaskFolder</span></span>](../api/outlookuser-post-taskfolders.md) |[<span data-ttu-id="71037-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="71037-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="71037-117">Создайте папку задач в группе задач по умолчанию (`My Tasks`) почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-117">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|[<span data-ttu-id="71037-118">Список Таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="71037-118">List taskFolders</span></span>](../api/outlookuser-list-taskfolders.md) |<span data-ttu-id="71037-119">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="71037-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="71037-120">Получение всех папок задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-120">Get all the Outlook task folders in the user's mailbox.</span></span>|
|[<span data-ttu-id="71037-121">Создание outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="71037-121">Create outlookTaskGroup</span></span>](../api/outlookuser-post-taskgroups.md) |[<span data-ttu-id="71037-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="71037-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="71037-123">Создайте группу задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-123">Create an Outlook task group in the user's mailbox.</span></span>|
|[<span data-ttu-id="71037-124">Список taskGroups</span><span class="sxs-lookup"><span data-stu-id="71037-124">List taskGroups</span></span>](../api/outlookuser-list-taskgroups.md) |<span data-ttu-id="71037-125">Коллекция [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="71037-125">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="71037-126">Получение всех групп задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-126">Get all the Outlook task groups in the user's mailbox.</span></span>|
|[<span data-ttu-id="71037-127">Создание outlookTask</span><span class="sxs-lookup"><span data-stu-id="71037-127">Create outlookTask</span></span>](../api/outlookuser-post-tasks.md) |[<span data-ttu-id="71037-128">outlookTask</span><span class="sxs-lookup"><span data-stu-id="71037-128">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="71037-129">Создайте задачу Outlook в группе задач по умолчанию (`My Tasks`) и папке задач по умолчанию (`Tasks`) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-129">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|[<span data-ttu-id="71037-130">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="71037-130">List tasks</span></span>](../api/outlookuser-list-tasks.md) |<span data-ttu-id="71037-131">Коллекция [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="71037-131">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="71037-132">Получение всех задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-132">Get all the Outlook tasks in the user's mailbox.</span></span>|
|[<span data-ttu-id="71037-133">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="71037-133">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="71037-134">Коллекция [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="71037-134">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="71037-135">Получение списка языковых стандартов и языков, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-135">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="71037-136">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="71037-136">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="71037-137">Коллекция [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="71037-137">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="71037-138">Получение списка часовых поясов, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-138">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="71037-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="71037-139">Properties</span></span>
<span data-ttu-id="71037-140">Нет</span><span class="sxs-lookup"><span data-stu-id="71037-140">None</span></span>

## <a name="relationships"></a><span data-ttu-id="71037-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="71037-141">Relationships</span></span>
| <span data-ttu-id="71037-142">Отношение</span><span class="sxs-lookup"><span data-stu-id="71037-142">Relationship</span></span> | <span data-ttu-id="71037-143">Тип</span><span class="sxs-lookup"><span data-stu-id="71037-143">Type</span></span>   |<span data-ttu-id="71037-144">Описание</span><span class="sxs-lookup"><span data-stu-id="71037-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71037-145">masterCategories</span><span class="sxs-lookup"><span data-stu-id="71037-145">masterCategories</span></span>|<span data-ttu-id="71037-146">Коллекция [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="71037-146">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="71037-147">Список категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-147">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="71037-148">Таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="71037-148">taskFolders</span></span>|<span data-ttu-id="71037-149">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="71037-149">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="71037-150">Папки задач Outlook пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-150">The user's Outlook task folders.</span></span> <span data-ttu-id="71037-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="71037-151">Read-only.</span></span> <span data-ttu-id="71037-152">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="71037-152">Nullable.</span></span>|
|<span data-ttu-id="71037-153">taskGroups</span><span class="sxs-lookup"><span data-stu-id="71037-153">taskGroups</span></span>|<span data-ttu-id="71037-154">Коллекция [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="71037-154">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="71037-155">Группы задач Outlook пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-155">The user's Outlook task groups.</span></span> <span data-ttu-id="71037-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="71037-156">Read-only.</span></span> <span data-ttu-id="71037-157">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="71037-157">Nullable.</span></span>|
|<span data-ttu-id="71037-158">tasks</span><span class="sxs-lookup"><span data-stu-id="71037-158">tasks</span></span>|<span data-ttu-id="71037-159">Коллекция [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="71037-159">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="71037-160">Задачи Outlook пользователя.</span><span class="sxs-lookup"><span data-stu-id="71037-160">The user's Outlook tasks.</span></span> <span data-ttu-id="71037-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="71037-161">Read-only.</span></span> <span data-ttu-id="71037-162">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="71037-162">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71037-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71037-163">JSON representation</span></span>

<span data-ttu-id="71037-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71037-164">Here is a JSON representation of the resource</span></span>

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
