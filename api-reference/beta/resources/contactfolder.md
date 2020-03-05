---
title: Тип ресурса contactFolder
description: Папка, содержащая контакты.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8ebca7ecd2ba49c3a14973bbc6060980c07927d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507459"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="22ace-103">Тип ресурса contactFolder</span><span class="sxs-lookup"><span data-stu-id="22ace-103">contactFolder resource type</span></span>

<span data-ttu-id="22ace-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="22ace-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22ace-105">Папка, содержащая контакты.</span><span class="sxs-lookup"><span data-stu-id="22ace-105">A folder that contains contacts.</span></span>

<span data-ttu-id="22ace-106">Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/contactfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="22ace-106">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="22ace-107">Методы</span><span class="sxs-lookup"><span data-stu-id="22ace-107">Methods</span></span>

| <span data-ttu-id="22ace-108">Метод</span><span class="sxs-lookup"><span data-stu-id="22ace-108">Method</span></span>       | <span data-ttu-id="22ace-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="22ace-109">Return Type</span></span>  |<span data-ttu-id="22ace-110">Описание</span><span class="sxs-lookup"><span data-stu-id="22ace-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="22ace-111">Получение contactFolder</span><span class="sxs-lookup"><span data-stu-id="22ace-111">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="22ace-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="22ace-112">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="22ace-113">Получение папки с контактами с помощью идентификатора папки контактов.</span><span class="sxs-lookup"><span data-stu-id="22ace-113">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="22ace-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="22ace-114">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="22ace-115">contactFolder</span><span class="sxs-lookup"><span data-stu-id="22ace-115">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="22ace-116">Обновление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="22ace-116">Update contactFolder object.</span></span> |
|<span data-ttu-id="22ace-117">[удаление](../api/contactfolder-delete.md);</span><span class="sxs-lookup"><span data-stu-id="22ace-117">[Delete](../api/contactfolder-delete.md)</span></span> | <span data-ttu-id="22ace-118">Нет</span><span class="sxs-lookup"><span data-stu-id="22ace-118">None</span></span> |<span data-ttu-id="22ace-119">Удаление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="22ace-119">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="22ace-120">Список экземпляров childFolders</span><span class="sxs-lookup"><span data-stu-id="22ace-120">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="22ace-121">Коллекция [contactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="22ace-121">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="22ace-122">Получение коллекции дочерних папок для указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="22ace-122">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="22ace-123">Создание дочернего элемента contactFolder</span><span class="sxs-lookup"><span data-stu-id="22ace-123">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="22ace-124">contactFolder</span><span class="sxs-lookup"><span data-stu-id="22ace-124">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="22ace-125">Создание дочернего объекта contactFolder указанной папки.</span><span class="sxs-lookup"><span data-stu-id="22ace-125">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="22ace-126">delta</span><span class="sxs-lookup"><span data-stu-id="22ace-126">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="22ace-127">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="22ace-127">[contact](contact.md) collection</span></span>| <span data-ttu-id="22ace-128">Получение набора папок контактов, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="22ace-128">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="22ace-129">Список контактов в папке</span><span class="sxs-lookup"><span data-stu-id="22ace-129">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="22ace-130">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="22ace-130">[contact](contact.md) collection</span></span>| <span data-ttu-id="22ace-131">Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="22ace-131">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="22ace-132">Создание контакта в папке</span><span class="sxs-lookup"><span data-stu-id="22ace-132">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="22ace-133">contact</span><span class="sxs-lookup"><span data-stu-id="22ace-133">contact</span></span>](contact.md)| <span data-ttu-id="22ace-134">Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="22ace-134">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="22ace-135">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="22ace-135">**Extended properties**</span></span>| | |
|[<span data-ttu-id="22ace-136">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="22ace-136">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="22ace-137">contactFolder</span><span class="sxs-lookup"><span data-stu-id="22ace-137">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="22ace-138">Создание одного или несколько расширенных свойств с одним значением в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="22ace-138">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="22ace-139">Получение contactFolder с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="22ace-139">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="22ace-140">contactFolder</span><span class="sxs-lookup"><span data-stu-id="22ace-140">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="22ace-141">Получение экземпляров contactFolder, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="22ace-141">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="22ace-142">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="22ace-142">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="22ace-143">contactFolder</span><span class="sxs-lookup"><span data-stu-id="22ace-143">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="22ace-144">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="22ace-144">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="22ace-145">Получение contactFolder с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="22ace-145">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="22ace-146">contactFolder</span><span class="sxs-lookup"><span data-stu-id="22ace-146">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="22ace-147">Получение экземпляра contactFolder, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="22ace-147">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="22ace-148">Свойства</span><span class="sxs-lookup"><span data-stu-id="22ace-148">Properties</span></span>
| <span data-ttu-id="22ace-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="22ace-149">Property</span></span>     | <span data-ttu-id="22ace-150">Тип</span><span class="sxs-lookup"><span data-stu-id="22ace-150">Type</span></span>   |<span data-ttu-id="22ace-151">Описание</span><span class="sxs-lookup"><span data-stu-id="22ace-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22ace-152">displayName</span><span class="sxs-lookup"><span data-stu-id="22ace-152">displayName</span></span>|<span data-ttu-id="22ace-153">Строка</span><span class="sxs-lookup"><span data-stu-id="22ace-153">String</span></span>|<span data-ttu-id="22ace-154">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="22ace-154">The folder's display name.</span></span>|
|<span data-ttu-id="22ace-155">id</span><span class="sxs-lookup"><span data-stu-id="22ace-155">id</span></span>|<span data-ttu-id="22ace-156">String</span><span class="sxs-lookup"><span data-stu-id="22ace-156">String</span></span>|<span data-ttu-id="22ace-p101">Уникальный идентификатор папки с контактами. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="22ace-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="22ace-159">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="22ace-159">parentFolderId</span></span>|<span data-ttu-id="22ace-160">String</span><span class="sxs-lookup"><span data-stu-id="22ace-160">String</span></span>|<span data-ttu-id="22ace-161">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="22ace-161">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="22ace-162">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="22ace-162">wellKnownName</span></span>|<span data-ttu-id="22ace-163">строка</span><span class="sxs-lookup"><span data-stu-id="22ace-163">string</span></span>|<span data-ttu-id="22ace-164">Имя папки, если она является распознаваемой папкой.</span><span class="sxs-lookup"><span data-stu-id="22ace-164">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="22ace-165">В `contacts` настоящее время это единственная распознанная папка контактов.</span><span class="sxs-lookup"><span data-stu-id="22ace-165">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22ace-166">Связи</span><span class="sxs-lookup"><span data-stu-id="22ace-166">Relationships</span></span>
| <span data-ttu-id="22ace-167">Связь</span><span class="sxs-lookup"><span data-stu-id="22ace-167">Relationship</span></span> | <span data-ttu-id="22ace-168">Тип</span><span class="sxs-lookup"><span data-stu-id="22ace-168">Type</span></span>   |<span data-ttu-id="22ace-169">Описание</span><span class="sxs-lookup"><span data-stu-id="22ace-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22ace-170">childFolders</span><span class="sxs-lookup"><span data-stu-id="22ace-170">childFolders</span></span>|<span data-ttu-id="22ace-171">Коллекция [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="22ace-171">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="22ace-p103">Коллекция дочерних папок в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="22ace-p103">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="22ace-176">contacts</span><span class="sxs-lookup"><span data-stu-id="22ace-176">contacts</span></span>|<span data-ttu-id="22ace-177">Коллекция [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="22ace-177">[Contact](contact.md) collection</span></span>|<span data-ttu-id="22ace-p104">Контакты в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="22ace-p104">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="22ace-182">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="22ace-182">multiValueExtendedProperties</span></span>|<span data-ttu-id="22ace-183">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="22ace-183">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="22ace-p105">Коллекция расширенных свойств с несколькими значениями, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="22ace-p105">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="22ace-187">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="22ace-187">singleValueExtendedProperties</span></span>|<span data-ttu-id="22ace-188">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="22ace-188">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="22ace-p106">Коллекция расширенных свойств с одним значением, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="22ace-p106">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22ace-192">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22ace-192">JSON representation</span></span>

<span data-ttu-id="22ace-193">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22ace-193">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
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

## <a name="see-also"></a><span data-ttu-id="22ace-194">См. также</span><span class="sxs-lookup"><span data-stu-id="22ace-194">See also</span></span>

- [<span data-ttu-id="22ace-195">Отслеживание изменений данных Microsoft Graph с помощью запроса изменений</span><span class="sxs-lookup"><span data-stu-id="22ace-195">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="22ace-196">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="22ace-196">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
