---
title: Тип ресурса attachment
description: Вы можете добавить связанное содержимое в экземпляр event,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: a71d7940e6825659143e69b2af6290f0671f59ae
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036100"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="e639a-103">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="e639a-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e639a-104">Вы можете добавить связанное содержимое для [события](../resources/event.md)пользователя, [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [записи](../resources/post.md) группы в виде вложения.</span><span class="sxs-lookup"><span data-stu-id="e639a-104">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="e639a-105">**attachment** — базовый ресурс для следующих производных типов вложений:</span><span class="sxs-lookup"><span data-stu-id="e639a-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="e639a-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="e639a-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="e639a-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="e639a-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="e639a-108">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="e639a-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

<span data-ttu-id="e639a-109">События в групповой календаре не поддерживают вложения.</span><span class="sxs-lookup"><span data-stu-id="e639a-109">Events in group calendars do not support attachments.</span></span>

## <a name="methods"></a><span data-ttu-id="e639a-110">Методы</span><span class="sxs-lookup"><span data-stu-id="e639a-110">Methods</span></span>

<span data-ttu-id="e639a-111">Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="e639a-111">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="e639a-112">Метод</span><span class="sxs-lookup"><span data-stu-id="e639a-112">Method</span></span>       | <span data-ttu-id="e639a-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e639a-113">Return Type</span></span>  |<span data-ttu-id="e639a-114">Описание</span><span class="sxs-lookup"><span data-stu-id="e639a-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e639a-115">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="e639a-115">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="e639a-116">attachment</span><span class="sxs-lookup"><span data-stu-id="e639a-116">attachment</span></span>](attachment.md) |<span data-ttu-id="e639a-117">Чтение свойств, связей или необработанного содержимого вложения, вложенного в пользовательское событие, сообщение, задачу Outlook или POST.</span><span class="sxs-lookup"><span data-stu-id="e639a-117">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="e639a-118">Добавление вложения в событие пользователя</span><span class="sxs-lookup"><span data-stu-id="e639a-118">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="e639a-119">attachment</span><span class="sxs-lookup"><span data-stu-id="e639a-119">attachment</span></span>](attachment.md) |<span data-ttu-id="e639a-120">Добавление файла, элемента или ссылки на вложение в событие в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="e639a-120">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="e639a-121">Добавление вложения в сообщение</span><span class="sxs-lookup"><span data-stu-id="e639a-121">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="e639a-122">attachment</span><span class="sxs-lookup"><span data-stu-id="e639a-122">attachment</span></span>](attachment.md) |<span data-ttu-id="e639a-123">Добавление в сообщение файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="e639a-123">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="e639a-124">Добавление вложения к задаче Outlook</span><span class="sxs-lookup"><span data-stu-id="e639a-124">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="e639a-125">attachment</span><span class="sxs-lookup"><span data-stu-id="e639a-125">attachment</span></span>](attachment.md) |<span data-ttu-id="e639a-126">Добавление файла, элемента или ссылки на вложение к задаче Outlook.</span><span class="sxs-lookup"><span data-stu-id="e639a-126">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="e639a-127">Добавление вложения в запись</span><span class="sxs-lookup"><span data-stu-id="e639a-127">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="e639a-128">attachment</span><span class="sxs-lookup"><span data-stu-id="e639a-128">attachment</span></span>](attachment.md) |<span data-ttu-id="e639a-129">Добавление в запись файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="e639a-129">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="e639a-130">Список вложений пользовательского события</span><span class="sxs-lookup"><span data-stu-id="e639a-130">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="e639a-131">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="e639a-131">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e639a-132">Получение списка вложений для события в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="e639a-132">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="e639a-133">Список вложений для сообщения</span><span class="sxs-lookup"><span data-stu-id="e639a-133">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="e639a-134">Коллекция [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="e639a-134">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e639a-135">Получение списка вложений для сообщения.</span><span class="sxs-lookup"><span data-stu-id="e639a-135">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="e639a-136">Список вложений задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="e639a-136">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="e639a-137">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="e639a-137">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e639a-138">Получение списка вложений для задачи Outlook.</span><span class="sxs-lookup"><span data-stu-id="e639a-138">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="e639a-139">Список вложений для записи</span><span class="sxs-lookup"><span data-stu-id="e639a-139">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="e639a-140">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="e639a-140">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e639a-141">Получение списка вложений для записи.</span><span class="sxs-lookup"><span data-stu-id="e639a-141">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="e639a-142">Удаление</span><span class="sxs-lookup"><span data-stu-id="e639a-142">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="e639a-143">Нет</span><span class="sxs-lookup"><span data-stu-id="e639a-143">None</span></span> |<span data-ttu-id="e639a-144">Удаление вложения для события, сообщения, задачи Outlook или POST.</span><span class="sxs-lookup"><span data-stu-id="e639a-144">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="e639a-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="e639a-145">Properties</span></span>

<span data-ttu-id="e639a-p101">Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="e639a-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="e639a-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="e639a-148">Property</span></span>     | <span data-ttu-id="e639a-149">Тип</span><span class="sxs-lookup"><span data-stu-id="e639a-149">Type</span></span>   |<span data-ttu-id="e639a-150">Описание</span><span class="sxs-lookup"><span data-stu-id="e639a-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e639a-151">contentType</span><span class="sxs-lookup"><span data-stu-id="e639a-151">contentType</span></span>|<span data-ttu-id="e639a-152">String</span><span class="sxs-lookup"><span data-stu-id="e639a-152">String</span></span>|<span data-ttu-id="e639a-153">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="e639a-153">The MIME type.</span></span>|
|<span data-ttu-id="e639a-154">id</span><span class="sxs-lookup"><span data-stu-id="e639a-154">id</span></span>|<span data-ttu-id="e639a-155">Строка</span><span class="sxs-lookup"><span data-stu-id="e639a-155">String</span></span>| <span data-ttu-id="e639a-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e639a-156">Read-only.</span></span>|
|<span data-ttu-id="e639a-157">isInline</span><span class="sxs-lookup"><span data-stu-id="e639a-157">isInline</span></span>|<span data-ttu-id="e639a-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="e639a-158">Boolean</span></span>|<span data-ttu-id="e639a-159">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="e639a-159">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="e639a-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e639a-160">lastModifiedDateTime</span></span>|<span data-ttu-id="e639a-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e639a-161">DateTimeOffset</span></span>|<span data-ttu-id="e639a-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e639a-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e639a-164">имя</span><span class="sxs-lookup"><span data-stu-id="e639a-164">name</span></span>|<span data-ttu-id="e639a-165">String</span><span class="sxs-lookup"><span data-stu-id="e639a-165">String</span></span>|<span data-ttu-id="e639a-166">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="e639a-166">The display name of the attachment.</span></span> <span data-ttu-id="e639a-167">Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="e639a-167">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="e639a-168">size</span><span class="sxs-lookup"><span data-stu-id="e639a-168">size</span></span>|<span data-ttu-id="e639a-169">Int32</span><span class="sxs-lookup"><span data-stu-id="e639a-169">Int32</span></span>|<span data-ttu-id="e639a-170">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="e639a-170">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e639a-171">Отношения</span><span class="sxs-lookup"><span data-stu-id="e639a-171">Relationships</span></span>
<span data-ttu-id="e639a-172">Нет</span><span class="sxs-lookup"><span data-stu-id="e639a-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e639a-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e639a-173">JSON representation</span></span>

<span data-ttu-id="e639a-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e639a-174">Here is a JSON representation of the resource</span></span>

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
