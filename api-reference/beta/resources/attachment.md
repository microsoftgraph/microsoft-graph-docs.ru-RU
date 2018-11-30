---
title: Тип ресурса attachment
description: Связанное содержимое можно добавить на событие
ms.openlocfilehash: f0bb9ec37d2fe3d034dce9532ad316d371c4937e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082145"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="4e55b-103">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="4e55b-103">attachment resource type</span></span>

> <span data-ttu-id="4e55b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4e55b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e55b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e55b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e55b-106">Связанное содержимое можно добавить для [события](../resources/event.md), [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [публикации](../resources/post.md) в виде вложения.</span><span class="sxs-lookup"><span data-stu-id="4e55b-106">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="4e55b-107">**attachment** — базовый ресурс для следующих производных типов вложений:</span><span class="sxs-lookup"><span data-stu-id="4e55b-107">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="4e55b-108">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="4e55b-108">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="4e55b-109">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="4e55b-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="4e55b-110">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="4e55b-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="4e55b-111">Методы</span><span class="sxs-lookup"><span data-stu-id="4e55b-111">Methods</span></span>

<span data-ttu-id="4e55b-112">Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="4e55b-112">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="4e55b-113">Метод</span><span class="sxs-lookup"><span data-stu-id="4e55b-113">Method</span></span>       | <span data-ttu-id="4e55b-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e55b-114">Return Type</span></span>  |<span data-ttu-id="4e55b-115">Описание</span><span class="sxs-lookup"><span data-stu-id="4e55b-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e55b-116">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="4e55b-116">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="4e55b-117">attachment</span><span class="sxs-lookup"><span data-stu-id="4e55b-117">attachment</span></span>](attachment.md) |<span data-ttu-id="4e55b-118">Чтение свойства и связи вложения, подключенного к события, сообщения, задачи Outlook или post.</span><span class="sxs-lookup"><span data-stu-id="4e55b-118">Read the properties and relationships of an attachment, attached to an event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="4e55b-119">Добавление вложения к данным о событии</span><span class="sxs-lookup"><span data-stu-id="4e55b-119">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="4e55b-120">attachment</span><span class="sxs-lookup"><span data-stu-id="4e55b-120">attachment</span></span>](attachment.md) |<span data-ttu-id="4e55b-121">Добавление для события файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="4e55b-121">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="4e55b-122">Добавление вложения в сообщение</span><span class="sxs-lookup"><span data-stu-id="4e55b-122">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="4e55b-123">attachment</span><span class="sxs-lookup"><span data-stu-id="4e55b-123">attachment</span></span>](attachment.md) |<span data-ttu-id="4e55b-124">Добавление в сообщение файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="4e55b-124">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="4e55b-125">Добавление вложения в задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="4e55b-125">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="4e55b-126">attachment</span><span class="sxs-lookup"><span data-stu-id="4e55b-126">attachment</span></span>](attachment.md) |<span data-ttu-id="4e55b-127">Добавление файла, элемента или вложения ссылки на задачи Outlook.</span><span class="sxs-lookup"><span data-stu-id="4e55b-127">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="4e55b-128">Добавление вложения в запись</span><span class="sxs-lookup"><span data-stu-id="4e55b-128">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="4e55b-129">attachment</span><span class="sxs-lookup"><span data-stu-id="4e55b-129">attachment</span></span>](attachment.md) |<span data-ttu-id="4e55b-130">Добавление в запись файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="4e55b-130">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="4e55b-131">Список вложений для события</span><span class="sxs-lookup"><span data-stu-id="4e55b-131">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="4e55b-132">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="4e55b-132">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="4e55b-133">Получение списка вложений для события.</span><span class="sxs-lookup"><span data-stu-id="4e55b-133">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="4e55b-134">Список вложений для сообщения</span><span class="sxs-lookup"><span data-stu-id="4e55b-134">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="4e55b-135">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="4e55b-135">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="4e55b-136">Получение списка вложений для сообщения.</span><span class="sxs-lookup"><span data-stu-id="4e55b-136">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="4e55b-137">Вложения списка задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="4e55b-137">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="4e55b-138">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="4e55b-138">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="4e55b-139">Получение списка вложений для задачи Outlook.</span><span class="sxs-lookup"><span data-stu-id="4e55b-139">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="4e55b-140">Список вложений для записи</span><span class="sxs-lookup"><span data-stu-id="4e55b-140">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="4e55b-141">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="4e55b-141">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="4e55b-142">Получение списка вложений для записи.</span><span class="sxs-lookup"><span data-stu-id="4e55b-142">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="4e55b-143">Удаление</span><span class="sxs-lookup"><span data-stu-id="4e55b-143">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="4e55b-144">Нет</span><span class="sxs-lookup"><span data-stu-id="4e55b-144">None</span></span> |<span data-ttu-id="4e55b-145">Удаление вложения на события, сообщения, задачи Outlook или post.</span><span class="sxs-lookup"><span data-stu-id="4e55b-145">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="4e55b-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e55b-146">Properties</span></span>

<span data-ttu-id="4e55b-p102">Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="4e55b-p102">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="4e55b-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e55b-149">Property</span></span>     | <span data-ttu-id="4e55b-150">Тип</span><span class="sxs-lookup"><span data-stu-id="4e55b-150">Type</span></span>   |<span data-ttu-id="4e55b-151">Описание</span><span class="sxs-lookup"><span data-stu-id="4e55b-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e55b-152">contentType</span><span class="sxs-lookup"><span data-stu-id="4e55b-152">contentType</span></span>|<span data-ttu-id="4e55b-153">String</span><span class="sxs-lookup"><span data-stu-id="4e55b-153">String</span></span>|<span data-ttu-id="4e55b-154">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="4e55b-154">The MIME type.</span></span>|
|<span data-ttu-id="4e55b-155">id</span><span class="sxs-lookup"><span data-stu-id="4e55b-155">id</span></span>|<span data-ttu-id="4e55b-156">String</span><span class="sxs-lookup"><span data-stu-id="4e55b-156">String</span></span>| <span data-ttu-id="4e55b-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e55b-157">Read-only.</span></span>|
|<span data-ttu-id="4e55b-158">isInline</span><span class="sxs-lookup"><span data-stu-id="4e55b-158">isInline</span></span>|<span data-ttu-id="4e55b-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e55b-159">Boolean</span></span>|<span data-ttu-id="4e55b-160">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="4e55b-160">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="4e55b-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e55b-161">lastModifiedDateTime</span></span>|<span data-ttu-id="4e55b-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e55b-162">DateTimeOffset</span></span>|<span data-ttu-id="4e55b-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4e55b-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4e55b-165">имя</span><span class="sxs-lookup"><span data-stu-id="4e55b-165">name</span></span>|<span data-ttu-id="4e55b-166">String</span><span class="sxs-lookup"><span data-stu-id="4e55b-166">String</span></span>|<span data-ttu-id="4e55b-167">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="4e55b-167">The display name of the attachment.</span></span> <span data-ttu-id="4e55b-168">Она не обязательно должна находиться фактическое имя файла.</span><span class="sxs-lookup"><span data-stu-id="4e55b-168">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="4e55b-169">size</span><span class="sxs-lookup"><span data-stu-id="4e55b-169">size</span></span>|<span data-ttu-id="4e55b-170">Int32</span><span class="sxs-lookup"><span data-stu-id="4e55b-170">Int32</span></span>|<span data-ttu-id="4e55b-171">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="4e55b-171">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e55b-172">Отношения</span><span class="sxs-lookup"><span data-stu-id="4e55b-172">Relationships</span></span>
<span data-ttu-id="4e55b-173">Нет</span><span class="sxs-lookup"><span data-stu-id="4e55b-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e55b-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e55b-174">JSON representation</span></span>

<span data-ttu-id="4e55b-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e55b-175">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
