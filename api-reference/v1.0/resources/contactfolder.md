---
title: Тип ресурса contactFolder
description: Папка, содержащая контакты.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6cf4d6ed75427dce527ced6cb64d0cdcb9afed99
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548168"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="c29fb-103">Тип ресурса contactFolder</span><span class="sxs-lookup"><span data-stu-id="c29fb-103">contactFolder resource type</span></span>

<span data-ttu-id="c29fb-104">Папка, содержащая контакты.</span><span class="sxs-lookup"><span data-stu-id="c29fb-104">A folder that contains contacts.</span></span>

<span data-ttu-id="c29fb-105">Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/contactfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="c29fb-105">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="c29fb-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c29fb-106">Methods</span></span>

| <span data-ttu-id="c29fb-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c29fb-107">Method</span></span>       | <span data-ttu-id="c29fb-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c29fb-108">Return Type</span></span>  |<span data-ttu-id="c29fb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c29fb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c29fb-110">Получение contactFolder</span><span class="sxs-lookup"><span data-stu-id="c29fb-110">Get contactFolder</span></span>](../api/contactfolder-get.md) | <span data-ttu-id="c29fb-111">[contactFolder](contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c29fb-111">[contactFolder](contactfolder.md)</span></span> |<span data-ttu-id="c29fb-112">Получение папки с контактами с помощью идентификатора папки контактов.</span><span class="sxs-lookup"><span data-stu-id="c29fb-112">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="c29fb-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="c29fb-113">Update</span></span>](../api/contactfolder-update.md) | <span data-ttu-id="c29fb-114">[contactFolder](contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c29fb-114">[contactFolder](contactfolder.md)</span></span> |<span data-ttu-id="c29fb-115">Обновление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="c29fb-115">Update contactFolder object.</span></span> |
|[<span data-ttu-id="c29fb-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="c29fb-116">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="c29fb-117">Нет</span><span class="sxs-lookup"><span data-stu-id="c29fb-117">None</span></span> |<span data-ttu-id="c29fb-118">Удаление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="c29fb-118">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="c29fb-119">Список экземпляров childFolders</span><span class="sxs-lookup"><span data-stu-id="c29fb-119">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="c29fb-120">Коллекция [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="c29fb-120">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="c29fb-121">Получение коллекции дочерних папок для указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="c29fb-121">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="c29fb-122">Создание дочернего элемента contactFolder</span><span class="sxs-lookup"><span data-stu-id="c29fb-122">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="c29fb-123">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="c29fb-123">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="c29fb-124">Создание дочернего элемента contactFolder для указанной папки.</span><span class="sxs-lookup"><span data-stu-id="c29fb-124">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="c29fb-125">delta</span><span class="sxs-lookup"><span data-stu-id="c29fb-125">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="c29fb-126">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="c29fb-126">[contact](contact.md) collection</span></span>| <span data-ttu-id="c29fb-127">Получение набора папок контактов, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="c29fb-127">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="c29fb-128">Список контактов в папке</span><span class="sxs-lookup"><span data-stu-id="c29fb-128">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="c29fb-129">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="c29fb-129">[Contact](contact.md) collection</span></span>| <span data-ttu-id="c29fb-130">Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="c29fb-130">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="c29fb-131">Создание контакта в папке</span><span class="sxs-lookup"><span data-stu-id="c29fb-131">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="c29fb-132">Contact</span><span class="sxs-lookup"><span data-stu-id="c29fb-132">Contact</span></span>](contact.md)| <span data-ttu-id="c29fb-133">Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="c29fb-133">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="c29fb-134">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="c29fb-134">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |<span data-ttu-id="c29fb-135">[contactFolder](contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c29fb-135">[contactFolder](contactfolder.md)</span></span>  |<span data-ttu-id="c29fb-136">Создание одного или несколько расширенных свойств с одним значением в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="c29fb-136">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="c29fb-137">Получение contactFolder с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="c29fb-137">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | <span data-ttu-id="c29fb-138">[contactFolder](contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c29fb-138">[contactFolder](contactfolder.md)</span></span> | <span data-ttu-id="c29fb-139">Получение экземпляров contactFolder, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="c29fb-139">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="c29fb-140">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="c29fb-140">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="c29fb-141">[contactFolder](contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c29fb-141">[contactFolder](contactfolder.md)</span></span> | <span data-ttu-id="c29fb-142">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="c29fb-142">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="c29fb-143">Получение contactFolder с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="c29fb-143">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | <span data-ttu-id="c29fb-144">[contactFolder](contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c29fb-144">[contactFolder](contactfolder.md)</span></span> | <span data-ttu-id="c29fb-145">Получение экземпляра contactFolder, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="c29fb-145">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="c29fb-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="c29fb-146">Properties</span></span>
| <span data-ttu-id="c29fb-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="c29fb-147">Property</span></span>     | <span data-ttu-id="c29fb-148">Тип</span><span class="sxs-lookup"><span data-stu-id="c29fb-148">Type</span></span>   |<span data-ttu-id="c29fb-149">Описание</span><span class="sxs-lookup"><span data-stu-id="c29fb-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c29fb-150">displayName</span><span class="sxs-lookup"><span data-stu-id="c29fb-150">displayName</span></span>|<span data-ttu-id="c29fb-151">String</span><span class="sxs-lookup"><span data-stu-id="c29fb-151">String</span></span>|<span data-ttu-id="c29fb-152">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="c29fb-152">The folder's display name.</span></span>|
|<span data-ttu-id="c29fb-153">id</span><span class="sxs-lookup"><span data-stu-id="c29fb-153">id</span></span>|<span data-ttu-id="c29fb-154">Строка</span><span class="sxs-lookup"><span data-stu-id="c29fb-154">String</span></span>|<span data-ttu-id="c29fb-p101">Уникальный идентификатор папки с контактами. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c29fb-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="c29fb-157">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="c29fb-157">parentFolderId</span></span>|<span data-ttu-id="c29fb-158">String</span><span class="sxs-lookup"><span data-stu-id="c29fb-158">String</span></span>|<span data-ttu-id="c29fb-159">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="c29fb-159">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c29fb-160">Связи</span><span class="sxs-lookup"><span data-stu-id="c29fb-160">Relationships</span></span>
| <span data-ttu-id="c29fb-161">Отношение</span><span class="sxs-lookup"><span data-stu-id="c29fb-161">Relationship</span></span> | <span data-ttu-id="c29fb-162">Тип</span><span class="sxs-lookup"><span data-stu-id="c29fb-162">Type</span></span>   |<span data-ttu-id="c29fb-163">Описание</span><span class="sxs-lookup"><span data-stu-id="c29fb-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c29fb-164">childFolders</span><span class="sxs-lookup"><span data-stu-id="c29fb-164">childFolders</span></span>|<span data-ttu-id="c29fb-165">Коллекция [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="c29fb-165">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="c29fb-p102">Коллекция дочерних папок в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c29fb-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c29fb-170">contacts</span><span class="sxs-lookup"><span data-stu-id="c29fb-170">contacts</span></span>|<span data-ttu-id="c29fb-171">Коллекция [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="c29fb-171">[Contact](contact.md) collection</span></span>|<span data-ttu-id="c29fb-p103">Контакты в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c29fb-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c29fb-176">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="c29fb-176">multiValueExtendedProperties</span></span>|<span data-ttu-id="c29fb-177">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="c29fb-177">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="c29fb-p104">Коллекция расширенных свойств с несколькими значениями, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c29fb-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c29fb-181">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="c29fb-181">singleValueExtendedProperties</span></span>|<span data-ttu-id="c29fb-182">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="c29fb-182">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="c29fb-p105">Коллекция расширенных свойств с одним значением, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c29fb-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c29fb-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c29fb-186">JSON representation</span></span>

<span data-ttu-id="c29fb-187">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c29fb-187">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c29fb-188">См. также</span><span class="sxs-lookup"><span data-stu-id="c29fb-188">See also</span></span>

- [<span data-ttu-id="c29fb-189">Отслеживание изменений данных Microsoft Graph с помощью запроса изменений</span><span class="sxs-lookup"><span data-stu-id="c29fb-189">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="c29fb-190">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="c29fb-190">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
