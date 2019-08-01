---
title: Тип ресурса attachment
description: Вы можете добавить связанное содержимое в экземпляр event,
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d47fde49a76f00658e39d9a3ae6629cd9bcf56b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030074"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="3562f-103">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="3562f-103">attachment resource type</span></span>

<span data-ttu-id="3562f-104">Вы можете добавить связанное содержимое в экземпляр [event](../resources/event.md), [message](../resources/message.md) или [post](../resources/post.md) в форме вложения.</span><span class="sxs-lookup"><span data-stu-id="3562f-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="3562f-105">**attachment** — базовый ресурс для следующих производных типов вложений:</span><span class="sxs-lookup"><span data-stu-id="3562f-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="3562f-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="3562f-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="3562f-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="3562f-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="3562f-108">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="3562f-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>


## <a name="methods"></a><span data-ttu-id="3562f-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3562f-109">Methods</span></span>

<span data-ttu-id="3562f-110">Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="3562f-110">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="3562f-111">Метод</span><span class="sxs-lookup"><span data-stu-id="3562f-111">Method</span></span>       | <span data-ttu-id="3562f-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3562f-112">Return Type</span></span>  |<span data-ttu-id="3562f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="3562f-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3562f-114">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="3562f-114">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="3562f-115">attachment</span><span class="sxs-lookup"><span data-stu-id="3562f-115">attachment</span></span>](attachment.md) |<span data-ttu-id="3562f-116">Чтение свойств и связей объекта, представляющего вложение, которое было добавлено к сообщению, записи или данным о событии.</span><span class="sxs-lookup"><span data-stu-id="3562f-116">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="3562f-117">Добавление вложения к данным о событии</span><span class="sxs-lookup"><span data-stu-id="3562f-117">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="3562f-118">attachment</span><span class="sxs-lookup"><span data-stu-id="3562f-118">attachment</span></span>](attachment.md) |<span data-ttu-id="3562f-119">Добавление для события файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="3562f-119">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="3562f-120">Добавление вложения в сообщение</span><span class="sxs-lookup"><span data-stu-id="3562f-120">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="3562f-121">attachment</span><span class="sxs-lookup"><span data-stu-id="3562f-121">attachment</span></span>](attachment.md) |<span data-ttu-id="3562f-122">Добавление в сообщение файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="3562f-122">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="3562f-123">Добавление вложения в запись</span><span class="sxs-lookup"><span data-stu-id="3562f-123">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="3562f-124">attachment</span><span class="sxs-lookup"><span data-stu-id="3562f-124">attachment</span></span>](attachment.md) |<span data-ttu-id="3562f-125">Добавление в запись файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="3562f-125">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="3562f-126">Список вложений для события</span><span class="sxs-lookup"><span data-stu-id="3562f-126">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="3562f-127">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="3562f-127">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="3562f-128">Получение списка вложений для события.</span><span class="sxs-lookup"><span data-stu-id="3562f-128">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="3562f-129">Список вложений для сообщения</span><span class="sxs-lookup"><span data-stu-id="3562f-129">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="3562f-130">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="3562f-130">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="3562f-131">Получение списка вложений для сообщения.</span><span class="sxs-lookup"><span data-stu-id="3562f-131">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="3562f-132">Список вложений для записи</span><span class="sxs-lookup"><span data-stu-id="3562f-132">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="3562f-133">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="3562f-133">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="3562f-134">Получение списка вложений для записи.</span><span class="sxs-lookup"><span data-stu-id="3562f-134">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="3562f-135">Удаление</span><span class="sxs-lookup"><span data-stu-id="3562f-135">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="3562f-136">Нет</span><span class="sxs-lookup"><span data-stu-id="3562f-136">None</span></span> |<span data-ttu-id="3562f-137">Удаление объекта, представляющего вложение, которое было добавлено к сообщению, записи или данным о событии.</span><span class="sxs-lookup"><span data-stu-id="3562f-137">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="3562f-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="3562f-138">Properties</span></span>

<span data-ttu-id="3562f-p101">Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="3562f-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="3562f-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="3562f-141">Property</span></span>     | <span data-ttu-id="3562f-142">Тип</span><span class="sxs-lookup"><span data-stu-id="3562f-142">Type</span></span>   |<span data-ttu-id="3562f-143">Описание</span><span class="sxs-lookup"><span data-stu-id="3562f-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3562f-144">contentType</span><span class="sxs-lookup"><span data-stu-id="3562f-144">contentType</span></span>|<span data-ttu-id="3562f-145">String</span><span class="sxs-lookup"><span data-stu-id="3562f-145">String</span></span>|<span data-ttu-id="3562f-146">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="3562f-146">The MIME type.</span></span>|
|<span data-ttu-id="3562f-147">id</span><span class="sxs-lookup"><span data-stu-id="3562f-147">id</span></span>|<span data-ttu-id="3562f-148">String</span><span class="sxs-lookup"><span data-stu-id="3562f-148">String</span></span>| <span data-ttu-id="3562f-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3562f-149">Read-only.</span></span>|
|<span data-ttu-id="3562f-150">isInline</span><span class="sxs-lookup"><span data-stu-id="3562f-150">isInline</span></span>|<span data-ttu-id="3562f-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="3562f-151">Boolean</span></span>|<span data-ttu-id="3562f-152">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="3562f-152">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="3562f-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3562f-153">lastModifiedDateTime</span></span>|<span data-ttu-id="3562f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3562f-154">DateTimeOffset</span></span>|<span data-ttu-id="3562f-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3562f-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3562f-157">имя</span><span class="sxs-lookup"><span data-stu-id="3562f-157">name</span></span>|<span data-ttu-id="3562f-158">String</span><span class="sxs-lookup"><span data-stu-id="3562f-158">String</span></span>|<span data-ttu-id="3562f-159">Имя вложенного файла.</span><span class="sxs-lookup"><span data-stu-id="3562f-159">The attachment's file name.</span></span>|
|<span data-ttu-id="3562f-160">size</span><span class="sxs-lookup"><span data-stu-id="3562f-160">size</span></span>|<span data-ttu-id="3562f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="3562f-161">Int32</span></span>|<span data-ttu-id="3562f-162">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="3562f-162">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3562f-163">Отношения</span><span class="sxs-lookup"><span data-stu-id="3562f-163">Relationships</span></span>
<span data-ttu-id="3562f-164">Нет</span><span class="sxs-lookup"><span data-stu-id="3562f-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3562f-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3562f-165">JSON representation</span></span>

<span data-ttu-id="3562f-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3562f-166">Here is a JSON representation of the resource</span></span>

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
