---
title: Тип ресурса contactFolder
description: Папка, содержащая контакты.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 03bc6f2a2dfda74af701a14a5b59cbc8865420b8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449481"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="eb47f-103">Тип ресурса contactFolder</span><span class="sxs-lookup"><span data-stu-id="eb47f-103">contactFolder resource type</span></span>

<span data-ttu-id="eb47f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb47f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb47f-105">Папка, содержащая контакты.</span><span class="sxs-lookup"><span data-stu-id="eb47f-105">A folder that contains contacts.</span></span>

<span data-ttu-id="eb47f-106">Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/contactfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="eb47f-106">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="eb47f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="eb47f-107">Methods</span></span>

| <span data-ttu-id="eb47f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="eb47f-108">Method</span></span>       | <span data-ttu-id="eb47f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eb47f-109">Return Type</span></span>  |<span data-ttu-id="eb47f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eb47f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eb47f-111">Получение contactFolder</span><span class="sxs-lookup"><span data-stu-id="eb47f-111">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="eb47f-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="eb47f-112">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="eb47f-113">Получение папки с контактами с помощью идентификатора папки контактов.</span><span class="sxs-lookup"><span data-stu-id="eb47f-113">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="eb47f-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="eb47f-114">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="eb47f-115">contactFolder</span><span class="sxs-lookup"><span data-stu-id="eb47f-115">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="eb47f-116">Обновление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="eb47f-116">Update contactFolder object.</span></span> |
|<span data-ttu-id="eb47f-117">[удаление](../api/contactfolder-delete.md);</span><span class="sxs-lookup"><span data-stu-id="eb47f-117">[Delete](../api/contactfolder-delete.md)</span></span> | <span data-ttu-id="eb47f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="eb47f-118">None</span></span> |<span data-ttu-id="eb47f-119">Удаление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="eb47f-119">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="eb47f-120">Список экземпляров childFolders</span><span class="sxs-lookup"><span data-stu-id="eb47f-120">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="eb47f-121">Коллекция [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="eb47f-121">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="eb47f-122">Получение коллекции дочерних папок для указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="eb47f-122">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="eb47f-123">Создание дочернего элемента contactFolder</span><span class="sxs-lookup"><span data-stu-id="eb47f-123">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="eb47f-124">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="eb47f-124">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="eb47f-125">Создание дочернего элемента contactFolder для указанной папки.</span><span class="sxs-lookup"><span data-stu-id="eb47f-125">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="eb47f-126">delta</span><span class="sxs-lookup"><span data-stu-id="eb47f-126">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="eb47f-127">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="eb47f-127">[contact](contact.md) collection</span></span>| <span data-ttu-id="eb47f-128">Получение набора папок контактов, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="eb47f-128">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="eb47f-129">Список контактов в папке</span><span class="sxs-lookup"><span data-stu-id="eb47f-129">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="eb47f-130">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="eb47f-130">[Contact](contact.md) collection</span></span>| <span data-ttu-id="eb47f-131">Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="eb47f-131">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="eb47f-132">Создание контакта в папке</span><span class="sxs-lookup"><span data-stu-id="eb47f-132">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="eb47f-133">Contact</span><span class="sxs-lookup"><span data-stu-id="eb47f-133">Contact</span></span>](contact.md)| <span data-ttu-id="eb47f-134">Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="eb47f-134">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="eb47f-135">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="eb47f-135">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="eb47f-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="eb47f-136">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="eb47f-137">Создание одного или несколько расширенных свойств с одним значением в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="eb47f-137">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="eb47f-138">Получение contactFolder с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="eb47f-138">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="eb47f-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="eb47f-139">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="eb47f-140">Получение экземпляров contactFolder, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="eb47f-140">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="eb47f-141">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="eb47f-141">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="eb47f-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="eb47f-142">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="eb47f-143">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="eb47f-143">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="eb47f-144">Получение contactFolder с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="eb47f-144">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="eb47f-145">contactFolder</span><span class="sxs-lookup"><span data-stu-id="eb47f-145">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="eb47f-146">Получение экземпляра contactFolder, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="eb47f-146">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="eb47f-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb47f-147">Properties</span></span>
| <span data-ttu-id="eb47f-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb47f-148">Property</span></span>     | <span data-ttu-id="eb47f-149">Тип</span><span class="sxs-lookup"><span data-stu-id="eb47f-149">Type</span></span>   |<span data-ttu-id="eb47f-150">Описание</span><span class="sxs-lookup"><span data-stu-id="eb47f-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb47f-151">displayName</span><span class="sxs-lookup"><span data-stu-id="eb47f-151">displayName</span></span>|<span data-ttu-id="eb47f-152">Строка</span><span class="sxs-lookup"><span data-stu-id="eb47f-152">String</span></span>|<span data-ttu-id="eb47f-153">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="eb47f-153">The folder's display name.</span></span>|
|<span data-ttu-id="eb47f-154">id</span><span class="sxs-lookup"><span data-stu-id="eb47f-154">id</span></span>|<span data-ttu-id="eb47f-155">String</span><span class="sxs-lookup"><span data-stu-id="eb47f-155">String</span></span>|<span data-ttu-id="eb47f-p101">Уникальный идентификатор папки с контактами. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb47f-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="eb47f-158">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="eb47f-158">parentFolderId</span></span>|<span data-ttu-id="eb47f-159">String</span><span class="sxs-lookup"><span data-stu-id="eb47f-159">String</span></span>|<span data-ttu-id="eb47f-160">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="eb47f-160">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb47f-161">Связи</span><span class="sxs-lookup"><span data-stu-id="eb47f-161">Relationships</span></span>
| <span data-ttu-id="eb47f-162">Связь</span><span class="sxs-lookup"><span data-stu-id="eb47f-162">Relationship</span></span> | <span data-ttu-id="eb47f-163">Тип</span><span class="sxs-lookup"><span data-stu-id="eb47f-163">Type</span></span>   |<span data-ttu-id="eb47f-164">Описание</span><span class="sxs-lookup"><span data-stu-id="eb47f-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb47f-165">childFolders</span><span class="sxs-lookup"><span data-stu-id="eb47f-165">childFolders</span></span>|<span data-ttu-id="eb47f-166">Коллекция [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="eb47f-166">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="eb47f-p102">Коллекция дочерних папок в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="eb47f-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="eb47f-171">contacts</span><span class="sxs-lookup"><span data-stu-id="eb47f-171">contacts</span></span>|<span data-ttu-id="eb47f-172">Коллекция [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="eb47f-172">[Contact](contact.md) collection</span></span>|<span data-ttu-id="eb47f-p103">Контакты в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="eb47f-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="eb47f-177">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="eb47f-177">multiValueExtendedProperties</span></span>|<span data-ttu-id="eb47f-178">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="eb47f-178">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="eb47f-p104">Коллекция расширенных свойств с несколькими значениями, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="eb47f-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="eb47f-182">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="eb47f-182">singleValueExtendedProperties</span></span>|<span data-ttu-id="eb47f-183">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="eb47f-183">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="eb47f-p105">Коллекция расширенных свойств с одним значением, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="eb47f-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb47f-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb47f-187">JSON representation</span></span>

<span data-ttu-id="eb47f-188">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb47f-188">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="eb47f-189">См. также</span><span class="sxs-lookup"><span data-stu-id="eb47f-189">See also</span></span>

- [<span data-ttu-id="eb47f-190">Отслеживание изменений данных Microsoft Graph с помощью запроса изменений</span><span class="sxs-lookup"><span data-stu-id="eb47f-190">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="eb47f-191">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="eb47f-191">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
