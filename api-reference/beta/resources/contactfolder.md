---
title: Тип ресурса contactFolder
description: Папка, содержащая контакты.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a4fcb5152a3d7cb5f26214cf2b0a1e4a31dc1ffb
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575872"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="d7376-103">Тип ресурса contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7376-103">contactFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7376-104">Папка, содержащая контакты.</span><span class="sxs-lookup"><span data-stu-id="d7376-104">A folder that contains contacts.</span></span>

<span data-ttu-id="d7376-105">В этом ресурсе возможно использование [запроса изменений](/graph/delta-query-overview) для отслеживания добавочных дополнений, удалений и обновлений благодаря функции [delta](../api/contactfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="d7376-105">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="d7376-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d7376-106">Methods</span></span>

| <span data-ttu-id="d7376-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d7376-107">Method</span></span>       | <span data-ttu-id="d7376-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d7376-108">Return Type</span></span>  |<span data-ttu-id="d7376-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d7376-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7376-110">Получение contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7376-110">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="d7376-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7376-111">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="d7376-112">Получение папки с контактами с помощью идентификатора папки контактов.</span><span class="sxs-lookup"><span data-stu-id="d7376-112">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="d7376-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="d7376-113">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="d7376-114">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7376-114">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="d7376-115">Обновление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="d7376-115">Update contactFolder object.</span></span> |
|[<span data-ttu-id="d7376-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="d7376-116">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="d7376-117">Нет</span><span class="sxs-lookup"><span data-stu-id="d7376-117">None</span></span> |<span data-ttu-id="d7376-118">Удаление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="d7376-118">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="d7376-119">Список экземпляров childFolders</span><span class="sxs-lookup"><span data-stu-id="d7376-119">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="d7376-120">[contactFolder](contactfolder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d7376-120">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="d7376-121">Получение коллекции дочерних папок для указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="d7376-121">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="d7376-122">Создание дочернего элемента contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7376-122">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |<span data-ttu-id="d7376-123">[contactFolder](contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="d7376-123">[contactFolder](contactfolder.md)</span></span>| <span data-ttu-id="d7376-124">Создание дочернего элемента contactFolder для указанной папки.</span><span class="sxs-lookup"><span data-stu-id="d7376-124">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="d7376-125">delta</span><span class="sxs-lookup"><span data-stu-id="d7376-125">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="d7376-126">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="d7376-126">[contact](contact.md) collection</span></span>| <span data-ttu-id="d7376-127">Получение набора папок контактов, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="d7376-127">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="d7376-128">Список контактов в папке</span><span class="sxs-lookup"><span data-stu-id="d7376-128">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="d7376-129">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="d7376-129">[contact](contact.md) collection</span></span>| <span data-ttu-id="d7376-130">Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="d7376-130">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="d7376-131">Создание контакта в папке</span><span class="sxs-lookup"><span data-stu-id="d7376-131">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="d7376-132">contact</span><span class="sxs-lookup"><span data-stu-id="d7376-132">contact</span></span>](contact.md)| <span data-ttu-id="d7376-133">Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="d7376-133">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="d7376-134">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="d7376-134">**Extended properties**</span></span>| | |
|[<span data-ttu-id="d7376-135">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="d7376-135">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="d7376-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7376-136">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="d7376-137">Создание одного или несколько расширенных свойств с одним значением в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="d7376-137">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="d7376-138">Получение contactFolder с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="d7376-138">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="d7376-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7376-139">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="d7376-140">Получение экземпляров contactFolder, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="d7376-140">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="d7376-141">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="d7376-141">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="d7376-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7376-142">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="d7376-143">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="d7376-143">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="d7376-144">Получение contactFolder с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="d7376-144">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="d7376-145">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7376-145">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="d7376-146">Получение экземпляра contactFolder, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="d7376-146">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="d7376-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7376-147">Properties</span></span>
| <span data-ttu-id="d7376-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7376-148">Property</span></span>     | <span data-ttu-id="d7376-149">Тип</span><span class="sxs-lookup"><span data-stu-id="d7376-149">Type</span></span>   |<span data-ttu-id="d7376-150">Описание</span><span class="sxs-lookup"><span data-stu-id="d7376-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7376-151">displayName</span><span class="sxs-lookup"><span data-stu-id="d7376-151">displayName</span></span>|<span data-ttu-id="d7376-152">String</span><span class="sxs-lookup"><span data-stu-id="d7376-152">String</span></span>|<span data-ttu-id="d7376-153">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="d7376-153">The folder's display name.</span></span>|
|<span data-ttu-id="d7376-154">id</span><span class="sxs-lookup"><span data-stu-id="d7376-154">id</span></span>|<span data-ttu-id="d7376-155">String</span><span class="sxs-lookup"><span data-stu-id="d7376-155">String</span></span>|<span data-ttu-id="d7376-p101">Уникальный идентификатор папки с контактами. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7376-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="d7376-158">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="d7376-158">parentFolderId</span></span>|<span data-ttu-id="d7376-159">String</span><span class="sxs-lookup"><span data-stu-id="d7376-159">String</span></span>|<span data-ttu-id="d7376-160">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="d7376-160">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="d7376-161">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="d7376-161">wellKnownName</span></span>|<span data-ttu-id="d7376-162">string</span><span class="sxs-lookup"><span data-stu-id="d7376-162">string</span></span>|<span data-ttu-id="d7376-163">Имя папки, если распознанный папки.</span><span class="sxs-lookup"><span data-stu-id="d7376-163">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="d7376-164">В настоящее время `contacts` является единственным папку распознанный контакты.</span><span class="sxs-lookup"><span data-stu-id="d7376-164">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7376-165">Связи</span><span class="sxs-lookup"><span data-stu-id="d7376-165">Relationships</span></span>
| <span data-ttu-id="d7376-166">Связь</span><span class="sxs-lookup"><span data-stu-id="d7376-166">Relationship</span></span> | <span data-ttu-id="d7376-167">Тип</span><span class="sxs-lookup"><span data-stu-id="d7376-167">Type</span></span>   |<span data-ttu-id="d7376-168">Описание</span><span class="sxs-lookup"><span data-stu-id="d7376-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7376-169">childFolders</span><span class="sxs-lookup"><span data-stu-id="d7376-169">childFolders</span></span>|<span data-ttu-id="d7376-170">Коллекция [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="d7376-170">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="d7376-p103">Коллекция дочерних папок в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d7376-p103">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d7376-175">contacts</span><span class="sxs-lookup"><span data-stu-id="d7376-175">contacts</span></span>|<span data-ttu-id="d7376-176">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="d7376-176">[Contact](contact.md) collection</span></span>|<span data-ttu-id="d7376-p104">Контакты в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d7376-p104">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d7376-181">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="d7376-181">multiValueLegacyExtendedProperty</span></span>|<span data-ttu-id="d7376-182">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="d7376-182">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d7376-p105">Коллекция расширенных свойств с несколькими значениями, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d7376-p105">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d7376-186">singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="d7376-186">singleValueLegacyExtendedProperty</span></span>|<span data-ttu-id="d7376-187">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="d7376-187">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d7376-p106">Коллекция расширенных свойств с одним значением, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d7376-p106">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7376-191">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7376-191">JSON representation</span></span>

<span data-ttu-id="d7376-192">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7376-192">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueLegacyExtendedProperty",
    "singleValueLegacyExtendedProperty"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "wellKnownName": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="d7376-193">См. также</span><span class="sxs-lookup"><span data-stu-id="d7376-193">See also</span></span>

- [<span data-ttu-id="d7376-194">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="d7376-194">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="d7376-195">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="d7376-195">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/contactfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
