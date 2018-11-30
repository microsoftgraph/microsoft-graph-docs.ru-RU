---
title: Тип ресурса contactFolder
description: Папка, содержащая контакты.
ms.openlocfilehash: 3e9916d70a23c8acd4b1da2ee8f7e2df4c408e41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079164"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="c2aa9-103">Тип ресурса contactFolder</span><span class="sxs-lookup"><span data-stu-id="c2aa9-103">contactFolder resource type</span></span>

> <span data-ttu-id="c2aa9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2aa9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2aa9-106">Папка, содержащая контакты.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-106">A folder that contains contacts.</span></span>

<span data-ttu-id="c2aa9-107">В этом ресурсе возможно использование [запроса изменений](/graph/delta-query-overview) для отслеживания добавочных дополнений, удалений и обновлений благодаря функции [delta](../api/contactfolder-delta.md).</span><span class="sxs-lookup"><span data-stu-id="c2aa9-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="c2aa9-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c2aa9-108">Methods</span></span>

| <span data-ttu-id="c2aa9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c2aa9-109">Method</span></span>       | <span data-ttu-id="c2aa9-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c2aa9-110">Return Type</span></span>  |<span data-ttu-id="c2aa9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c2aa9-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c2aa9-112">Получение contactFolder</span><span class="sxs-lookup"><span data-stu-id="c2aa9-112">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="c2aa9-113">contactFolder</span><span class="sxs-lookup"><span data-stu-id="c2aa9-113">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="c2aa9-114">Получение папки с контактами с помощью идентификатора папки контактов.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-114">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="c2aa9-115">Обновление</span><span class="sxs-lookup"><span data-stu-id="c2aa9-115">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="c2aa9-116">contactFolder</span><span class="sxs-lookup"><span data-stu-id="c2aa9-116">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="c2aa9-117">Обновление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-117">Update contactFolder object.</span></span> |
|[<span data-ttu-id="c2aa9-118">Удаление</span><span class="sxs-lookup"><span data-stu-id="c2aa9-118">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="c2aa9-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c2aa9-119">None</span></span> |<span data-ttu-id="c2aa9-120">Удаление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-120">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="c2aa9-121">Список экземпляров childFolders</span><span class="sxs-lookup"><span data-stu-id="c2aa9-121">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="c2aa9-122">[contactFolder](contactfolder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c2aa9-122">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="c2aa9-123">Получение коллекции дочерних папок для указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-123">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="c2aa9-124">Создание дочернего элемента contactFolder</span><span class="sxs-lookup"><span data-stu-id="c2aa9-124">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |<span data-ttu-id="c2aa9-125">[contactFolder](contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c2aa9-125">[contactFolder](contactfolder.md)</span></span>| <span data-ttu-id="c2aa9-126">Создание дочернего элемента contactFolder для указанной папки.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-126">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="c2aa9-127">delta</span><span class="sxs-lookup"><span data-stu-id="c2aa9-127">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="c2aa9-128">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="c2aa9-128">[contact](contact.md) collection</span></span>| <span data-ttu-id="c2aa9-129">Получение набора папок контактов, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-129">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="c2aa9-130">Список контактов в папке</span><span class="sxs-lookup"><span data-stu-id="c2aa9-130">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="c2aa9-131">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="c2aa9-131">[contact](contact.md) collection</span></span>| <span data-ttu-id="c2aa9-132">Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-132">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="c2aa9-133">Создание контакта в папке</span><span class="sxs-lookup"><span data-stu-id="c2aa9-133">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="c2aa9-134">контакт</span><span class="sxs-lookup"><span data-stu-id="c2aa9-134">contact</span></span>](contact.md)| <span data-ttu-id="c2aa9-135">Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-135">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="c2aa9-136">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="c2aa9-136">**Extended properties**</span></span>| | |
|[<span data-ttu-id="c2aa9-137">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="c2aa9-137">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="c2aa9-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="c2aa9-138">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="c2aa9-139">Создание одного или несколько расширенных свойств с одним значением в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-139">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="c2aa9-140">Получение contactFolder с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="c2aa9-140">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="c2aa9-141">contactFolder</span><span class="sxs-lookup"><span data-stu-id="c2aa9-141">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="c2aa9-142">Получение экземпляров contactFolder, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-142">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="c2aa9-143">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="c2aa9-143">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="c2aa9-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="c2aa9-144">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="c2aa9-145">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-145">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="c2aa9-146">Получение contactFolder с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="c2aa9-146">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="c2aa9-147">contactFolder</span><span class="sxs-lookup"><span data-stu-id="c2aa9-147">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="c2aa9-148">Получение экземпляра contactFolder, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-148">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="c2aa9-149">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2aa9-149">Properties</span></span>
| <span data-ttu-id="c2aa9-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2aa9-150">Property</span></span>     | <span data-ttu-id="c2aa9-151">Тип</span><span class="sxs-lookup"><span data-stu-id="c2aa9-151">Type</span></span>   |<span data-ttu-id="c2aa9-152">Описание</span><span class="sxs-lookup"><span data-stu-id="c2aa9-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2aa9-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c2aa9-153">displayName</span></span>|<span data-ttu-id="c2aa9-154">String</span><span class="sxs-lookup"><span data-stu-id="c2aa9-154">String</span></span>|<span data-ttu-id="c2aa9-155">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-155">The folder's display name.</span></span>|
|<span data-ttu-id="c2aa9-156">id</span><span class="sxs-lookup"><span data-stu-id="c2aa9-156">id</span></span>|<span data-ttu-id="c2aa9-157">String</span><span class="sxs-lookup"><span data-stu-id="c2aa9-157">String</span></span>|<span data-ttu-id="c2aa9-p102">Уникальный идентификатор папки с контактами. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-p102">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="c2aa9-160">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="c2aa9-160">parentFolderId</span></span>|<span data-ttu-id="c2aa9-161">String</span><span class="sxs-lookup"><span data-stu-id="c2aa9-161">String</span></span>|<span data-ttu-id="c2aa9-162">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-162">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="c2aa9-163">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="c2aa9-163">wellKnownName</span></span>|<span data-ttu-id="c2aa9-164">string</span><span class="sxs-lookup"><span data-stu-id="c2aa9-164">string</span></span>|<span data-ttu-id="c2aa9-165">Имя папки, если распознанный папки.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-165">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="c2aa9-166">В настоящее время `contacts` является единственным папку распознанный контакты.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-166">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2aa9-167">Связи</span><span class="sxs-lookup"><span data-stu-id="c2aa9-167">Relationships</span></span>
| <span data-ttu-id="c2aa9-168">Связь</span><span class="sxs-lookup"><span data-stu-id="c2aa9-168">Relationship</span></span> | <span data-ttu-id="c2aa9-169">Тип</span><span class="sxs-lookup"><span data-stu-id="c2aa9-169">Type</span></span>   |<span data-ttu-id="c2aa9-170">Описание</span><span class="sxs-lookup"><span data-stu-id="c2aa9-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2aa9-171">childFolders</span><span class="sxs-lookup"><span data-stu-id="c2aa9-171">childFolders</span></span>|<span data-ttu-id="c2aa9-172">Коллекция [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="c2aa9-172">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="c2aa9-p104">Коллекция дочерних папок в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-p104">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c2aa9-177">contacts</span><span class="sxs-lookup"><span data-stu-id="c2aa9-177">contacts</span></span>|<span data-ttu-id="c2aa9-178">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="c2aa9-178">[Contact](contact.md) collection</span></span>|<span data-ttu-id="c2aa9-p105">Контакты в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-p105">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c2aa9-183">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="c2aa9-183">multiValueExtendedProperties</span></span>|<span data-ttu-id="c2aa9-184">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="c2aa9-184">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="c2aa9-p106">Коллекция расширенных свойств с несколькими значениями, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-p106">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c2aa9-188">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="c2aa9-188">singleValueExtendedProperties</span></span>|<span data-ttu-id="c2aa9-189">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="c2aa9-189">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="c2aa9-p107">Коллекция расширенных свойств с одним значением, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-p107">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2aa9-193">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2aa9-193">JSON representation</span></span>

<span data-ttu-id="c2aa9-194">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2aa9-194">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c2aa9-195">См. также</span><span class="sxs-lookup"><span data-stu-id="c2aa9-195">See also</span></span>

- [<span data-ttu-id="c2aa9-196">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="c2aa9-196">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="c2aa9-197">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="c2aa9-197">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
