---
title: Тип ресурса contactFolder
description: Папка, содержащая контакты.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e18c1688bced04f20d12211fb5e5a70e884bd0b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056983"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="239ba-103">Тип ресурса contactFolder</span><span class="sxs-lookup"><span data-stu-id="239ba-103">contactFolder resource type</span></span>

<span data-ttu-id="239ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="239ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="239ba-105">Папка, содержащая контакты.</span><span class="sxs-lookup"><span data-stu-id="239ba-105">A folder that contains contacts.</span></span>

<span data-ttu-id="239ba-106">Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/contactfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="239ba-106">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="239ba-107">Методы</span><span class="sxs-lookup"><span data-stu-id="239ba-107">Methods</span></span>

| <span data-ttu-id="239ba-108">Метод</span><span class="sxs-lookup"><span data-stu-id="239ba-108">Method</span></span>       | <span data-ttu-id="239ba-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="239ba-109">Return Type</span></span>  |<span data-ttu-id="239ba-110">Описание</span><span class="sxs-lookup"><span data-stu-id="239ba-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="239ba-111">Получение contactFolder</span><span class="sxs-lookup"><span data-stu-id="239ba-111">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="239ba-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="239ba-112">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="239ba-113">Получение папки с контактами с помощью идентификатора папки контактов.</span><span class="sxs-lookup"><span data-stu-id="239ba-113">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="239ba-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="239ba-114">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="239ba-115">contactFolder</span><span class="sxs-lookup"><span data-stu-id="239ba-115">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="239ba-116">Обновление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="239ba-116">Update contactFolder object.</span></span> |
|<span data-ttu-id="239ba-117">[удаление](../api/contactfolder-delete.md);</span><span class="sxs-lookup"><span data-stu-id="239ba-117">[Delete](../api/contactfolder-delete.md)</span></span> | <span data-ttu-id="239ba-118">Нет</span><span class="sxs-lookup"><span data-stu-id="239ba-118">None</span></span> |<span data-ttu-id="239ba-119">Удаление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="239ba-119">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="239ba-120">Список экземпляров childFolders</span><span class="sxs-lookup"><span data-stu-id="239ba-120">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="239ba-121">Коллекция [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="239ba-121">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="239ba-122">Получение коллекции дочерних папок для указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="239ba-122">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="239ba-123">Создание дочернего элемента contactFolder</span><span class="sxs-lookup"><span data-stu-id="239ba-123">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="239ba-124">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="239ba-124">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="239ba-125">Создание дочернего элемента contactFolder для указанной папки.</span><span class="sxs-lookup"><span data-stu-id="239ba-125">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="239ba-126">delta</span><span class="sxs-lookup"><span data-stu-id="239ba-126">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="239ba-127">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="239ba-127">[contact](contact.md) collection</span></span>| <span data-ttu-id="239ba-128">Получение набора папок контактов, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="239ba-128">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="239ba-129">Список контактов в папке</span><span class="sxs-lookup"><span data-stu-id="239ba-129">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="239ba-130">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="239ba-130">[Contact](contact.md) collection</span></span>| <span data-ttu-id="239ba-131">Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="239ba-131">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="239ba-132">Создание контакта в папке</span><span class="sxs-lookup"><span data-stu-id="239ba-132">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="239ba-133">Contact</span><span class="sxs-lookup"><span data-stu-id="239ba-133">Contact</span></span>](contact.md)| <span data-ttu-id="239ba-134">Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="239ba-134">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="239ba-135">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="239ba-135">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="239ba-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="239ba-136">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="239ba-137">Создание одного или несколько расширенных свойств с одним значением в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="239ba-137">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="239ba-138">Получение contactFolder с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="239ba-138">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="239ba-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="239ba-139">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="239ba-140">Получение экземпляров contactFolder, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="239ba-140">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="239ba-141">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="239ba-141">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="239ba-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="239ba-142">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="239ba-143">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="239ba-143">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="239ba-144">Получение contactFolder с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="239ba-144">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="239ba-145">contactFolder</span><span class="sxs-lookup"><span data-stu-id="239ba-145">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="239ba-146">Получение экземпляра contactFolder, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="239ba-146">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="239ba-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="239ba-147">Properties</span></span>
| <span data-ttu-id="239ba-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="239ba-148">Property</span></span>     | <span data-ttu-id="239ba-149">Тип</span><span class="sxs-lookup"><span data-stu-id="239ba-149">Type</span></span>   |<span data-ttu-id="239ba-150">Описание</span><span class="sxs-lookup"><span data-stu-id="239ba-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="239ba-151">displayName</span><span class="sxs-lookup"><span data-stu-id="239ba-151">displayName</span></span>|<span data-ttu-id="239ba-152">String</span><span class="sxs-lookup"><span data-stu-id="239ba-152">String</span></span>|<span data-ttu-id="239ba-153">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="239ba-153">The folder's display name.</span></span>|
|<span data-ttu-id="239ba-154">id</span><span class="sxs-lookup"><span data-stu-id="239ba-154">id</span></span>|<span data-ttu-id="239ba-155">String</span><span class="sxs-lookup"><span data-stu-id="239ba-155">String</span></span>|<span data-ttu-id="239ba-p101">Уникальный идентификатор папки с контактами. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="239ba-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="239ba-158">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="239ba-158">parentFolderId</span></span>|<span data-ttu-id="239ba-159">String</span><span class="sxs-lookup"><span data-stu-id="239ba-159">String</span></span>|<span data-ttu-id="239ba-160">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="239ba-160">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="239ba-161">Связи</span><span class="sxs-lookup"><span data-stu-id="239ba-161">Relationships</span></span>
| <span data-ttu-id="239ba-162">Связь</span><span class="sxs-lookup"><span data-stu-id="239ba-162">Relationship</span></span> | <span data-ttu-id="239ba-163">Тип</span><span class="sxs-lookup"><span data-stu-id="239ba-163">Type</span></span>   |<span data-ttu-id="239ba-164">Описание</span><span class="sxs-lookup"><span data-stu-id="239ba-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="239ba-165">childFolders</span><span class="sxs-lookup"><span data-stu-id="239ba-165">childFolders</span></span>|<span data-ttu-id="239ba-166">Коллекция [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="239ba-166">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="239ba-p102">Коллекция дочерних папок в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="239ba-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="239ba-171">contacts</span><span class="sxs-lookup"><span data-stu-id="239ba-171">contacts</span></span>|<span data-ttu-id="239ba-172">Коллекция [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="239ba-172">[Contact](contact.md) collection</span></span>|<span data-ttu-id="239ba-p103">Контакты в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="239ba-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="239ba-177">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="239ba-177">multiValueExtendedProperties</span></span>|<span data-ttu-id="239ba-178">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="239ba-178">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="239ba-p104">Коллекция расширенных свойств с несколькими значениями, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="239ba-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="239ba-182">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="239ba-182">singleValueExtendedProperties</span></span>|<span data-ttu-id="239ba-183">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="239ba-183">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="239ba-p105">Коллекция расширенных свойств с одним значением, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="239ba-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="239ba-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="239ba-187">JSON representation</span></span>

<span data-ttu-id="239ba-188">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="239ba-188">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.contactFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "navigability": "single",
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="239ba-189">См. также</span><span class="sxs-lookup"><span data-stu-id="239ba-189">See also</span></span>

- [<span data-ttu-id="239ba-190">Отслеживание изменений данных Microsoft Graph с помощью запроса изменений</span><span class="sxs-lookup"><span data-stu-id="239ba-190">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="239ba-191">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="239ba-191">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

