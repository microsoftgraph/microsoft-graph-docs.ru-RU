# <a name="referenceattachment-resource-type"></a><span data-ttu-id="4460f-101">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="4460f-101">referenceAttachment resource type</span></span>

<span data-ttu-id="4460f-102">Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.</span><span class="sxs-lookup"><span data-stu-id="4460f-102">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="4460f-103">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="4460f-103">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4460f-104">Методы</span><span class="sxs-lookup"><span data-stu-id="4460f-104">Methods</span></span>

| <span data-ttu-id="4460f-105">Метод</span><span class="sxs-lookup"><span data-stu-id="4460f-105">Method</span></span>       | <span data-ttu-id="4460f-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4460f-106">Return Type</span></span>  |<span data-ttu-id="4460f-107">Описание</span><span class="sxs-lookup"><span data-stu-id="4460f-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4460f-108">Get</span><span class="sxs-lookup"><span data-stu-id="4460f-108">Get</span></span>](../api/attachment_get.md) | [<span data-ttu-id="4460f-109">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="4460f-109">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="4460f-110">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="4460f-110">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="4460f-111">Delete</span><span class="sxs-lookup"><span data-stu-id="4460f-111">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="4460f-112">Нет</span><span class="sxs-lookup"><span data-stu-id="4460f-112">None</span></span> |<span data-ttu-id="4460f-113">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="4460f-113">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4460f-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="4460f-114">Properties</span></span>
| <span data-ttu-id="4460f-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="4460f-115">Property</span></span>     | <span data-ttu-id="4460f-116">Тип</span><span class="sxs-lookup"><span data-stu-id="4460f-116">Type</span></span>   |<span data-ttu-id="4460f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="4460f-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4460f-118">contentType</span><span class="sxs-lookup"><span data-stu-id="4460f-118">contentType</span></span>|<span data-ttu-id="4460f-119">String</span><span class="sxs-lookup"><span data-stu-id="4460f-119">String</span></span>|<span data-ttu-id="4460f-120">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="4460f-120">The content type of the attachment.</span></span>|
|<span data-ttu-id="4460f-121">id</span><span class="sxs-lookup"><span data-stu-id="4460f-121">id</span></span>|<span data-ttu-id="4460f-122">String</span><span class="sxs-lookup"><span data-stu-id="4460f-122">String</span></span>|<span data-ttu-id="4460f-p101">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4460f-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="4460f-125">isInline</span><span class="sxs-lookup"><span data-stu-id="4460f-125">isInline</span></span>|<span data-ttu-id="4460f-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="4460f-126">Boolean</span></span>|<span data-ttu-id="4460f-127">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="4460f-127">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="4460f-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4460f-128">lastModifiedDateTime</span></span>|<span data-ttu-id="4460f-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4460f-129">DateTimeOffset</span></span>|<span data-ttu-id="4460f-p102">Дата и время последнего изменения вложения. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4460f-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4460f-133">имя</span><span class="sxs-lookup"><span data-stu-id="4460f-133">name</span></span>|<span data-ttu-id="4460f-134">String</span><span class="sxs-lookup"><span data-stu-id="4460f-134">String</span></span>|<span data-ttu-id="4460f-p103">Текст, который отображается под значком, представляет внедренное вложение. Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="4460f-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="4460f-137">size</span><span class="sxs-lookup"><span data-stu-id="4460f-137">size</span></span>|<span data-ttu-id="4460f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="4460f-138">Int32</span></span>|<span data-ttu-id="4460f-139">Объем метаданных, которые хранятся в сообщении с вложением (в байтах).</span><span class="sxs-lookup"><span data-stu-id="4460f-139">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="4460f-140">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="4460f-140">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4460f-141">Связи</span><span class="sxs-lookup"><span data-stu-id="4460f-141">Relationships</span></span>
<span data-ttu-id="4460f-142">Нет</span><span class="sxs-lookup"><span data-stu-id="4460f-142">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="4460f-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4460f-143">JSON representation</span></span>

<span data-ttu-id="4460f-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4460f-144">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
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
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
