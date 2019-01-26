---
title: Тип ресурса outlookUser
description: Представляет службы Outlook, доступные пользователю.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f8265f9da285ce0f52e6201ffdb1298893b86753
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574098"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="eb2a6-103">Тип ресурса outlookUser</span><span class="sxs-lookup"><span data-stu-id="eb2a6-103">outlookUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb2a6-104">Представляет службы Outlook, доступные пользователю.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="eb2a6-105">Методы</span><span class="sxs-lookup"><span data-stu-id="eb2a6-105">Methods</span></span>

| <span data-ttu-id="eb2a6-106">Метод</span><span class="sxs-lookup"><span data-stu-id="eb2a6-106">Method</span></span>           | <span data-ttu-id="eb2a6-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eb2a6-107">Return Type</span></span>    |<span data-ttu-id="eb2a6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="eb2a6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eb2a6-109">Создание категории</span><span class="sxs-lookup"><span data-stu-id="eb2a6-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="eb2a6-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="eb2a6-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="eb2a6-111">Создание объекта **outlookCategory** в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="eb2a6-112">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="eb2a6-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="eb2a6-113">Коллекция [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="eb2a6-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="eb2a6-114">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="eb2a6-115">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="eb2a6-115">Create outlookTaskFolder</span></span>](../api/outlookuser-post-taskfolders.md) |[<span data-ttu-id="eb2a6-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="eb2a6-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="eb2a6-117">Создайте папку задачи в группе задач по умолчанию (`My Tasks`) из почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-117">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|[<span data-ttu-id="eb2a6-118">Список taskFolders</span><span class="sxs-lookup"><span data-stu-id="eb2a6-118">List taskFolders</span></span>](../api/outlookuser-list-taskfolders.md) |<span data-ttu-id="eb2a6-119">[outlookTaskFolder](outlooktaskfolder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="eb2a6-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="eb2a6-120">Получите все папки задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-120">Get all the Outlook task folders in the user's mailbox.</span></span>|
|[<span data-ttu-id="eb2a6-121">Создание outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="eb2a6-121">Create outlookTaskGroup</span></span>](../api/outlookuser-post-taskgroups.md) |[<span data-ttu-id="eb2a6-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="eb2a6-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="eb2a6-123">Создайте группу задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-123">Create an Outlook task group in the user's mailbox.</span></span>|
|[<span data-ttu-id="eb2a6-124">Список taskGroups</span><span class="sxs-lookup"><span data-stu-id="eb2a6-124">List taskGroups</span></span>](../api/outlookuser-list-taskgroups.md) |<span data-ttu-id="eb2a6-125">[outlookTaskGroup](outlooktaskgroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="eb2a6-125">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="eb2a6-126">Получение всех групп задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-126">Get all the Outlook task groups in the user's mailbox.</span></span>|
|[<span data-ttu-id="eb2a6-127">Создание outlookTask</span><span class="sxs-lookup"><span data-stu-id="eb2a6-127">Create outlookTask</span></span>](../api/outlookuser-post-tasks.md) |[<span data-ttu-id="eb2a6-128">outlookTask</span><span class="sxs-lookup"><span data-stu-id="eb2a6-128">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="eb2a6-129">Создание задачи Outlook в группе задач по умолчанию (`My Tasks`) и папки задач по умолчанию (`Tasks`) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-129">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|[<span data-ttu-id="eb2a6-130">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="eb2a6-130">List tasks</span></span>](../api/outlookuser-list-tasks.md) |<span data-ttu-id="eb2a6-131">[outlookTask](outlooktask.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="eb2a6-131">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="eb2a6-132">Получите все задачи Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-132">Get all the Outlook tasks in the user's mailbox.</span></span>|
|[<span data-ttu-id="eb2a6-133">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="eb2a6-133">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="eb2a6-134">Коллекция [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="eb2a6-134">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="eb2a6-135">Получение списка языковых стандартов и языков, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-135">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="eb2a6-136">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="eb2a6-136">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="eb2a6-137">Коллекция [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="eb2a6-137">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="eb2a6-138">Получение списка часовых поясов, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-138">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="eb2a6-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb2a6-139">Properties</span></span>
<span data-ttu-id="eb2a6-140">Нет</span><span class="sxs-lookup"><span data-stu-id="eb2a6-140">None</span></span>

## <a name="relationships"></a><span data-ttu-id="eb2a6-141">Связи</span><span class="sxs-lookup"><span data-stu-id="eb2a6-141">Relationships</span></span>
| <span data-ttu-id="eb2a6-142">Связь</span><span class="sxs-lookup"><span data-stu-id="eb2a6-142">Relationship</span></span> | <span data-ttu-id="eb2a6-143">Тип</span><span class="sxs-lookup"><span data-stu-id="eb2a6-143">Type</span></span>   |<span data-ttu-id="eb2a6-144">Описание</span><span class="sxs-lookup"><span data-stu-id="eb2a6-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb2a6-145">masterCategories</span><span class="sxs-lookup"><span data-stu-id="eb2a6-145">masterCategories</span></span>|<span data-ttu-id="eb2a6-146">Коллекция [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="eb2a6-146">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="eb2a6-147">Список категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-147">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="eb2a6-148">taskFolders</span><span class="sxs-lookup"><span data-stu-id="eb2a6-148">taskFolders</span></span>|<span data-ttu-id="eb2a6-149">[outlookTaskFolder](outlooktaskfolder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="eb2a6-149">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="eb2a6-150">Папки задач Outlook пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-150">The user's Outlook task folders.</span></span> <span data-ttu-id="eb2a6-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-151">Read-only.</span></span> <span data-ttu-id="eb2a6-152">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-152">Nullable.</span></span>|
|<span data-ttu-id="eb2a6-153">taskGroups</span><span class="sxs-lookup"><span data-stu-id="eb2a6-153">taskGroups</span></span>|<span data-ttu-id="eb2a6-154">[outlookTaskGroup](outlooktaskgroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="eb2a6-154">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="eb2a6-155">Группы задач пользователя Outlook.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-155">The user's Outlook task groups.</span></span> <span data-ttu-id="eb2a6-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-156">Read-only.</span></span> <span data-ttu-id="eb2a6-157">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-157">Nullable.</span></span>|
|<span data-ttu-id="eb2a6-158">tasks</span><span class="sxs-lookup"><span data-stu-id="eb2a6-158">tasks</span></span>|<span data-ttu-id="eb2a6-159">[outlookTask](outlooktask.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="eb2a6-159">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="eb2a6-160">Задачи Outlook пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-160">The user's Outlook tasks.</span></span> <span data-ttu-id="eb2a6-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-161">Read-only.</span></span> <span data-ttu-id="eb2a6-162">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="eb2a6-162">Nullable.</span></span>|


<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.outlookUser"
}-->
```json
{
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
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
