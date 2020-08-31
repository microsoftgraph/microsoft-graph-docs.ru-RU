---
title: Тип ресурса outlookUser
description: Представляет службы Outlook, доступные пользователю.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 25aae9eeea7c2bf216ec94ffa2f1ac9654e04d79
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312112"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="55ed4-103">Тип ресурса outlookUser</span><span class="sxs-lookup"><span data-stu-id="55ed4-103">outlookUser resource type</span></span>

<span data-ttu-id="55ed4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55ed4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="55ed4-105">Представляет службы Outlook, доступные пользователю.</span><span class="sxs-lookup"><span data-stu-id="55ed4-105">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="55ed4-106">Методы</span><span class="sxs-lookup"><span data-stu-id="55ed4-106">Methods</span></span>

| <span data-ttu-id="55ed4-107">Метод</span><span class="sxs-lookup"><span data-stu-id="55ed4-107">Method</span></span>           | <span data-ttu-id="55ed4-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="55ed4-108">Return Type</span></span>    |<span data-ttu-id="55ed4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="55ed4-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55ed4-110">Создание категории</span><span class="sxs-lookup"><span data-stu-id="55ed4-110">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="55ed4-111">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="55ed4-111">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="55ed4-112">Создание объекта **outlookCategory** в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-112">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="55ed4-113">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="55ed4-113">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="55ed4-114">Коллекция [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="55ed4-114">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="55ed4-115">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-115">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="55ed4-116">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="55ed4-116">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="55ed4-117">Коллекция [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="55ed4-117">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="55ed4-118">Получение списка языковых стандартов и языков, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-118">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="55ed4-119">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="55ed4-119">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="55ed4-120">Коллекция [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="55ed4-120">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="55ed4-121">Получение списка часовых поясов, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-121">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |
|<span data-ttu-id="55ed4-122">[Создание outlookTaskFolder](../api/outlookuser-post-taskfolders.md) (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="55ed4-122">[Create outlookTaskFolder](../api/outlookuser-post-taskfolders.md) (deprecated)</span></span> |[<span data-ttu-id="55ed4-123">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55ed4-123">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="55ed4-124">Создайте папку задач в группе задач по умолчанию ( `My Tasks` ) почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-124">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|<span data-ttu-id="55ed4-125">[Список таскфолдерс](../api/outlookuser-list-taskfolders.md) (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="55ed4-125">[List taskFolders](../api/outlookuser-list-taskfolders.md) (deprecated)</span></span> |<span data-ttu-id="55ed4-126">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="55ed4-126">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="55ed4-127">Получение всех папок задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-127">Get all the Outlook task folders in the user's mailbox.</span></span>|
|<span data-ttu-id="55ed4-128">[Создание outlookTaskGroup](../api/outlookuser-post-taskgroups.md) (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="55ed4-128">[Create outlookTaskGroup](../api/outlookuser-post-taskgroups.md) (deprecated)</span></span> |[<span data-ttu-id="55ed4-129">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="55ed4-129">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="55ed4-130">Создайте группу задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-130">Create an Outlook task group in the user's mailbox.</span></span>|
|<span data-ttu-id="55ed4-131">[Список taskGroups](../api/outlookuser-list-taskgroups.md) (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="55ed4-131">[List taskGroups](../api/outlookuser-list-taskgroups.md) (deprecated)</span></span> |<span data-ttu-id="55ed4-132">Коллекция [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="55ed4-132">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="55ed4-133">Получение всех групп задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-133">Get all the Outlook task groups in the user's mailbox.</span></span>|
|<span data-ttu-id="55ed4-134">[Создание outlookTask](../api/outlookuser-post-tasks.md) (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="55ed4-134">[Create outlookTask](../api/outlookuser-post-tasks.md) (deprecated)</span></span> |[<span data-ttu-id="55ed4-135">outlookTask</span><span class="sxs-lookup"><span data-stu-id="55ed4-135">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="55ed4-136">Создайте задачу Outlook в группе задач по умолчанию ( `My Tasks` ) и папке задач по умолчанию ( `Tasks` ) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-136">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|<span data-ttu-id="55ed4-137">[Список задач](../api/outlookuser-list-tasks.md) (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="55ed4-137">[List tasks](../api/outlookuser-list-tasks.md) (deprecated)</span></span> |<span data-ttu-id="55ed4-138">Коллекция объектов [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="55ed4-138">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="55ed4-139">Получение всех задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-139">Get all the Outlook tasks in the user's mailbox.</span></span>|



## <a name="properties"></a><span data-ttu-id="55ed4-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="55ed4-140">Properties</span></span>
<span data-ttu-id="55ed4-141">Нет</span><span class="sxs-lookup"><span data-stu-id="55ed4-141">None</span></span>

## <a name="relationships"></a><span data-ttu-id="55ed4-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="55ed4-142">Relationships</span></span>
| <span data-ttu-id="55ed4-143">Связь</span><span class="sxs-lookup"><span data-stu-id="55ed4-143">Relationship</span></span> | <span data-ttu-id="55ed4-144">Тип</span><span class="sxs-lookup"><span data-stu-id="55ed4-144">Type</span></span>   |<span data-ttu-id="55ed4-145">Описание</span><span class="sxs-lookup"><span data-stu-id="55ed4-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55ed4-146">masterCategories</span><span class="sxs-lookup"><span data-stu-id="55ed4-146">masterCategories</span></span>|<span data-ttu-id="55ed4-147">Коллекция [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="55ed4-147">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="55ed4-148">Список категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-148">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="55ed4-149">Таскфолдерс (устаревший)</span><span class="sxs-lookup"><span data-stu-id="55ed4-149">taskFolders (deprecated)</span></span>|<span data-ttu-id="55ed4-150">Коллекция [outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="55ed4-150">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="55ed4-151">Папки задач Outlook пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-151">The user's Outlook task folders.</span></span> <span data-ttu-id="55ed4-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55ed4-152">Read-only.</span></span> <span data-ttu-id="55ed4-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="55ed4-153">Nullable.</span></span>|
|<span data-ttu-id="55ed4-154">taskGroups (устаревший)</span><span class="sxs-lookup"><span data-stu-id="55ed4-154">taskGroups (deprecated)</span></span>|<span data-ttu-id="55ed4-155">Коллекция [outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="55ed4-155">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="55ed4-156">Группы задач Outlook пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-156">The user's Outlook task groups.</span></span> <span data-ttu-id="55ed4-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55ed4-157">Read-only.</span></span> <span data-ttu-id="55ed4-158">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="55ed4-158">Nullable.</span></span>|
|<span data-ttu-id="55ed4-159">задачи (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="55ed4-159">tasks (deprecated)</span></span>|<span data-ttu-id="55ed4-160">Коллекция объектов [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="55ed4-160">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="55ed4-161">Задачи Outlook пользователя.</span><span class="sxs-lookup"><span data-stu-id="55ed4-161">The user's Outlook tasks.</span></span> <span data-ttu-id="55ed4-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55ed4-162">Read-only.</span></span> <span data-ttu-id="55ed4-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="55ed4-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55ed4-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55ed4-164">JSON representation</span></span>

<span data-ttu-id="55ed4-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55ed4-165">Here is a JSON representation of the resource</span></span>

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
