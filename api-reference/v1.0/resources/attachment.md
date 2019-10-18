---
title: Тип ресурса attachment
description: Вы можете добавить связанное содержимое в экземпляр event,
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c7bf5eef63921f1cc3fab985f4832177767fe1fc
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036076"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="01463-103">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="01463-103">attachment resource type</span></span>

<span data-ttu-id="01463-104">Вы можете добавить связанное содержимое в экземпляр [event](../resources/event.md), [message](../resources/message.md) или [post](../resources/post.md) в форме вложения.</span><span class="sxs-lookup"><span data-stu-id="01463-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="01463-105">**attachment** — базовый ресурс для следующих производных типов вложений:</span><span class="sxs-lookup"><span data-stu-id="01463-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="01463-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="01463-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="01463-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="01463-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="01463-108">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="01463-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

<span data-ttu-id="01463-109">События в календарях группы не поддерживают вложения.</span><span class="sxs-lookup"><span data-stu-id="01463-109">Events in group calendars do not support attachments.</span></span>

## <a name="methods"></a><span data-ttu-id="01463-110">Методы</span><span class="sxs-lookup"><span data-stu-id="01463-110">Methods</span></span>

<span data-ttu-id="01463-111">Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="01463-111">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="01463-112">Метод</span><span class="sxs-lookup"><span data-stu-id="01463-112">Method</span></span>       | <span data-ttu-id="01463-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="01463-113">Return Type</span></span>  |<span data-ttu-id="01463-114">Описание</span><span class="sxs-lookup"><span data-stu-id="01463-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="01463-115">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="01463-115">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="01463-116">attachment</span><span class="sxs-lookup"><span data-stu-id="01463-116">attachment</span></span>](attachment.md) |<span data-ttu-id="01463-117">Чтение свойств, связей или необработанного содержимого объекта, представляющего вложение, которое было добавлено к пользовательскому событию, сообщению или записи.</span><span class="sxs-lookup"><span data-stu-id="01463-117">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="01463-118">Добавление вложения в пользовательское событие</span><span class="sxs-lookup"><span data-stu-id="01463-118">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="01463-119">attachment</span><span class="sxs-lookup"><span data-stu-id="01463-119">attachment</span></span>](attachment.md) |<span data-ttu-id="01463-120">Добавление файла, элемента или вложения-ссылки в качестве события в пользовательском календаре.</span><span class="sxs-lookup"><span data-stu-id="01463-120">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="01463-121">Добавление вложения в сообщение</span><span class="sxs-lookup"><span data-stu-id="01463-121">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="01463-122">attachment</span><span class="sxs-lookup"><span data-stu-id="01463-122">attachment</span></span>](attachment.md) |<span data-ttu-id="01463-123">Добавление в сообщение файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="01463-123">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="01463-124">Добавление вложения в запись</span><span class="sxs-lookup"><span data-stu-id="01463-124">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="01463-125">attachment</span><span class="sxs-lookup"><span data-stu-id="01463-125">attachment</span></span>](attachment.md) |<span data-ttu-id="01463-126">Добавление в запись файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="01463-126">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="01463-127">Список вложений пользовательского события</span><span class="sxs-lookup"><span data-stu-id="01463-127">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="01463-128">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="01463-128">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="01463-129">Получение списка вложений для события в пользовательском календаре.</span><span class="sxs-lookup"><span data-stu-id="01463-129">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="01463-130">Список вложений для сообщения</span><span class="sxs-lookup"><span data-stu-id="01463-130">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="01463-131">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="01463-131">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="01463-132">Получение списка вложений для сообщения.</span><span class="sxs-lookup"><span data-stu-id="01463-132">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="01463-133">Список вложений для записи</span><span class="sxs-lookup"><span data-stu-id="01463-133">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="01463-134">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="01463-134">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="01463-135">Получение списка вложений для записи.</span><span class="sxs-lookup"><span data-stu-id="01463-135">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="01463-136">Удаление</span><span class="sxs-lookup"><span data-stu-id="01463-136">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="01463-137">Нет</span><span class="sxs-lookup"><span data-stu-id="01463-137">None</span></span> |<span data-ttu-id="01463-138">Удаление объекта, представляющего вложение, которое было добавлено к сообщению, записи или данным о событии.</span><span class="sxs-lookup"><span data-stu-id="01463-138">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="01463-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="01463-139">Properties</span></span>

<span data-ttu-id="01463-p101">Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="01463-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="01463-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="01463-142">Property</span></span>     | <span data-ttu-id="01463-143">Тип</span><span class="sxs-lookup"><span data-stu-id="01463-143">Type</span></span>   |<span data-ttu-id="01463-144">Описание</span><span class="sxs-lookup"><span data-stu-id="01463-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01463-145">contentType</span><span class="sxs-lookup"><span data-stu-id="01463-145">contentType</span></span>|<span data-ttu-id="01463-146">String</span><span class="sxs-lookup"><span data-stu-id="01463-146">String</span></span>|<span data-ttu-id="01463-147">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="01463-147">The MIME type.</span></span>|
|<span data-ttu-id="01463-148">id</span><span class="sxs-lookup"><span data-stu-id="01463-148">id</span></span>|<span data-ttu-id="01463-149">String</span><span class="sxs-lookup"><span data-stu-id="01463-149">String</span></span>| <span data-ttu-id="01463-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01463-150">Read-only.</span></span>|
|<span data-ttu-id="01463-151">isInline</span><span class="sxs-lookup"><span data-stu-id="01463-151">isInline</span></span>|<span data-ttu-id="01463-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="01463-152">Boolean</span></span>|<span data-ttu-id="01463-153">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="01463-153">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="01463-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01463-154">lastModifiedDateTime</span></span>|<span data-ttu-id="01463-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01463-155">DateTimeOffset</span></span>|<span data-ttu-id="01463-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="01463-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="01463-158">имя</span><span class="sxs-lookup"><span data-stu-id="01463-158">name</span></span>|<span data-ttu-id="01463-159">String</span><span class="sxs-lookup"><span data-stu-id="01463-159">String</span></span>|<span data-ttu-id="01463-160">Имя вложенного файла.</span><span class="sxs-lookup"><span data-stu-id="01463-160">The attachment's file name.</span></span>|
|<span data-ttu-id="01463-161">size</span><span class="sxs-lookup"><span data-stu-id="01463-161">size</span></span>|<span data-ttu-id="01463-162">Int32</span><span class="sxs-lookup"><span data-stu-id="01463-162">Int32</span></span>|<span data-ttu-id="01463-163">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="01463-163">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01463-164">Отношения</span><span class="sxs-lookup"><span data-stu-id="01463-164">Relationships</span></span>
<span data-ttu-id="01463-165">Нет</span><span class="sxs-lookup"><span data-stu-id="01463-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01463-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01463-166">JSON representation</span></span>

<span data-ttu-id="01463-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01463-167">Here is a JSON representation of the resource</span></span>

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
