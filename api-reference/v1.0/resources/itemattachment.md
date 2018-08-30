# <a name="itemattachment-resource-type"></a><span data-ttu-id="960c3-101">Тип ресурса itemAttachment</span><span class="sxs-lookup"><span data-stu-id="960c3-101">itemAttachment resource type</span></span>

<span data-ttu-id="960c3-102">Контакт, событие или сообщение, вложенное в другое событие, сообщение или публикацию.</span><span class="sxs-lookup"><span data-stu-id="960c3-102">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="960c3-103">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="960c3-103">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="960c3-104">Методы</span><span class="sxs-lookup"><span data-stu-id="960c3-104">Methods</span></span>

| <span data-ttu-id="960c3-105">Метод</span><span class="sxs-lookup"><span data-stu-id="960c3-105">Method</span></span>       | <span data-ttu-id="960c3-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="960c3-106">Return Type</span></span>  |<span data-ttu-id="960c3-107">Описание</span><span class="sxs-lookup"><span data-stu-id="960c3-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="960c3-108">Get</span><span class="sxs-lookup"><span data-stu-id="960c3-108">Get</span></span>](../api/attachment_get.md) | <span data-ttu-id="960c3-109">[itemAttachment](itemattachment.md)</span><span class="sxs-lookup"><span data-stu-id="960c3-109">[itemAttachment](itemattachment.md),</span></span> |<span data-ttu-id="960c3-110">Чтение свойств и связей объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="960c3-110">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="960c3-111">Delete</span><span class="sxs-lookup"><span data-stu-id="960c3-111">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="960c3-112">Нет</span><span class="sxs-lookup"><span data-stu-id="960c3-112">None</span></span> |<span data-ttu-id="960c3-113">Удаление объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="960c3-113">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="960c3-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="960c3-114">Properties</span></span>
| <span data-ttu-id="960c3-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="960c3-115">Property</span></span>     | <span data-ttu-id="960c3-116">Тип</span><span class="sxs-lookup"><span data-stu-id="960c3-116">Type</span></span>   |<span data-ttu-id="960c3-117">Описание</span><span class="sxs-lookup"><span data-stu-id="960c3-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="960c3-118">contentType</span><span class="sxs-lookup"><span data-stu-id="960c3-118">contentType</span></span>|<span data-ttu-id="960c3-119">Строка</span><span class="sxs-lookup"><span data-stu-id="960c3-119">String</span></span>|<span data-ttu-id="960c3-120">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="960c3-120">The content type of the attachment.</span></span>|
|<span data-ttu-id="960c3-121">id</span><span class="sxs-lookup"><span data-stu-id="960c3-121">id</span></span>|<span data-ttu-id="960c3-122">Строка</span><span class="sxs-lookup"><span data-stu-id="960c3-122">String</span></span>| <span data-ttu-id="960c3-123">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="960c3-123">The attachment ID.</span></span>|
|<span data-ttu-id="960c3-124">isInline</span><span class="sxs-lookup"><span data-stu-id="960c3-124">isInline</span></span>|<span data-ttu-id="960c3-125">Логический</span><span class="sxs-lookup"><span data-stu-id="960c3-125">Boolean</span></span>|<span data-ttu-id="960c3-126">Значение true указывает, что вложение является встроенным, например внедренным изображением в теле элемента.</span><span class="sxs-lookup"><span data-stu-id="960c3-126">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="960c3-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="960c3-127">lastModifiedDateTime</span></span>|<span data-ttu-id="960c3-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="960c3-128">DateTimeOffset</span></span>|<span data-ttu-id="960c3-129">Время и дата последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="960c3-129">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="960c3-130">name</span><span class="sxs-lookup"><span data-stu-id="960c3-130">name</span></span>|<span data-ttu-id="960c3-131">Строка</span><span class="sxs-lookup"><span data-stu-id="960c3-131">String</span></span>|<span data-ttu-id="960c3-132">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="960c3-132">The display name of the attachment.</span></span>|
|<span data-ttu-id="960c3-133">size</span><span class="sxs-lookup"><span data-stu-id="960c3-133">size</span></span>|<span data-ttu-id="960c3-134">Int32</span><span class="sxs-lookup"><span data-stu-id="960c3-134">Int32</span></span>|<span data-ttu-id="960c3-135">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="960c3-135">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="960c3-136">Связи</span><span class="sxs-lookup"><span data-stu-id="960c3-136">Relationships</span></span>
| <span data-ttu-id="960c3-137">Связь</span><span class="sxs-lookup"><span data-stu-id="960c3-137">Relationship</span></span> | <span data-ttu-id="960c3-138">Тип</span><span class="sxs-lookup"><span data-stu-id="960c3-138">Type</span></span>   |<span data-ttu-id="960c3-139">Описание</span><span class="sxs-lookup"><span data-stu-id="960c3-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="960c3-140">item</span><span class="sxs-lookup"><span data-stu-id="960c3-140">item</span></span>|[<span data-ttu-id="960c3-141">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="960c3-141">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="960c3-p101">Вложенное сообщение или событие. Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="960c3-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="960c3-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="960c3-144">JSON representation</span></span>

<span data-ttu-id="960c3-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="960c3-145">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "@odata.type": "microsoft.graph.itemAttachment",
  "@odata.annotations": [
    {
      "property": "item",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024,
  "item": { "@odata.type": "microsoft.graph.outlookItem" }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
