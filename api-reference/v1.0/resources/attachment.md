---
title: Тип ресурса attachment
description: Связанное содержимое можно добавить на событие
localization_priority: Priority
ms.openlocfilehash: 284895871a0c6a80140ff248045b89d2de104c20
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892332"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="1eb06-103">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="1eb06-103">attachment resource type</span></span>

<span data-ttu-id="1eb06-104">Вы можете добавить связанное содержимое в экземпляр [event](../resources/event.md), [message](../resources/message.md) или [post](../resources/post.md) в форме вложения.</span><span class="sxs-lookup"><span data-stu-id="1eb06-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="1eb06-105">**attachment** — базовый ресурс для следующих производных типов вложений:</span><span class="sxs-lookup"><span data-stu-id="1eb06-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="1eb06-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="1eb06-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="1eb06-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="1eb06-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="1eb06-108">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="1eb06-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>


## <a name="methods"></a><span data-ttu-id="1eb06-109">Методы</span><span class="sxs-lookup"><span data-stu-id="1eb06-109">Methods</span></span>

<span data-ttu-id="1eb06-110">Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="1eb06-110">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="1eb06-111">Метод</span><span class="sxs-lookup"><span data-stu-id="1eb06-111">Method</span></span>       | <span data-ttu-id="1eb06-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1eb06-112">Return Type</span></span>  |<span data-ttu-id="1eb06-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1eb06-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1eb06-114">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="1eb06-114">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="1eb06-115">attachment</span><span class="sxs-lookup"><span data-stu-id="1eb06-115">attachment</span></span>](attachment.md) |<span data-ttu-id="1eb06-116">Чтение свойств и связей объекта, представляющего вложение, которое было добавлено к сообщению, записи или данным о событии.</span><span class="sxs-lookup"><span data-stu-id="1eb06-116">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="1eb06-117">Добавление вложения к данным о событии</span><span class="sxs-lookup"><span data-stu-id="1eb06-117">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="1eb06-118">attachment</span><span class="sxs-lookup"><span data-stu-id="1eb06-118">attachment</span></span>](attachment.md) |<span data-ttu-id="1eb06-119">Добавление для события файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="1eb06-119">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="1eb06-120">Добавление вложения в сообщение</span><span class="sxs-lookup"><span data-stu-id="1eb06-120">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="1eb06-121">attachment</span><span class="sxs-lookup"><span data-stu-id="1eb06-121">attachment</span></span>](attachment.md) |<span data-ttu-id="1eb06-122">Добавление в сообщение файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="1eb06-122">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="1eb06-123">Добавление вложения в запись</span><span class="sxs-lookup"><span data-stu-id="1eb06-123">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="1eb06-124">attachment</span><span class="sxs-lookup"><span data-stu-id="1eb06-124">attachment</span></span>](attachment.md) |<span data-ttu-id="1eb06-125">Добавление в запись файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="1eb06-125">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="1eb06-126">Список вложений для события</span><span class="sxs-lookup"><span data-stu-id="1eb06-126">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="1eb06-127">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="1eb06-127">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="1eb06-128">Получение списка вложений для события.</span><span class="sxs-lookup"><span data-stu-id="1eb06-128">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="1eb06-129">Список вложений для сообщения</span><span class="sxs-lookup"><span data-stu-id="1eb06-129">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="1eb06-130">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="1eb06-130">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="1eb06-131">Получение списка вложений для сообщения.</span><span class="sxs-lookup"><span data-stu-id="1eb06-131">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="1eb06-132">Список вложений для записи</span><span class="sxs-lookup"><span data-stu-id="1eb06-132">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="1eb06-133">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="1eb06-133">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="1eb06-134">Получение списка вложений для записи.</span><span class="sxs-lookup"><span data-stu-id="1eb06-134">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="1eb06-135">Удаление</span><span class="sxs-lookup"><span data-stu-id="1eb06-135">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="1eb06-136">Нет</span><span class="sxs-lookup"><span data-stu-id="1eb06-136">None</span></span> |<span data-ttu-id="1eb06-137">Удаление объекта, представляющего вложение, которое было добавлено к сообщению, записи или данным о событии.</span><span class="sxs-lookup"><span data-stu-id="1eb06-137">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="1eb06-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="1eb06-138">Properties</span></span>

<span data-ttu-id="1eb06-p101">Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="1eb06-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="1eb06-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="1eb06-141">Property</span></span>     | <span data-ttu-id="1eb06-142">Тип</span><span class="sxs-lookup"><span data-stu-id="1eb06-142">Type</span></span>   |<span data-ttu-id="1eb06-143">Описание</span><span class="sxs-lookup"><span data-stu-id="1eb06-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1eb06-144">contentType</span><span class="sxs-lookup"><span data-stu-id="1eb06-144">contentType</span></span>|<span data-ttu-id="1eb06-145">String</span><span class="sxs-lookup"><span data-stu-id="1eb06-145">String</span></span>|<span data-ttu-id="1eb06-146">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="1eb06-146">The MIME type.</span></span>|
|<span data-ttu-id="1eb06-147">id</span><span class="sxs-lookup"><span data-stu-id="1eb06-147">id</span></span>|<span data-ttu-id="1eb06-148">Строка</span><span class="sxs-lookup"><span data-stu-id="1eb06-148">String</span></span>| <span data-ttu-id="1eb06-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1eb06-149">Read-only.</span></span>|
|<span data-ttu-id="1eb06-150">isInline</span><span class="sxs-lookup"><span data-stu-id="1eb06-150">isInline</span></span>|<span data-ttu-id="1eb06-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="1eb06-151">Boolean</span></span>|<span data-ttu-id="1eb06-152">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="1eb06-152">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="1eb06-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1eb06-153">lastModifiedDateTime</span></span>|<span data-ttu-id="1eb06-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1eb06-154">DateTimeOffset</span></span>|<span data-ttu-id="1eb06-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1eb06-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1eb06-157">имя</span><span class="sxs-lookup"><span data-stu-id="1eb06-157">name</span></span>|<span data-ttu-id="1eb06-158">String</span><span class="sxs-lookup"><span data-stu-id="1eb06-158">String</span></span>|<span data-ttu-id="1eb06-159">Имя вложенного файла.</span><span class="sxs-lookup"><span data-stu-id="1eb06-159">The attachment's file name.</span></span>|
|<span data-ttu-id="1eb06-160">size</span><span class="sxs-lookup"><span data-stu-id="1eb06-160">size</span></span>|<span data-ttu-id="1eb06-161">Int32</span><span class="sxs-lookup"><span data-stu-id="1eb06-161">Int32</span></span>|<span data-ttu-id="1eb06-162">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="1eb06-162">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1eb06-163">Отношения</span><span class="sxs-lookup"><span data-stu-id="1eb06-163">Relationships</span></span>
<span data-ttu-id="1eb06-164">Нет</span><span class="sxs-lookup"><span data-stu-id="1eb06-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1eb06-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1eb06-165">JSON representation</span></span>

<span data-ttu-id="1eb06-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1eb06-166">Here is a JSON representation of the resource</span></span>

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
