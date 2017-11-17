# <a name="attachment-resource-type"></a><span data-ttu-id="d05f9-101">Тип ресурса attachment</span><span class="sxs-lookup"><span data-stu-id="d05f9-101">attachment resource type</span></span>

<span data-ttu-id="d05f9-102">Вы можете добавить связанное содержимое в экземпляр [event](../resources/event.md), [message](../resources/message.md) или [post](../resources/post.md) в форме вложения.</span><span class="sxs-lookup"><span data-stu-id="d05f9-102">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="d05f9-103">**attachment** — базовый ресурс для следующих производных типов вложений:</span><span class="sxs-lookup"><span data-stu-id="d05f9-103">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="d05f9-104">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="d05f9-104">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="d05f9-105">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="d05f9-105">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="d05f9-106">ссылка на файл (ресурс [referenceAttachment](../resources/referenceAttachment.md)).</span><span class="sxs-lookup"><span data-stu-id="d05f9-106">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource)</span></span>


## <a name="methods"></a><span data-ttu-id="d05f9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d05f9-107">Methods</span></span>

<span data-ttu-id="d05f9-108">Указанные ниже методы применяются к любому из производных типов вложений (**fileAttachment**, **itemAttachment** или **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="d05f9-108">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="d05f9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d05f9-109">Method</span></span>       | <span data-ttu-id="d05f9-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d05f9-110">Return Type</span></span>  |<span data-ttu-id="d05f9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d05f9-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d05f9-112">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="d05f9-112">Get attachment</span></span>](../api/attachment_get.md) | [<span data-ttu-id="d05f9-113">attachment</span><span class="sxs-lookup"><span data-stu-id="d05f9-113">attachment</span></span>](attachment.md) |<span data-ttu-id="d05f9-114">Чтение свойств и связей объекта, представляющего вложение, которое было добавлено к сообщению, записи или данным о событии.</span><span class="sxs-lookup"><span data-stu-id="d05f9-114">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="d05f9-115">Добавление вложения к данным о событии</span><span class="sxs-lookup"><span data-stu-id="d05f9-115">Add attachment to an event</span></span>](../api/event_post_attachments.md) | [<span data-ttu-id="d05f9-116">attachment</span><span class="sxs-lookup"><span data-stu-id="d05f9-116">attachment</span></span>](attachment.md) |<span data-ttu-id="d05f9-117">Добавление для события файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="d05f9-117">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="d05f9-118">Добавление вложения в сообщение</span><span class="sxs-lookup"><span data-stu-id="d05f9-118">Add attachment to a message</span></span>](../api/message_post_attachments.md) | [<span data-ttu-id="d05f9-119">attachment</span><span class="sxs-lookup"><span data-stu-id="d05f9-119">attachment</span></span>](attachment.md) |<span data-ttu-id="d05f9-120">Добавление в сообщение файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="d05f9-120">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="d05f9-121">Добавление вложения в запись</span><span class="sxs-lookup"><span data-stu-id="d05f9-121">Add attachment to a post</span></span>](../api/post_post_attachments.md) | [<span data-ttu-id="d05f9-122">attachment</span><span class="sxs-lookup"><span data-stu-id="d05f9-122">attachment</span></span>](attachment.md) |<span data-ttu-id="d05f9-123">Добавление в запись файла, элемента или ссылки в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="d05f9-123">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="d05f9-124">Список вложений для события</span><span class="sxs-lookup"><span data-stu-id="d05f9-124">List attachments of an event</span></span>](../api/event_list_attachments.md) | <span data-ttu-id="d05f9-125">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="d05f9-125">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="d05f9-126">Получение списка вложений для события.</span><span class="sxs-lookup"><span data-stu-id="d05f9-126">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="d05f9-127">Список вложений для сообщения</span><span class="sxs-lookup"><span data-stu-id="d05f9-127">List attachments of a message</span></span>](../api/message_list_attachments.md) | <span data-ttu-id="d05f9-128">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="d05f9-128">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="d05f9-129">Получение списка вложений для сообщения.</span><span class="sxs-lookup"><span data-stu-id="d05f9-129">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="d05f9-130">Список вложений для записи</span><span class="sxs-lookup"><span data-stu-id="d05f9-130">List attachments of a post</span></span>](../api/post_list_attachments.md) | <span data-ttu-id="d05f9-131">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="d05f9-131">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="d05f9-132">Получение списка вложений для записи.</span><span class="sxs-lookup"><span data-stu-id="d05f9-132">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="d05f9-133">Удаление</span><span class="sxs-lookup"><span data-stu-id="d05f9-133">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="d05f9-134">Нет</span><span class="sxs-lookup"><span data-stu-id="d05f9-134">None</span></span> |<span data-ttu-id="d05f9-135">Удаление объекта, представляющего вложение, которое было добавлено к сообщению, записи или данным о событии.</span><span class="sxs-lookup"><span data-stu-id="d05f9-135">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="d05f9-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="d05f9-136">Properties</span></span>

<span data-ttu-id="d05f9-p101">Ниже перечислены базовые свойства любого ресурса attachment. Чтобы просмотреть дополнительные свойства, откройте статью о конкретном типе вложения ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceAttachment.md)).</span><span class="sxs-lookup"><span data-stu-id="d05f9-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceAttachment.md)) for additional properties.</span></span>

| <span data-ttu-id="d05f9-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="d05f9-139">Property</span></span>     | <span data-ttu-id="d05f9-140">Тип</span><span class="sxs-lookup"><span data-stu-id="d05f9-140">Type</span></span>   |<span data-ttu-id="d05f9-141">Описание</span><span class="sxs-lookup"><span data-stu-id="d05f9-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d05f9-142">contentType</span><span class="sxs-lookup"><span data-stu-id="d05f9-142">contentType</span></span>|<span data-ttu-id="d05f9-143">String</span><span class="sxs-lookup"><span data-stu-id="d05f9-143">String</span></span>|<span data-ttu-id="d05f9-144">Тип MIME.</span><span class="sxs-lookup"><span data-stu-id="d05f9-144">The MIME type.</span></span>|
|<span data-ttu-id="d05f9-145">id</span><span class="sxs-lookup"><span data-stu-id="d05f9-145">id</span></span>|<span data-ttu-id="d05f9-146">String</span><span class="sxs-lookup"><span data-stu-id="d05f9-146">String</span></span>| <span data-ttu-id="d05f9-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d05f9-147">Read-only.</span></span>|
|<span data-ttu-id="d05f9-148">isInline</span><span class="sxs-lookup"><span data-stu-id="d05f9-148">isInline</span></span>|<span data-ttu-id="d05f9-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="d05f9-149">Boolean</span></span>|<span data-ttu-id="d05f9-150">Значение `true`, если вложение является встроенным. В противном случае — значение `false`.</span><span class="sxs-lookup"><span data-stu-id="d05f9-150">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="d05f9-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d05f9-151">lastModifiedDateTime</span></span>|<span data-ttu-id="d05f9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d05f9-152">DateTimeOffset</span></span>|<span data-ttu-id="d05f9-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d05f9-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d05f9-155">имя</span><span class="sxs-lookup"><span data-stu-id="d05f9-155">name</span></span>|<span data-ttu-id="d05f9-156">String</span><span class="sxs-lookup"><span data-stu-id="d05f9-156">String</span></span>|<span data-ttu-id="d05f9-157">Имя вложенного файла.</span><span class="sxs-lookup"><span data-stu-id="d05f9-157">The attachment's file name.</span></span>|
|<span data-ttu-id="d05f9-158">size</span><span class="sxs-lookup"><span data-stu-id="d05f9-158">size</span></span>|<span data-ttu-id="d05f9-159">Int32</span><span class="sxs-lookup"><span data-stu-id="d05f9-159">Int32</span></span>|<span data-ttu-id="d05f9-160">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="d05f9-160">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d05f9-161">Отношения</span><span class="sxs-lookup"><span data-stu-id="d05f9-161">Relationships</span></span>
<span data-ttu-id="d05f9-162">Нет</span><span class="sxs-lookup"><span data-stu-id="d05f9-162">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d05f9-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d05f9-163">JSON representation</span></span>

<span data-ttu-id="d05f9-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d05f9-164">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
