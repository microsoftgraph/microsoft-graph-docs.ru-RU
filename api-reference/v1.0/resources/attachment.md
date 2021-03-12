---
title: Тип ресурса attachment
description: Вы можете добавить связанное содержимое в экземпляр event,
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e82ce58786e23448458e9e1c60fad5d0c54b6388
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722435"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="4bdbd-103">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="4bdbd-103">attachment resource type</span></span>

<span data-ttu-id="4bdbd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bdbd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4bdbd-105">Вы можете добавить связанное содержимое в экземпляр [event](../resources/event.md), [message](../resources/message.md) или [post](../resources/post.md) в форме вложения.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-105">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="4bdbd-106">**attachment** — базовый ресурс для следующих производных типов вложений:</span><span class="sxs-lookup"><span data-stu-id="4bdbd-106">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="4bdbd-107">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="4bdbd-107">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="4bdbd-108">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="4bdbd-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="4bdbd-109">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="4bdbd-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

<span data-ttu-id="4bdbd-110">События в календарях группы не поддерживают вложения.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-110">Events in group calendars do not support attachments.</span></span>

## <a name="methods"></a><span data-ttu-id="4bdbd-111">Методы</span><span class="sxs-lookup"><span data-stu-id="4bdbd-111">Methods</span></span>

<span data-ttu-id="4bdbd-112">Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="4bdbd-112">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="4bdbd-113">Метод</span><span class="sxs-lookup"><span data-stu-id="4bdbd-113">Method</span></span>       | <span data-ttu-id="4bdbd-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4bdbd-114">Return Type</span></span>  |<span data-ttu-id="4bdbd-115">Описание</span><span class="sxs-lookup"><span data-stu-id="4bdbd-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4bdbd-116">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="4bdbd-116">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="4bdbd-117">attachment</span><span class="sxs-lookup"><span data-stu-id="4bdbd-117">attachment</span></span>](attachment.md) |<span data-ttu-id="4bdbd-118">Чтение свойств, связей или необработанного содержимого объекта, представляющего вложение, которое было добавлено к пользовательскому событию, сообщению или записи.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-118">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, or post.</span></span>|
|[<span data-ttu-id="4bdbd-119">Добавление вложения в пользовательское событие</span><span class="sxs-lookup"><span data-stu-id="4bdbd-119">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="4bdbd-120">attachment</span><span class="sxs-lookup"><span data-stu-id="4bdbd-120">attachment</span></span>](attachment.md) |<span data-ttu-id="4bdbd-121">Добавление файла, элемента или вложения-ссылки в качестве события в пользовательском календаре.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-121">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="4bdbd-122">Добавление вложения в сообщение</span><span class="sxs-lookup"><span data-stu-id="4bdbd-122">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="4bdbd-123">attachment</span><span class="sxs-lookup"><span data-stu-id="4bdbd-123">attachment</span></span>](attachment.md) |<span data-ttu-id="4bdbd-124">Добавление в сообщение файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-124">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="4bdbd-125">Добавление вложения в запись</span><span class="sxs-lookup"><span data-stu-id="4bdbd-125">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="4bdbd-126">attachment</span><span class="sxs-lookup"><span data-stu-id="4bdbd-126">attachment</span></span>](attachment.md) |<span data-ttu-id="4bdbd-127">Добавление в запись файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-127">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="4bdbd-128">Список вложений пользовательского события</span><span class="sxs-lookup"><span data-stu-id="4bdbd-128">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="4bdbd-129">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="4bdbd-129">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="4bdbd-130">Получение списка вложений для события в пользовательском календаре.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-130">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="4bdbd-131">Список вложений для сообщения</span><span class="sxs-lookup"><span data-stu-id="4bdbd-131">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="4bdbd-132">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="4bdbd-132">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="4bdbd-133">Получение списка вложений для сообщения.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-133">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="4bdbd-134">Список вложений для записи</span><span class="sxs-lookup"><span data-stu-id="4bdbd-134">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="4bdbd-135">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="4bdbd-135">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="4bdbd-136">Получение списка вложений для записи.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-136">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="4bdbd-137">Удаление</span><span class="sxs-lookup"><span data-stu-id="4bdbd-137">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="4bdbd-138">Нет</span><span class="sxs-lookup"><span data-stu-id="4bdbd-138">None</span></span> |<span data-ttu-id="4bdbd-139">Удаление объекта, представляющего вложение, которое было добавлено к сообщению, записи или данным о событии.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-139">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="4bdbd-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="4bdbd-140">Properties</span></span>

<span data-ttu-id="4bdbd-p101">Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="4bdbd-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="4bdbd-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bdbd-143">Property</span></span>     | <span data-ttu-id="4bdbd-144">Тип</span><span class="sxs-lookup"><span data-stu-id="4bdbd-144">Type</span></span>   |<span data-ttu-id="4bdbd-145">Описание</span><span class="sxs-lookup"><span data-stu-id="4bdbd-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bdbd-146">contentType</span><span class="sxs-lookup"><span data-stu-id="4bdbd-146">contentType</span></span>|<span data-ttu-id="4bdbd-147">String</span><span class="sxs-lookup"><span data-stu-id="4bdbd-147">String</span></span>|<span data-ttu-id="4bdbd-148">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-148">The MIME type.</span></span>|
|<span data-ttu-id="4bdbd-149">id</span><span class="sxs-lookup"><span data-stu-id="4bdbd-149">id</span></span>|<span data-ttu-id="4bdbd-150">String</span><span class="sxs-lookup"><span data-stu-id="4bdbd-150">String</span></span>| <span data-ttu-id="4bdbd-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-151">Read-only.</span></span>|
|<span data-ttu-id="4bdbd-152">isInline</span><span class="sxs-lookup"><span data-stu-id="4bdbd-152">isInline</span></span>|<span data-ttu-id="4bdbd-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bdbd-153">Boolean</span></span>|<span data-ttu-id="4bdbd-154">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-154">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="4bdbd-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4bdbd-155">lastModifiedDateTime</span></span>|<span data-ttu-id="4bdbd-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bdbd-156">DateTimeOffset</span></span>|<span data-ttu-id="4bdbd-157">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4bdbd-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4bdbd-158">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-158">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="4bdbd-159">name</span><span class="sxs-lookup"><span data-stu-id="4bdbd-159">name</span></span>|<span data-ttu-id="4bdbd-160">String</span><span class="sxs-lookup"><span data-stu-id="4bdbd-160">String</span></span>|<span data-ttu-id="4bdbd-161">Имя вложенного файла.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-161">The attachment's file name.</span></span>|
|<span data-ttu-id="4bdbd-162">size</span><span class="sxs-lookup"><span data-stu-id="4bdbd-162">size</span></span>|<span data-ttu-id="4bdbd-163">Int32</span><span class="sxs-lookup"><span data-stu-id="4bdbd-163">Int32</span></span>|<span data-ttu-id="4bdbd-164">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-164">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bdbd-165">Отношения</span><span class="sxs-lookup"><span data-stu-id="4bdbd-165">Relationships</span></span>
<span data-ttu-id="4bdbd-166">Нет</span><span class="sxs-lookup"><span data-stu-id="4bdbd-166">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4bdbd-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4bdbd-167">JSON representation</span></span>

<span data-ttu-id="4bdbd-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-168">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "abstract": true,
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

