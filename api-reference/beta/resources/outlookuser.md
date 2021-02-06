---
title: Тип ресурса outlookUser
description: Представляет службы Outlook, доступные пользователю.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 15afe75d10bad489b913eaf7215cbc8327e02317
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130671"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="1cf6f-103">Тип ресурса outlookUser</span><span class="sxs-lookup"><span data-stu-id="1cf6f-103">outlookUser resource type</span></span>

<span data-ttu-id="1cf6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cf6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="1cf6f-105">Представляет службы Outlook, доступные пользователю.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-105">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="1cf6f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1cf6f-106">Methods</span></span>

| <span data-ttu-id="1cf6f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1cf6f-107">Method</span></span>           | <span data-ttu-id="1cf6f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1cf6f-108">Return Type</span></span>    |<span data-ttu-id="1cf6f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1cf6f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1cf6f-110">Создание категории</span><span class="sxs-lookup"><span data-stu-id="1cf6f-110">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="1cf6f-111">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="1cf6f-111">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="1cf6f-112">Создание объекта **outlookCategory** в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-112">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="1cf6f-113">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="1cf6f-113">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="1cf6f-114">Коллекция [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-114">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="1cf6f-115">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-115">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="1cf6f-116">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="1cf6f-116">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="1cf6f-117">Коллекция [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-117">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="1cf6f-118">Получение списка языковых стандартов и языков, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-118">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="1cf6f-119">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="1cf6f-119">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="1cf6f-120">Коллекция [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-120">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="1cf6f-121">Получение списка часовых поясов, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-121">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |
|<span data-ttu-id="1cf6f-122">[Create outlookTaskFolder](../api/outlookuser-post-taskfolders.md) (deprecated)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-122">[Create outlookTaskFolder](../api/outlookuser-post-taskfolders.md) (deprecated)</span></span> |[<span data-ttu-id="1cf6f-123">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1cf6f-123">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="1cf6f-124">Создайте папку задач в группе задач по умолчанию `My Tasks` () почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-124">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|<span data-ttu-id="1cf6f-125">[Список taskFolders](../api/outlookuser-list-taskfolders.md) (неподдержный)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-125">[List taskFolders](../api/outlookuser-list-taskfolders.md) (deprecated)</span></span> |<span data-ttu-id="1cf6f-126">[Коллекция outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-126">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="1cf6f-127">Получите все папки задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-127">Get all the Outlook task folders in the user's mailbox.</span></span>|
|<span data-ttu-id="1cf6f-128">[Создание outlookTaskGroup](../api/outlookuser-post-taskgroups.md) (неподготовлено)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-128">[Create outlookTaskGroup](../api/outlookuser-post-taskgroups.md) (deprecated)</span></span> |[<span data-ttu-id="1cf6f-129">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="1cf6f-129">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="1cf6f-130">Создайте группу задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-130">Create an Outlook task group in the user's mailbox.</span></span>|
|<span data-ttu-id="1cf6f-131">[Список taskGroups](../api/outlookuser-list-taskgroups.md) (неподготовленный)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-131">[List taskGroups](../api/outlookuser-list-taskgroups.md) (deprecated)</span></span> |<span data-ttu-id="1cf6f-132">[Коллекция outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-132">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="1cf6f-133">Получите все группы задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-133">Get all the Outlook task groups in the user's mailbox.</span></span>|
|<span data-ttu-id="1cf6f-134">[Создание объекта outlookTask](../api/outlookuser-post-tasks.md) (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-134">[Create outlookTask](../api/outlookuser-post-tasks.md) (deprecated)</span></span> |[<span data-ttu-id="1cf6f-135">outlookTask</span><span class="sxs-lookup"><span data-stu-id="1cf6f-135">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="1cf6f-136">Создайте задачу Outlook в группе задач по умолчанию () и папке задач по умолчанию () в почтовом ящике `My Tasks` `Tasks` пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-136">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|<span data-ttu-id="1cf6f-137">[Перечисление задач](../api/outlookuser-list-tasks.md) (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-137">[List tasks](../api/outlookuser-list-tasks.md) (deprecated)</span></span> |<span data-ttu-id="1cf6f-138">Коллекция объектов [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-138">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="1cf6f-139">Получение всех задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-139">Get all the Outlook tasks in the user's mailbox.</span></span>|



## <a name="properties"></a><span data-ttu-id="1cf6f-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="1cf6f-140">Properties</span></span>
<span data-ttu-id="1cf6f-141">Нет</span><span class="sxs-lookup"><span data-stu-id="1cf6f-141">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1cf6f-142">Связи</span><span class="sxs-lookup"><span data-stu-id="1cf6f-142">Relationships</span></span>
| <span data-ttu-id="1cf6f-143">Связь</span><span class="sxs-lookup"><span data-stu-id="1cf6f-143">Relationship</span></span> | <span data-ttu-id="1cf6f-144">Тип</span><span class="sxs-lookup"><span data-stu-id="1cf6f-144">Type</span></span>   |<span data-ttu-id="1cf6f-145">Описание</span><span class="sxs-lookup"><span data-stu-id="1cf6f-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cf6f-146">masterCategories</span><span class="sxs-lookup"><span data-stu-id="1cf6f-146">masterCategories</span></span>|<span data-ttu-id="1cf6f-147">Коллекция [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-147">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="1cf6f-148">Список категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-148">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="1cf6f-149">taskFolders (неподдержный)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-149">taskFolders (deprecated)</span></span>|<span data-ttu-id="1cf6f-150">[Коллекция outlookTaskFolder](outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-150">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="1cf6f-151">Папки задач Outlook пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-151">The user's Outlook task folders.</span></span> <span data-ttu-id="1cf6f-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-152">Read-only.</span></span> <span data-ttu-id="1cf6f-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-153">Nullable.</span></span>|
|<span data-ttu-id="1cf6f-154">taskGroups (неподготовленные)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-154">taskGroups (deprecated)</span></span>|<span data-ttu-id="1cf6f-155">[Коллекция outlookTaskGroup](outlooktaskgroup.md)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-155">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="1cf6f-156">Группы задач Outlook пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-156">The user's Outlook task groups.</span></span> <span data-ttu-id="1cf6f-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-157">Read-only.</span></span> <span data-ttu-id="1cf6f-158">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-158">Nullable.</span></span>|
|<span data-ttu-id="1cf6f-159">задачи (неподготовленные)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-159">tasks (deprecated)</span></span>|<span data-ttu-id="1cf6f-160">Коллекция объектов [outlookTask](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="1cf6f-160">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="1cf6f-161">Задачи пользователя Outlook.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-161">The user's Outlook tasks.</span></span> <span data-ttu-id="1cf6f-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-162">Read-only.</span></span> <span data-ttu-id="1cf6f-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1cf6f-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1cf6f-164">JSON representation</span></span>

<span data-ttu-id="1cf6f-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cf6f-165">Here is a JSON representation of the resource</span></span>

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


