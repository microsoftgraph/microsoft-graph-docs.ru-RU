---
title: Тип ресурса attachment
description: Вы можете добавить связанное содержимое в событие,
localization_priority: Normal
ms.openlocfilehash: 59e1074cea9508af45cef0b6e61ea223a3ca851e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535599"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="e48e0-103">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="e48e0-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e48e0-104">Вы можете добавить связанное содержимое к [](../resources/event.md)событию [](../resources/message.md), сообщению, [задаче Outlook](../resources/outlooktask.md)или [публикации](../resources/post.md) в виде вложения.</span><span class="sxs-lookup"><span data-stu-id="e48e0-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="e48e0-105">**attachment** — базовый ресурс для следующих производных типов вложений:</span><span class="sxs-lookup"><span data-stu-id="e48e0-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="e48e0-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="e48e0-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="e48e0-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="e48e0-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="e48e0-108">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="e48e0-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="e48e0-109">Методы</span><span class="sxs-lookup"><span data-stu-id="e48e0-109">Methods</span></span>

<span data-ttu-id="e48e0-110">Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="e48e0-110">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="e48e0-111">Метод</span><span class="sxs-lookup"><span data-stu-id="e48e0-111">Method</span></span>       | <span data-ttu-id="e48e0-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e48e0-112">Return Type</span></span>  |<span data-ttu-id="e48e0-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e48e0-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e48e0-114">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="e48e0-114">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="e48e0-115">attachment</span><span class="sxs-lookup"><span data-stu-id="e48e0-115">attachment</span></span>](attachment.md) |<span data-ttu-id="e48e0-116">Считывание свойств и связей вложений, вложенных в событие, сообщение, задачу Outlook или POST.</span><span class="sxs-lookup"><span data-stu-id="e48e0-116">Read the properties and relationships of an attachment, attached to an event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="e48e0-117">Добавление вложения к данным о событии</span><span class="sxs-lookup"><span data-stu-id="e48e0-117">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="e48e0-118">attachment</span><span class="sxs-lookup"><span data-stu-id="e48e0-118">attachment</span></span>](attachment.md) |<span data-ttu-id="e48e0-119">Добавление для события файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="e48e0-119">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="e48e0-120">Добавление вложения в сообщение</span><span class="sxs-lookup"><span data-stu-id="e48e0-120">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="e48e0-121">attachment</span><span class="sxs-lookup"><span data-stu-id="e48e0-121">attachment</span></span>](attachment.md) |<span data-ttu-id="e48e0-122">Добавление в сообщение файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="e48e0-122">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="e48e0-123">Добавление вложения к задаче Outlook</span><span class="sxs-lookup"><span data-stu-id="e48e0-123">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="e48e0-124">attachment</span><span class="sxs-lookup"><span data-stu-id="e48e0-124">attachment</span></span>](attachment.md) |<span data-ttu-id="e48e0-125">Добавление файла, элемента или ссылки на вложение к задаче Outlook.</span><span class="sxs-lookup"><span data-stu-id="e48e0-125">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="e48e0-126">Добавление вложения в запись</span><span class="sxs-lookup"><span data-stu-id="e48e0-126">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="e48e0-127">attachment</span><span class="sxs-lookup"><span data-stu-id="e48e0-127">attachment</span></span>](attachment.md) |<span data-ttu-id="e48e0-128">Добавление в запись файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="e48e0-128">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="e48e0-129">Список вложений для события</span><span class="sxs-lookup"><span data-stu-id="e48e0-129">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="e48e0-130">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="e48e0-130">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e48e0-131">Получение списка вложений для события.</span><span class="sxs-lookup"><span data-stu-id="e48e0-131">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="e48e0-132">Список вложений для сообщения</span><span class="sxs-lookup"><span data-stu-id="e48e0-132">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="e48e0-133">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="e48e0-133">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e48e0-134">Получение списка вложений для сообщения.</span><span class="sxs-lookup"><span data-stu-id="e48e0-134">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="e48e0-135">Список вложений задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="e48e0-135">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="e48e0-136">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="e48e0-136">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e48e0-137">Получение списка вложений для задачи Outlook.</span><span class="sxs-lookup"><span data-stu-id="e48e0-137">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="e48e0-138">Список вложений для записи</span><span class="sxs-lookup"><span data-stu-id="e48e0-138">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="e48e0-139">Коллекция [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="e48e0-139">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e48e0-140">Получение списка вложений для записи.</span><span class="sxs-lookup"><span data-stu-id="e48e0-140">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="e48e0-141">Удаление</span><span class="sxs-lookup"><span data-stu-id="e48e0-141">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="e48e0-142">Нет</span><span class="sxs-lookup"><span data-stu-id="e48e0-142">None</span></span> |<span data-ttu-id="e48e0-143">Удаление вложения для события, сообщения, задачи Outlook или POST.</span><span class="sxs-lookup"><span data-stu-id="e48e0-143">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="e48e0-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="e48e0-144">Properties</span></span>

<span data-ttu-id="e48e0-p101">Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="e48e0-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="e48e0-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="e48e0-147">Property</span></span>     | <span data-ttu-id="e48e0-148">Тип</span><span class="sxs-lookup"><span data-stu-id="e48e0-148">Type</span></span>   |<span data-ttu-id="e48e0-149">Описание</span><span class="sxs-lookup"><span data-stu-id="e48e0-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e48e0-150">contentType</span><span class="sxs-lookup"><span data-stu-id="e48e0-150">contentType</span></span>|<span data-ttu-id="e48e0-151">String</span><span class="sxs-lookup"><span data-stu-id="e48e0-151">String</span></span>|<span data-ttu-id="e48e0-152">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="e48e0-152">The MIME type.</span></span>|
|<span data-ttu-id="e48e0-153">id</span><span class="sxs-lookup"><span data-stu-id="e48e0-153">id</span></span>|<span data-ttu-id="e48e0-154">String</span><span class="sxs-lookup"><span data-stu-id="e48e0-154">String</span></span>| <span data-ttu-id="e48e0-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e48e0-155">Read-only.</span></span>|
|<span data-ttu-id="e48e0-156">isInline</span><span class="sxs-lookup"><span data-stu-id="e48e0-156">isInline</span></span>|<span data-ttu-id="e48e0-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="e48e0-157">Boolean</span></span>|<span data-ttu-id="e48e0-158">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="e48e0-158">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="e48e0-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e48e0-159">lastModifiedDateTime</span></span>|<span data-ttu-id="e48e0-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e48e0-160">DateTimeOffset</span></span>|<span data-ttu-id="e48e0-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e48e0-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e48e0-163">name</span><span class="sxs-lookup"><span data-stu-id="e48e0-163">name</span></span>|<span data-ttu-id="e48e0-164">String</span><span class="sxs-lookup"><span data-stu-id="e48e0-164">String</span></span>|<span data-ttu-id="e48e0-165">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="e48e0-165">The display name of the attachment.</span></span> <span data-ttu-id="e48e0-166">Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="e48e0-166">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="e48e0-167">size</span><span class="sxs-lookup"><span data-stu-id="e48e0-167">size</span></span>|<span data-ttu-id="e48e0-168">Int32</span><span class="sxs-lookup"><span data-stu-id="e48e0-168">Int32</span></span>|<span data-ttu-id="e48e0-169">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="e48e0-169">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e48e0-170">Отношения</span><span class="sxs-lookup"><span data-stu-id="e48e0-170">Relationships</span></span>
<span data-ttu-id="e48e0-171">Нет</span><span class="sxs-lookup"><span data-stu-id="e48e0-171">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e48e0-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e48e0-172">JSON representation</span></span>

<span data-ttu-id="e48e0-173">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e48e0-173">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/attachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
