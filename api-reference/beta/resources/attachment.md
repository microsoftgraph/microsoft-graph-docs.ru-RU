---
title: Тип ресурса attachment
description: Вы можете добавить связанное содержимое в экземпляр event,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: da7e66d1edbda224fe547b7e7afc8fd88dc5e5aa
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622638"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="758a0-103">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="758a0-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="758a0-104">Вы можете добавить связанное содержимое для [события](../resources/event.md)пользователя, [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [записи](../resources/post.md) группы в виде вложения.</span><span class="sxs-lookup"><span data-stu-id="758a0-104">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="758a0-105">**attachment** — базовый ресурс для следующих производных типов вложений:</span><span class="sxs-lookup"><span data-stu-id="758a0-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="758a0-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="758a0-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="758a0-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="758a0-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="758a0-108">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="758a0-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

<span data-ttu-id="758a0-109">События в групповой календаре не поддерживают вложения.</span><span class="sxs-lookup"><span data-stu-id="758a0-109">Events in group calendars do not support attachments.</span></span>

## <a name="methods"></a><span data-ttu-id="758a0-110">Методы</span><span class="sxs-lookup"><span data-stu-id="758a0-110">Methods</span></span>

<span data-ttu-id="758a0-111">Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="758a0-111">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="758a0-112">Метод</span><span class="sxs-lookup"><span data-stu-id="758a0-112">Method</span></span>       | <span data-ttu-id="758a0-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="758a0-113">Return Type</span></span>  |<span data-ttu-id="758a0-114">Описание</span><span class="sxs-lookup"><span data-stu-id="758a0-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="758a0-115">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="758a0-115">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="758a0-116">attachment</span><span class="sxs-lookup"><span data-stu-id="758a0-116">attachment</span></span>](attachment.md) |<span data-ttu-id="758a0-117">Считывание свойств и связей вложений, вложенных в событие пользователя, сообщение, задачу Outlook или POST.</span><span class="sxs-lookup"><span data-stu-id="758a0-117">Read the properties and relationships of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="758a0-118">Добавление вложения в событие пользователя</span><span class="sxs-lookup"><span data-stu-id="758a0-118">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="758a0-119">attachment</span><span class="sxs-lookup"><span data-stu-id="758a0-119">attachment</span></span>](attachment.md) |<span data-ttu-id="758a0-120">Добавление файла, элемента или ссылки на вложение в событие в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="758a0-120">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="758a0-121">Добавление вложения в сообщение</span><span class="sxs-lookup"><span data-stu-id="758a0-121">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="758a0-122">attachment</span><span class="sxs-lookup"><span data-stu-id="758a0-122">attachment</span></span>](attachment.md) |<span data-ttu-id="758a0-123">Добавление в сообщение файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="758a0-123">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="758a0-124">Добавление вложения к задаче Outlook</span><span class="sxs-lookup"><span data-stu-id="758a0-124">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="758a0-125">attachment</span><span class="sxs-lookup"><span data-stu-id="758a0-125">attachment</span></span>](attachment.md) |<span data-ttu-id="758a0-126">Добавление файла, элемента или ссылки на вложение к задаче Outlook.</span><span class="sxs-lookup"><span data-stu-id="758a0-126">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="758a0-127">Добавление вложения в запись</span><span class="sxs-lookup"><span data-stu-id="758a0-127">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="758a0-128">attachment</span><span class="sxs-lookup"><span data-stu-id="758a0-128">attachment</span></span>](attachment.md) |<span data-ttu-id="758a0-129">Добавление в запись файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="758a0-129">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="758a0-130">Список вложений пользовательского события</span><span class="sxs-lookup"><span data-stu-id="758a0-130">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="758a0-131">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="758a0-131">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="758a0-132">Получение списка вложений для события в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="758a0-132">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="758a0-133">Список вложений для сообщения</span><span class="sxs-lookup"><span data-stu-id="758a0-133">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="758a0-134">Коллекция [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="758a0-134">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="758a0-135">Получение списка вложений для сообщения.</span><span class="sxs-lookup"><span data-stu-id="758a0-135">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="758a0-136">Список вложений задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="758a0-136">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="758a0-137">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="758a0-137">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="758a0-138">Получение списка вложений для задачи Outlook.</span><span class="sxs-lookup"><span data-stu-id="758a0-138">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="758a0-139">Список вложений для записи</span><span class="sxs-lookup"><span data-stu-id="758a0-139">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="758a0-140">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="758a0-140">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="758a0-141">Получение списка вложений для записи.</span><span class="sxs-lookup"><span data-stu-id="758a0-141">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="758a0-142">Удаление</span><span class="sxs-lookup"><span data-stu-id="758a0-142">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="758a0-143">Нет</span><span class="sxs-lookup"><span data-stu-id="758a0-143">None</span></span> |<span data-ttu-id="758a0-144">Удаление вложения для события, сообщения, задачи Outlook или POST.</span><span class="sxs-lookup"><span data-stu-id="758a0-144">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="758a0-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="758a0-145">Properties</span></span>

<span data-ttu-id="758a0-p101">Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="758a0-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="758a0-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="758a0-148">Property</span></span>     | <span data-ttu-id="758a0-149">Тип</span><span class="sxs-lookup"><span data-stu-id="758a0-149">Type</span></span>   |<span data-ttu-id="758a0-150">Описание</span><span class="sxs-lookup"><span data-stu-id="758a0-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="758a0-151">contentType</span><span class="sxs-lookup"><span data-stu-id="758a0-151">contentType</span></span>|<span data-ttu-id="758a0-152">String</span><span class="sxs-lookup"><span data-stu-id="758a0-152">String</span></span>|<span data-ttu-id="758a0-153">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="758a0-153">The MIME type.</span></span>|
|<span data-ttu-id="758a0-154">id</span><span class="sxs-lookup"><span data-stu-id="758a0-154">id</span></span>|<span data-ttu-id="758a0-155">Строка</span><span class="sxs-lookup"><span data-stu-id="758a0-155">String</span></span>| <span data-ttu-id="758a0-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="758a0-156">Read-only.</span></span>|
|<span data-ttu-id="758a0-157">isInline</span><span class="sxs-lookup"><span data-stu-id="758a0-157">isInline</span></span>|<span data-ttu-id="758a0-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="758a0-158">Boolean</span></span>|<span data-ttu-id="758a0-159">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="758a0-159">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="758a0-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="758a0-160">lastModifiedDateTime</span></span>|<span data-ttu-id="758a0-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="758a0-161">DateTimeOffset</span></span>|<span data-ttu-id="758a0-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="758a0-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="758a0-164">имя</span><span class="sxs-lookup"><span data-stu-id="758a0-164">name</span></span>|<span data-ttu-id="758a0-165">String</span><span class="sxs-lookup"><span data-stu-id="758a0-165">String</span></span>|<span data-ttu-id="758a0-166">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="758a0-166">The display name of the attachment.</span></span> <span data-ttu-id="758a0-167">Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="758a0-167">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="758a0-168">size</span><span class="sxs-lookup"><span data-stu-id="758a0-168">size</span></span>|<span data-ttu-id="758a0-169">Int32</span><span class="sxs-lookup"><span data-stu-id="758a0-169">Int32</span></span>|<span data-ttu-id="758a0-170">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="758a0-170">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="758a0-171">Отношения</span><span class="sxs-lookup"><span data-stu-id="758a0-171">Relationships</span></span>
<span data-ttu-id="758a0-172">Нет</span><span class="sxs-lookup"><span data-stu-id="758a0-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="758a0-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="758a0-173">JSON representation</span></span>

<span data-ttu-id="758a0-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="758a0-174">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
