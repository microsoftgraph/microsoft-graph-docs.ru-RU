---
title: Тип ресурса attachment
description: Вы можете добавить связанное содержимое в экземпляр event,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: d1296c40bfc434262f1911c6f9453725bc033999
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137622"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="f93cc-103">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="f93cc-103">attachment resource type</span></span>

<span data-ttu-id="f93cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f93cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="f93cc-105">Вы можете добавить связанное содержимое к событию [пользователя,](../resources/event.md) [сообщению,](../resources/message.md)задаче [Outlook](../resources/outlooktask.md)или [записи](../resources/post.md) группы в форме вложения.</span><span class="sxs-lookup"><span data-stu-id="f93cc-105">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span> 

<span data-ttu-id="f93cc-106">События в календарях группы не поддерживают вложения.</span><span class="sxs-lookup"><span data-stu-id="f93cc-106">Events in group calendars do not support attachments.</span></span>

<span data-ttu-id="f93cc-107">Задачи Outlook не поддерживают справочные вложения.</span><span class="sxs-lookup"><span data-stu-id="f93cc-107">Outlook tasks do not support reference attachments.</span></span>

<span data-ttu-id="f93cc-108">**attachment** — базовый ресурс для следующих производных типов вложений:</span><span class="sxs-lookup"><span data-stu-id="f93cc-108">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="f93cc-109">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="f93cc-109">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="f93cc-110">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="f93cc-110">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="f93cc-111">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f93cc-111">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

><span data-ttu-id="f93cc-112">**Примечание.** Размер вложенного файла или элемента не может быть меньше 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="f93cc-112">**Note**: There is a limit to the size of the file or item attachment you can add to under 4 MB.</span></span> 
>
> <span data-ttu-id="f93cc-113">Однако при вложении в сообщение файла размером от 3 МБ до [](../api/attachment-createuploadsession.md) 150 МБ можно создать сеанс отправки и итеративно отправить диапазоны файла для его вложения.</span><span class="sxs-lookup"><span data-stu-id="f93cc-113">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](../api/attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="f93cc-114">См. [пример вложенных больших файлов в](/graph/outlook-large-attachments) сообщения Outlook.</span><span class="sxs-lookup"><span data-stu-id="f93cc-114">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

## <a name="methods"></a><span data-ttu-id="f93cc-115">Методы</span><span class="sxs-lookup"><span data-stu-id="f93cc-115">Methods</span></span>

<span data-ttu-id="f93cc-116">Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="f93cc-116">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="f93cc-117">Метод</span><span class="sxs-lookup"><span data-stu-id="f93cc-117">Method</span></span>       | <span data-ttu-id="f93cc-118">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f93cc-118">Return Type</span></span>  |<span data-ttu-id="f93cc-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f93cc-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f93cc-120">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="f93cc-120">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="f93cc-121">attachment</span><span class="sxs-lookup"><span data-stu-id="f93cc-121">attachment</span></span>](attachment.md) |<span data-ttu-id="f93cc-122">Чтение свойств, связей или необработанных содержимого вложения, вложенного в событие пользователя, сообщение, задачу Outlook или публикацию.</span><span class="sxs-lookup"><span data-stu-id="f93cc-122">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="f93cc-123">Добавление вложения в пользовательское событие</span><span class="sxs-lookup"><span data-stu-id="f93cc-123">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="f93cc-124">attachment</span><span class="sxs-lookup"><span data-stu-id="f93cc-124">attachment</span></span>](attachment.md) |<span data-ttu-id="f93cc-125">Добавление файла, элемента или вложения-ссылки в качестве события в пользовательском календаре.</span><span class="sxs-lookup"><span data-stu-id="f93cc-125">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="f93cc-126">Добавление вложения в сообщение</span><span class="sxs-lookup"><span data-stu-id="f93cc-126">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="f93cc-127">attachment</span><span class="sxs-lookup"><span data-stu-id="f93cc-127">attachment</span></span>](attachment.md) |<span data-ttu-id="f93cc-128">Добавление в сообщение файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="f93cc-128">Add a file, item, or link attachment to a message.</span></span> <span data-ttu-id="f93cc-129">Эта операция ограничивает размер вложения, который можно добавить, до 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="f93cc-129">This operation limits the size of the attachment you can add to under 4 MB.</span></span>|
|[<span data-ttu-id="f93cc-130">Создание сеанса для вложения большого файла</span><span class="sxs-lookup"><span data-stu-id="f93cc-130">Create session to attach large file</span></span>](../api/attachment-createuploadsession.md)| [<span data-ttu-id="f93cc-131">uploadSession</span><span class="sxs-lookup"><span data-stu-id="f93cc-131">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="f93cc-132">Создайте сеанс отправки, который позволяет приложению итеративно отправлять диапазоны файла, чтобы встроить файл в указанное **сообщение.**</span><span class="sxs-lookup"><span data-stu-id="f93cc-132">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified **message**.</span></span> <span data-ttu-id="f93cc-133">Размер файла должен быть от 3 до 150 МБ.</span><span class="sxs-lookup"><span data-stu-id="f93cc-133">The file size must be between 3MB and 150MB.</span></span>|
|<span data-ttu-id="f93cc-134">[Добавление вложения в задачу Outlook](../api/outlooktask-post-attachments.md) (неподготовлено)</span><span class="sxs-lookup"><span data-stu-id="f93cc-134">[Add attachment to an Outlook task](../api/outlooktask-post-attachments.md) (deprecated)</span></span> | [<span data-ttu-id="f93cc-135">attachment</span><span class="sxs-lookup"><span data-stu-id="f93cc-135">attachment</span></span>](attachment.md) |<span data-ttu-id="f93cc-136">Добавление вложенного файла или элемента в задачу Outlook.</span><span class="sxs-lookup"><span data-stu-id="f93cc-136">Add a file or item attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="f93cc-137">Добавление вложения в запись</span><span class="sxs-lookup"><span data-stu-id="f93cc-137">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="f93cc-138">attachment</span><span class="sxs-lookup"><span data-stu-id="f93cc-138">attachment</span></span>](attachment.md) |<span data-ttu-id="f93cc-139">Добавление вложенного файла, элемента или ссылки в публикацию группы.</span><span class="sxs-lookup"><span data-stu-id="f93cc-139">Add a file, item, or link attachment to a group post.</span></span>|
|[<span data-ttu-id="f93cc-140">Список вложений пользовательского события</span><span class="sxs-lookup"><span data-stu-id="f93cc-140">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="f93cc-141">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="f93cc-141">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="f93cc-142">Получение списка вложений для события в пользовательском календаре.</span><span class="sxs-lookup"><span data-stu-id="f93cc-142">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="f93cc-143">Список вложений для сообщения</span><span class="sxs-lookup"><span data-stu-id="f93cc-143">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="f93cc-144">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="f93cc-144">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="f93cc-145">Получение списка вложений для сообщения.</span><span class="sxs-lookup"><span data-stu-id="f93cc-145">Get a list of attachments for a message.</span></span> |
|<span data-ttu-id="f93cc-146">[Список вложений задачи Outlook](../api/outlooktask-list-attachments.md) (неподготовлен)</span><span class="sxs-lookup"><span data-stu-id="f93cc-146">[List attachments of an Outlook task](../api/outlooktask-list-attachments.md) (deprecated)</span></span> | <span data-ttu-id="f93cc-147">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="f93cc-147">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="f93cc-148">Получите список вложений для задачи Outlook.</span><span class="sxs-lookup"><span data-stu-id="f93cc-148">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="f93cc-149">Список вложений для записи</span><span class="sxs-lookup"><span data-stu-id="f93cc-149">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="f93cc-150">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="f93cc-150">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="f93cc-151">Получение списка вложений для записи.</span><span class="sxs-lookup"><span data-stu-id="f93cc-151">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="f93cc-152">Удаление</span><span class="sxs-lookup"><span data-stu-id="f93cc-152">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="f93cc-153">Нет</span><span class="sxs-lookup"><span data-stu-id="f93cc-153">None</span></span> |<span data-ttu-id="f93cc-154">Удаление вложения для события, сообщения, задачи Outlook или публикации.</span><span class="sxs-lookup"><span data-stu-id="f93cc-154">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="f93cc-155">Свойства</span><span class="sxs-lookup"><span data-stu-id="f93cc-155">Properties</span></span>

<span data-ttu-id="f93cc-p104">Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f93cc-p104">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="f93cc-158">Свойство</span><span class="sxs-lookup"><span data-stu-id="f93cc-158">Property</span></span>     | <span data-ttu-id="f93cc-159">Тип</span><span class="sxs-lookup"><span data-stu-id="f93cc-159">Type</span></span>   |<span data-ttu-id="f93cc-160">Описание</span><span class="sxs-lookup"><span data-stu-id="f93cc-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f93cc-161">contentType</span><span class="sxs-lookup"><span data-stu-id="f93cc-161">contentType</span></span>|<span data-ttu-id="f93cc-162">String</span><span class="sxs-lookup"><span data-stu-id="f93cc-162">String</span></span>|<span data-ttu-id="f93cc-163">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="f93cc-163">The MIME type.</span></span>|
|<span data-ttu-id="f93cc-164">id</span><span class="sxs-lookup"><span data-stu-id="f93cc-164">id</span></span>|<span data-ttu-id="f93cc-165">String</span><span class="sxs-lookup"><span data-stu-id="f93cc-165">String</span></span>| <span data-ttu-id="f93cc-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f93cc-166">Read-only.</span></span>|
|<span data-ttu-id="f93cc-167">isInline</span><span class="sxs-lookup"><span data-stu-id="f93cc-167">isInline</span></span>|<span data-ttu-id="f93cc-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="f93cc-168">Boolean</span></span>|<span data-ttu-id="f93cc-169">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="f93cc-169">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="f93cc-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f93cc-170">lastModifiedDateTime</span></span>|<span data-ttu-id="f93cc-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f93cc-171">DateTimeOffset</span></span>|<span data-ttu-id="f93cc-p105">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f93cc-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f93cc-174">имя</span><span class="sxs-lookup"><span data-stu-id="f93cc-174">name</span></span>|<span data-ttu-id="f93cc-175">String</span><span class="sxs-lookup"><span data-stu-id="f93cc-175">String</span></span>|<span data-ttu-id="f93cc-176">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="f93cc-176">The display name of the attachment.</span></span> <span data-ttu-id="f93cc-177">Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="f93cc-177">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="f93cc-178">size</span><span class="sxs-lookup"><span data-stu-id="f93cc-178">size</span></span>|<span data-ttu-id="f93cc-179">Int32</span><span class="sxs-lookup"><span data-stu-id="f93cc-179">Int32</span></span>|<span data-ttu-id="f93cc-180">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="f93cc-180">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f93cc-181">Отношения</span><span class="sxs-lookup"><span data-stu-id="f93cc-181">Relationships</span></span>
<span data-ttu-id="f93cc-182">Нет</span><span class="sxs-lookup"><span data-stu-id="f93cc-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f93cc-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f93cc-183">JSON representation</span></span>

<span data-ttu-id="f93cc-184">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f93cc-184">Here is a JSON representation of the resource</span></span>

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


