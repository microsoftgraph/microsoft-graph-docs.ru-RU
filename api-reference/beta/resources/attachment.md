---
title: Тип ресурса attachment
description: Вы можете добавить связанное содержимое в экземпляр event,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 6c062ac3e832c2ce0385c4851330d5320ca34af9
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849501"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="2f176-103">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="2f176-103">attachment resource type</span></span>

<span data-ttu-id="2f176-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f176-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="2f176-105">Вы можете добавить связанное [message](../resources/message.md)содержимое в [события пользователя, сообщение,](../resources/event.md) [задачу Outlook или](../resources/outlooktask.md)запись в группе [в](../resources/post.md) виде вложения.</span><span class="sxs-lookup"><span data-stu-id="2f176-105">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span> 

<span data-ttu-id="2f176-106">События в календарях группы не поддерживают вложения.</span><span class="sxs-lookup"><span data-stu-id="2f176-106">Events in group calendars do not support attachments.</span></span>

<span data-ttu-id="2f176-107">Задачи Outlook не поддерживают ссылочные вложения.</span><span class="sxs-lookup"><span data-stu-id="2f176-107">Outlook tasks do not support reference attachments.</span></span>

<span data-ttu-id="2f176-108">**attachment** — базовый ресурс для следующих производных типов вложений:</span><span class="sxs-lookup"><span data-stu-id="2f176-108">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="2f176-109">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="2f176-109">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="2f176-110">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="2f176-110">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="2f176-111">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="2f176-111">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

><span data-ttu-id="2f176-112">**Примечание.** Существует ограничение размера файла или вложенного элемента, который можно добавить не более 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="2f176-112">**Note**: There is a limit to the size of the file or item attachment you can add to under 4 MB.</span></span> 
>
> <span data-ttu-id="2f176-113">Но если в сообщение вкладывается файл размером от 3 до 150 МБ, [вы](../api/attachment-createuploadsession.md) можете создать сеанс отправки и итеративно отправлять диапазоны файла, чтобы вложить его.</span><span class="sxs-lookup"><span data-stu-id="2f176-113">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](../api/attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="2f176-114">Пример [см. в разделе, посвященный крупных файлам](/graph/outlook-large-attachments) outlook, вложенные в сообщения Outlook.</span><span class="sxs-lookup"><span data-stu-id="2f176-114">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

## <a name="methods"></a><span data-ttu-id="2f176-115">Методы</span><span class="sxs-lookup"><span data-stu-id="2f176-115">Methods</span></span>

<span data-ttu-id="2f176-116">Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="2f176-116">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="2f176-117">Метод</span><span class="sxs-lookup"><span data-stu-id="2f176-117">Method</span></span>       | <span data-ttu-id="2f176-118">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2f176-118">Return Type</span></span>  |<span data-ttu-id="2f176-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2f176-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f176-120">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="2f176-120">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="2f176-121">attachment</span><span class="sxs-lookup"><span data-stu-id="2f176-121">attachment</span></span>](attachment.md) |<span data-ttu-id="2f176-122">Чтение свойств, связей или необработанного содержимого объекта, которое было вложено к пользовательскому событию, сообщению, задаче Outlook или записи.</span><span class="sxs-lookup"><span data-stu-id="2f176-122">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="2f176-123">Добавление вложения в пользовательское событие</span><span class="sxs-lookup"><span data-stu-id="2f176-123">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="2f176-124">attachment</span><span class="sxs-lookup"><span data-stu-id="2f176-124">attachment</span></span>](attachment.md) |<span data-ttu-id="2f176-125">Добавление файла, элемента или вложения-ссылки в качестве события в пользовательском календаре.</span><span class="sxs-lookup"><span data-stu-id="2f176-125">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="2f176-126">Добавление вложения в сообщение</span><span class="sxs-lookup"><span data-stu-id="2f176-126">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="2f176-127">attachment</span><span class="sxs-lookup"><span data-stu-id="2f176-127">attachment</span></span>](attachment.md) |<span data-ttu-id="2f176-128">Добавление в сообщение файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="2f176-128">Add a file, item, or link attachment to a message.</span></span> <span data-ttu-id="2f176-129">Эта операция ограничивает размер добавляемого вложения в размере не более 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="2f176-129">This operation limits the size of the attachment you can add to under 4 MB.</span></span>|
|[<span data-ttu-id="2f176-130">Создание сеанса для вложения большого файла</span><span class="sxs-lookup"><span data-stu-id="2f176-130">Create session to attach large file</span></span>](../api/attachment-createuploadsession.md)| [<span data-ttu-id="2f176-131">uploadSession</span><span class="sxs-lookup"><span data-stu-id="2f176-131">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="2f176-132">Создать сеанс отправки, позволяющий приложению выполнять итеративную отправку диапазонов файла, например, вложенный файл в указанное **сообщение.**</span><span class="sxs-lookup"><span data-stu-id="2f176-132">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified **message**.</span></span> <span data-ttu-id="2f176-133">Размер файла должен быть от 3 до 150 МБ.</span><span class="sxs-lookup"><span data-stu-id="2f176-133">The file size must be between 3MB and 150MB.</span></span>|
|[<span data-ttu-id="2f176-134">Добавление вложения в задачу Outlook</span><span class="sxs-lookup"><span data-stu-id="2f176-134">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="2f176-135">attachment</span><span class="sxs-lookup"><span data-stu-id="2f176-135">attachment</span></span>](attachment.md) |<span data-ttu-id="2f176-136">Добавление вложенного файла или элемента в задачу Outlook.</span><span class="sxs-lookup"><span data-stu-id="2f176-136">Add a file or item attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="2f176-137">Добавление вложения в запись</span><span class="sxs-lookup"><span data-stu-id="2f176-137">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="2f176-138">attachment</span><span class="sxs-lookup"><span data-stu-id="2f176-138">attachment</span></span>](attachment.md) |<span data-ttu-id="2f176-139">Добавление в запись группы файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="2f176-139">Add a file, item, or link attachment to a group post.</span></span>|
|[<span data-ttu-id="2f176-140">Список вложений пользовательского события</span><span class="sxs-lookup"><span data-stu-id="2f176-140">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="2f176-141">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="2f176-141">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="2f176-142">Получение списка вложений для события в пользовательском календаре.</span><span class="sxs-lookup"><span data-stu-id="2f176-142">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="2f176-143">Список вложений для сообщения</span><span class="sxs-lookup"><span data-stu-id="2f176-143">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="2f176-144">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="2f176-144">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="2f176-145">Получение списка вложений для сообщения.</span><span class="sxs-lookup"><span data-stu-id="2f176-145">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="2f176-146">Список вложений задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="2f176-146">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="2f176-147">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="2f176-147">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="2f176-148">Получение списка вложений для задачи Outlook.</span><span class="sxs-lookup"><span data-stu-id="2f176-148">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="2f176-149">Список вложений для записи</span><span class="sxs-lookup"><span data-stu-id="2f176-149">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="2f176-150">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="2f176-150">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="2f176-151">Получение списка вложений для записи.</span><span class="sxs-lookup"><span data-stu-id="2f176-151">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="2f176-152">Удаление</span><span class="sxs-lookup"><span data-stu-id="2f176-152">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="2f176-153">Нет</span><span class="sxs-lookup"><span data-stu-id="2f176-153">None</span></span> |<span data-ttu-id="2f176-154">Удаление объекта, прикрепка к сообщению, задаче Outlook или записи для события.</span><span class="sxs-lookup"><span data-stu-id="2f176-154">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="2f176-155">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f176-155">Properties</span></span>

<span data-ttu-id="2f176-p104">Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="2f176-p104">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="2f176-158">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f176-158">Property</span></span>     | <span data-ttu-id="2f176-159">Тип</span><span class="sxs-lookup"><span data-stu-id="2f176-159">Type</span></span>   |<span data-ttu-id="2f176-160">Описание</span><span class="sxs-lookup"><span data-stu-id="2f176-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f176-161">contentType</span><span class="sxs-lookup"><span data-stu-id="2f176-161">contentType</span></span>|<span data-ttu-id="2f176-162">String</span><span class="sxs-lookup"><span data-stu-id="2f176-162">String</span></span>|<span data-ttu-id="2f176-163">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="2f176-163">The MIME type.</span></span>|
|<span data-ttu-id="2f176-164">id</span><span class="sxs-lookup"><span data-stu-id="2f176-164">id</span></span>|<span data-ttu-id="2f176-165">String</span><span class="sxs-lookup"><span data-stu-id="2f176-165">String</span></span>| <span data-ttu-id="2f176-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f176-166">Read-only.</span></span>|
|<span data-ttu-id="2f176-167">isInline</span><span class="sxs-lookup"><span data-stu-id="2f176-167">isInline</span></span>|<span data-ttu-id="2f176-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f176-168">Boolean</span></span>|<span data-ttu-id="2f176-169">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="2f176-169">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="2f176-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f176-170">lastModifiedDateTime</span></span>|<span data-ttu-id="2f176-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f176-171">DateTimeOffset</span></span>|<span data-ttu-id="2f176-p105">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2f176-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2f176-174">имя</span><span class="sxs-lookup"><span data-stu-id="2f176-174">name</span></span>|<span data-ttu-id="2f176-175">String</span><span class="sxs-lookup"><span data-stu-id="2f176-175">String</span></span>|<span data-ttu-id="2f176-176">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="2f176-176">The display name of the attachment.</span></span> <span data-ttu-id="2f176-177">Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="2f176-177">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="2f176-178">size</span><span class="sxs-lookup"><span data-stu-id="2f176-178">size</span></span>|<span data-ttu-id="2f176-179">Int32</span><span class="sxs-lookup"><span data-stu-id="2f176-179">Int32</span></span>|<span data-ttu-id="2f176-180">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="2f176-180">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f176-181">Отношения</span><span class="sxs-lookup"><span data-stu-id="2f176-181">Relationships</span></span>
<span data-ttu-id="2f176-182">Нет</span><span class="sxs-lookup"><span data-stu-id="2f176-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f176-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f176-183">JSON representation</span></span>

<span data-ttu-id="2f176-184">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f176-184">Here is a JSON representation of the resource</span></span>

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
