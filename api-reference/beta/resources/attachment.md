---
title: Тип ресурса attachment
description: Вы можете добавить связанное содержимое в экземпляр event,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: a6810ff870124a793bee40ec9df66ae7cb5eabc8
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621661"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="390fd-103">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="390fd-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="390fd-104">Вы можете добавить связанное содержимое для [события](../resources/event.md)пользователя, [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [записи](../resources/post.md) группы в виде вложения.</span><span class="sxs-lookup"><span data-stu-id="390fd-104">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span> 

<span data-ttu-id="390fd-105">События в календарях группы не поддерживают вложения.</span><span class="sxs-lookup"><span data-stu-id="390fd-105">Events in group calendars do not support attachments.</span></span>

<span data-ttu-id="390fd-106">**attachment** — базовый ресурс для следующих производных типов вложений:</span><span class="sxs-lookup"><span data-stu-id="390fd-106">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="390fd-107">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="390fd-107">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="390fd-108">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="390fd-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="390fd-109">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="390fd-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

><span data-ttu-id="390fd-110">**Примечание**. так как в настоящее время общий размер каждого запроса REST составляет 4 МБ, в общем случае это ограничивает размер вложения файла или элемента, который можно добавить в раздел 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="390fd-110">**Note**: Since there is currently a limit of 4MB on the total size of each REST request, in general, this limits the size of the file or item attachment you can add to under 4MB.</span></span> 
>
> <span data-ttu-id="390fd-111">Однако при присоединении к сообщению файла, который находится в диапазоне от 3 МБ и 150MB, вы можете [создать сеанс отправки](../api/attachment-createuploadsession.md) и итеративно отправлять диапазоны файлов, чтобы присоединить их.</span><span class="sxs-lookup"><span data-stu-id="390fd-111">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](../api/attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="390fd-112">В этом примере показано, как [прикрепить большие файлы к сообщениям Outlook](/graph/outlook-large-attachments) .</span><span class="sxs-lookup"><span data-stu-id="390fd-112">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

## <a name="methods"></a><span data-ttu-id="390fd-113">Методы</span><span class="sxs-lookup"><span data-stu-id="390fd-113">Methods</span></span>

<span data-ttu-id="390fd-114">Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="390fd-114">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="390fd-115">Метод</span><span class="sxs-lookup"><span data-stu-id="390fd-115">Method</span></span>       | <span data-ttu-id="390fd-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="390fd-116">Return Type</span></span>  |<span data-ttu-id="390fd-117">Описание</span><span class="sxs-lookup"><span data-stu-id="390fd-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="390fd-118">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="390fd-118">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="390fd-119">attachment</span><span class="sxs-lookup"><span data-stu-id="390fd-119">attachment</span></span>](attachment.md) |<span data-ttu-id="390fd-120">Чтение свойств, связей или необработанного содержимого вложения, вложенного в пользовательское событие, сообщение, задачу Outlook или POST.</span><span class="sxs-lookup"><span data-stu-id="390fd-120">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="390fd-121">Добавление вложения в пользовательское событие</span><span class="sxs-lookup"><span data-stu-id="390fd-121">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="390fd-122">attachment</span><span class="sxs-lookup"><span data-stu-id="390fd-122">attachment</span></span>](attachment.md) |<span data-ttu-id="390fd-123">Добавление файла, элемента или вложения-ссылки в качестве события в пользовательском календаре.</span><span class="sxs-lookup"><span data-stu-id="390fd-123">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="390fd-124">Добавление вложения в сообщение</span><span class="sxs-lookup"><span data-stu-id="390fd-124">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="390fd-125">attachment</span><span class="sxs-lookup"><span data-stu-id="390fd-125">attachment</span></span>](attachment.md) |<span data-ttu-id="390fd-126">Добавление в сообщение файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="390fd-126">Add a file, item, or link attachment to a message.</span></span> <span data-ttu-id="390fd-127">При присоединении файла Размер файла должен быть меньше 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="390fd-127">If attaching a file, the file size must be less than 4MB.</span></span>|
|[<span data-ttu-id="390fd-128">Создание сеанса для присоединения большого файла</span><span class="sxs-lookup"><span data-stu-id="390fd-128">Create session to attach large file</span></span>](../api/attachment-createuploadsession.md)| [<span data-ttu-id="390fd-129">uploadSession</span><span class="sxs-lookup"><span data-stu-id="390fd-129">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="390fd-130">Создайте сеанс отправки, который позволяет приложению итеративно отправлять диапазоны файлов, чтобы прикрепить файл к указанному **сообщению**.</span><span class="sxs-lookup"><span data-stu-id="390fd-130">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified **message**.</span></span> <span data-ttu-id="390fd-131">Размер файла должен быть в пределах 3 МБ и 150MB.</span><span class="sxs-lookup"><span data-stu-id="390fd-131">The file size must be between 3MB and 150MB.</span></span>|
|[<span data-ttu-id="390fd-132">Добавление вложения к задаче Outlook</span><span class="sxs-lookup"><span data-stu-id="390fd-132">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="390fd-133">attachment</span><span class="sxs-lookup"><span data-stu-id="390fd-133">attachment</span></span>](attachment.md) |<span data-ttu-id="390fd-134">Добавление файла, элемента или ссылки на вложение к задаче Outlook.</span><span class="sxs-lookup"><span data-stu-id="390fd-134">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="390fd-135">Добавление вложения в запись</span><span class="sxs-lookup"><span data-stu-id="390fd-135">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="390fd-136">attachment</span><span class="sxs-lookup"><span data-stu-id="390fd-136">attachment</span></span>](attachment.md) |<span data-ttu-id="390fd-137">Добавление в запись файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="390fd-137">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="390fd-138">Список вложений пользовательского события</span><span class="sxs-lookup"><span data-stu-id="390fd-138">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="390fd-139">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="390fd-139">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="390fd-140">Получение списка вложений для события в пользовательском календаре.</span><span class="sxs-lookup"><span data-stu-id="390fd-140">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="390fd-141">Список вложений для сообщения</span><span class="sxs-lookup"><span data-stu-id="390fd-141">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="390fd-142">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="390fd-142">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="390fd-143">Получение списка вложений для сообщения.</span><span class="sxs-lookup"><span data-stu-id="390fd-143">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="390fd-144">Список вложений задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="390fd-144">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="390fd-145">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="390fd-145">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="390fd-146">Получение списка вложений для задачи Outlook.</span><span class="sxs-lookup"><span data-stu-id="390fd-146">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="390fd-147">Список вложений для записи</span><span class="sxs-lookup"><span data-stu-id="390fd-147">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="390fd-148">Коллекция [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="390fd-148">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="390fd-149">Получение списка вложений для записи.</span><span class="sxs-lookup"><span data-stu-id="390fd-149">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="390fd-150">Удаление</span><span class="sxs-lookup"><span data-stu-id="390fd-150">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="390fd-151">Нет</span><span class="sxs-lookup"><span data-stu-id="390fd-151">None</span></span> |<span data-ttu-id="390fd-152">Удаление вложения для события, сообщения, задачи Outlook или POST.</span><span class="sxs-lookup"><span data-stu-id="390fd-152">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="390fd-153">Свойства</span><span class="sxs-lookup"><span data-stu-id="390fd-153">Properties</span></span>

<span data-ttu-id="390fd-p104">Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="390fd-p104">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="390fd-156">Свойство</span><span class="sxs-lookup"><span data-stu-id="390fd-156">Property</span></span>     | <span data-ttu-id="390fd-157">Тип</span><span class="sxs-lookup"><span data-stu-id="390fd-157">Type</span></span>   |<span data-ttu-id="390fd-158">Описание</span><span class="sxs-lookup"><span data-stu-id="390fd-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="390fd-159">contentType</span><span class="sxs-lookup"><span data-stu-id="390fd-159">contentType</span></span>|<span data-ttu-id="390fd-160">String</span><span class="sxs-lookup"><span data-stu-id="390fd-160">String</span></span>|<span data-ttu-id="390fd-161">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="390fd-161">The MIME type.</span></span>|
|<span data-ttu-id="390fd-162">id</span><span class="sxs-lookup"><span data-stu-id="390fd-162">id</span></span>|<span data-ttu-id="390fd-163">Строка</span><span class="sxs-lookup"><span data-stu-id="390fd-163">String</span></span>| <span data-ttu-id="390fd-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="390fd-164">Read-only.</span></span>|
|<span data-ttu-id="390fd-165">isInline</span><span class="sxs-lookup"><span data-stu-id="390fd-165">isInline</span></span>|<span data-ttu-id="390fd-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="390fd-166">Boolean</span></span>|<span data-ttu-id="390fd-167">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="390fd-167">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="390fd-168">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="390fd-168">lastModifiedDateTime</span></span>|<span data-ttu-id="390fd-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="390fd-169">DateTimeOffset</span></span>|<span data-ttu-id="390fd-p105">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="390fd-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="390fd-172">имя</span><span class="sxs-lookup"><span data-stu-id="390fd-172">name</span></span>|<span data-ttu-id="390fd-173">String</span><span class="sxs-lookup"><span data-stu-id="390fd-173">String</span></span>|<span data-ttu-id="390fd-174">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="390fd-174">The display name of the attachment.</span></span> <span data-ttu-id="390fd-175">Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="390fd-175">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="390fd-176">size</span><span class="sxs-lookup"><span data-stu-id="390fd-176">size</span></span>|<span data-ttu-id="390fd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="390fd-177">Int32</span></span>|<span data-ttu-id="390fd-178">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="390fd-178">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="390fd-179">Отношения</span><span class="sxs-lookup"><span data-stu-id="390fd-179">Relationships</span></span>
<span data-ttu-id="390fd-180">Нет</span><span class="sxs-lookup"><span data-stu-id="390fd-180">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="390fd-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="390fd-181">JSON representation</span></span>

<span data-ttu-id="390fd-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="390fd-182">Here is a JSON representation of the resource</span></span>

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
