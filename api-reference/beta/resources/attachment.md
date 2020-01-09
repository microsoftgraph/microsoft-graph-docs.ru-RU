---
title: Тип ресурса attachment
description: Вы можете добавить связанное содержимое в экземпляр event,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 0c0f257a9bdcf6c149b4f6374e2011cebb437603
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994966"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="aad18-103">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="aad18-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aad18-104">Вы можете добавить связанное содержимое для [события](../resources/event.md)пользователя, [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [записи](../resources/post.md) группы в виде вложения.</span><span class="sxs-lookup"><span data-stu-id="aad18-104">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span> 

<span data-ttu-id="aad18-105">События в календарях группы не поддерживают вложения.</span><span class="sxs-lookup"><span data-stu-id="aad18-105">Events in group calendars do not support attachments.</span></span>

<span data-ttu-id="aad18-106">Задачи Outlook не поддерживают справочные вложения.</span><span class="sxs-lookup"><span data-stu-id="aad18-106">Outlook tasks do not support reference attachments.</span></span>

<span data-ttu-id="aad18-107">**attachment** — базовый ресурс для следующих производных типов вложений:</span><span class="sxs-lookup"><span data-stu-id="aad18-107">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="aad18-108">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="aad18-108">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="aad18-109">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="aad18-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="aad18-110">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="aad18-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

><span data-ttu-id="aad18-111">**Note**: ограничен размер вложения файла или элемента, который можно добавить в пределах 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="aad18-111">**Note**: There is a limit to the size of the file or item attachment you can add to under 4 MB.</span></span> 
>
> <span data-ttu-id="aad18-112">Однако при присоединении к сообщению файла, который находится в диапазоне от 3 МБ и 150MB, вы можете [создать сеанс отправки](../api/attachment-createuploadsession.md) и итеративно отправлять диапазоны файлов, чтобы присоединить их.</span><span class="sxs-lookup"><span data-stu-id="aad18-112">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](../api/attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="aad18-113">В этом примере показано, как [прикрепить большие файлы к сообщениям Outlook](/graph/outlook-large-attachments) .</span><span class="sxs-lookup"><span data-stu-id="aad18-113">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

## <a name="methods"></a><span data-ttu-id="aad18-114">Методы</span><span class="sxs-lookup"><span data-stu-id="aad18-114">Methods</span></span>

<span data-ttu-id="aad18-115">Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="aad18-115">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="aad18-116">Метод</span><span class="sxs-lookup"><span data-stu-id="aad18-116">Method</span></span>       | <span data-ttu-id="aad18-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aad18-117">Return Type</span></span>  |<span data-ttu-id="aad18-118">Описание</span><span class="sxs-lookup"><span data-stu-id="aad18-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aad18-119">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="aad18-119">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="aad18-120">attachment</span><span class="sxs-lookup"><span data-stu-id="aad18-120">attachment</span></span>](attachment.md) |<span data-ttu-id="aad18-121">Чтение свойств, связей или необработанного содержимого вложения, вложенного в пользовательское событие, сообщение, задачу Outlook или POST.</span><span class="sxs-lookup"><span data-stu-id="aad18-121">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="aad18-122">Добавление вложения в пользовательское событие</span><span class="sxs-lookup"><span data-stu-id="aad18-122">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="aad18-123">attachment</span><span class="sxs-lookup"><span data-stu-id="aad18-123">attachment</span></span>](attachment.md) |<span data-ttu-id="aad18-124">Добавление файла, элемента или вложения-ссылки в качестве события в пользовательском календаре.</span><span class="sxs-lookup"><span data-stu-id="aad18-124">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="aad18-125">Добавление вложения в сообщение</span><span class="sxs-lookup"><span data-stu-id="aad18-125">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="aad18-126">attachment</span><span class="sxs-lookup"><span data-stu-id="aad18-126">attachment</span></span>](attachment.md) |<span data-ttu-id="aad18-127">Добавление в сообщение файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="aad18-127">Add a file, item, or link attachment to a message.</span></span> <span data-ttu-id="aad18-128">Эта операция ограничит размер вложения, которое можно добавить в течение 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="aad18-128">This operation limits the size of the attachment you can add to under 4 MB.</span></span>|
|[<span data-ttu-id="aad18-129">Создание сеанса для присоединения большого файла</span><span class="sxs-lookup"><span data-stu-id="aad18-129">Create session to attach large file</span></span>](../api/attachment-createuploadsession.md)| [<span data-ttu-id="aad18-130">uploadSession</span><span class="sxs-lookup"><span data-stu-id="aad18-130">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="aad18-131">Создайте сеанс отправки, который позволяет приложению итеративно отправлять диапазоны файлов, чтобы прикрепить файл к указанному **сообщению**.</span><span class="sxs-lookup"><span data-stu-id="aad18-131">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified **message**.</span></span> <span data-ttu-id="aad18-132">Размер файла должен быть в пределах 3 МБ и 150MB.</span><span class="sxs-lookup"><span data-stu-id="aad18-132">The file size must be between 3MB and 150MB.</span></span>|
|[<span data-ttu-id="aad18-133">Добавление вложения к задаче Outlook</span><span class="sxs-lookup"><span data-stu-id="aad18-133">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="aad18-134">attachment</span><span class="sxs-lookup"><span data-stu-id="aad18-134">attachment</span></span>](attachment.md) |<span data-ttu-id="aad18-135">Добавление вложенного файла или элемента к задаче Outlook.</span><span class="sxs-lookup"><span data-stu-id="aad18-135">Add a file or item attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="aad18-136">Добавление вложения в запись</span><span class="sxs-lookup"><span data-stu-id="aad18-136">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="aad18-137">attachment</span><span class="sxs-lookup"><span data-stu-id="aad18-137">attachment</span></span>](attachment.md) |<span data-ttu-id="aad18-138">Добавление файла, элемента или ссылки на вложение в группу POST.</span><span class="sxs-lookup"><span data-stu-id="aad18-138">Add a file, item, or link attachment to a group post.</span></span>|
|[<span data-ttu-id="aad18-139">Список вложений пользовательского события</span><span class="sxs-lookup"><span data-stu-id="aad18-139">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="aad18-140">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="aad18-140">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="aad18-141">Получение списка вложений для события в пользовательском календаре.</span><span class="sxs-lookup"><span data-stu-id="aad18-141">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="aad18-142">Список вложений для сообщения</span><span class="sxs-lookup"><span data-stu-id="aad18-142">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="aad18-143">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="aad18-143">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="aad18-144">Получение списка вложений для сообщения.</span><span class="sxs-lookup"><span data-stu-id="aad18-144">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="aad18-145">Список вложений задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="aad18-145">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="aad18-146">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="aad18-146">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="aad18-147">Получение списка вложений для задачи Outlook.</span><span class="sxs-lookup"><span data-stu-id="aad18-147">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="aad18-148">Список вложений для записи</span><span class="sxs-lookup"><span data-stu-id="aad18-148">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="aad18-149">Коллекция [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="aad18-149">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="aad18-150">Получение списка вложений для записи.</span><span class="sxs-lookup"><span data-stu-id="aad18-150">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="aad18-151">Удаление</span><span class="sxs-lookup"><span data-stu-id="aad18-151">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="aad18-152">Нет</span><span class="sxs-lookup"><span data-stu-id="aad18-152">None</span></span> |<span data-ttu-id="aad18-153">Удаление вложения для события, сообщения, задачи Outlook или POST.</span><span class="sxs-lookup"><span data-stu-id="aad18-153">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="aad18-154">Свойства</span><span class="sxs-lookup"><span data-stu-id="aad18-154">Properties</span></span>

<span data-ttu-id="aad18-p104">Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="aad18-p104">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="aad18-157">Свойство</span><span class="sxs-lookup"><span data-stu-id="aad18-157">Property</span></span>     | <span data-ttu-id="aad18-158">Тип</span><span class="sxs-lookup"><span data-stu-id="aad18-158">Type</span></span>   |<span data-ttu-id="aad18-159">Описание</span><span class="sxs-lookup"><span data-stu-id="aad18-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aad18-160">contentType</span><span class="sxs-lookup"><span data-stu-id="aad18-160">contentType</span></span>|<span data-ttu-id="aad18-161">String</span><span class="sxs-lookup"><span data-stu-id="aad18-161">String</span></span>|<span data-ttu-id="aad18-162">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="aad18-162">The MIME type.</span></span>|
|<span data-ttu-id="aad18-163">id</span><span class="sxs-lookup"><span data-stu-id="aad18-163">id</span></span>|<span data-ttu-id="aad18-164">Строка</span><span class="sxs-lookup"><span data-stu-id="aad18-164">String</span></span>| <span data-ttu-id="aad18-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aad18-165">Read-only.</span></span>|
|<span data-ttu-id="aad18-166">isInline</span><span class="sxs-lookup"><span data-stu-id="aad18-166">isInline</span></span>|<span data-ttu-id="aad18-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad18-167">Boolean</span></span>|<span data-ttu-id="aad18-168">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="aad18-168">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="aad18-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aad18-169">lastModifiedDateTime</span></span>|<span data-ttu-id="aad18-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aad18-170">DateTimeOffset</span></span>|<span data-ttu-id="aad18-p105">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aad18-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="aad18-173">имя</span><span class="sxs-lookup"><span data-stu-id="aad18-173">name</span></span>|<span data-ttu-id="aad18-174">String</span><span class="sxs-lookup"><span data-stu-id="aad18-174">String</span></span>|<span data-ttu-id="aad18-175">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="aad18-175">The display name of the attachment.</span></span> <span data-ttu-id="aad18-176">Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="aad18-176">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="aad18-177">size</span><span class="sxs-lookup"><span data-stu-id="aad18-177">size</span></span>|<span data-ttu-id="aad18-178">Int32</span><span class="sxs-lookup"><span data-stu-id="aad18-178">Int32</span></span>|<span data-ttu-id="aad18-179">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="aad18-179">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aad18-180">Отношения</span><span class="sxs-lookup"><span data-stu-id="aad18-180">Relationships</span></span>
<span data-ttu-id="aad18-181">Нет</span><span class="sxs-lookup"><span data-stu-id="aad18-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aad18-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aad18-182">JSON representation</span></span>

<span data-ttu-id="aad18-183">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aad18-183">Here is a JSON representation of the resource</span></span>

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
