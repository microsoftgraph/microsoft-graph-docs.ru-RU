# <a name="itemreference-resource-type"></a><span data-ttu-id="8ac70-101">Тип ресурса ItemReference</span><span class="sxs-lookup"><span data-stu-id="8ac70-101">ItemReference resource type</span></span>

<span data-ttu-id="8ac70-102">Ресурс **ItemReference** предоставляет сведения, необходимые для обращения к ресурсу [DriveItem](driveitem.md) через API.</span><span class="sxs-lookup"><span data-stu-id="8ac70-102">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ac70-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ac70-103">JSON representation</span></span>

<span data-ttu-id="8ac70-104">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="8ac70-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a><span data-ttu-id="8ac70-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ac70-105">Properties</span></span>

| <span data-ttu-id="8ac70-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ac70-106">Property</span></span>      | <span data-ttu-id="8ac70-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8ac70-107">Type</span></span>                              | <span data-ttu-id="8ac70-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8ac70-108">Description</span></span>                                                                                                |
| :------------ | :-------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8ac70-109">driveId</span><span class="sxs-lookup"><span data-stu-id="8ac70-109">driveId</span></span>       | <span data-ttu-id="8ac70-110">String</span><span class="sxs-lookup"><span data-stu-id="8ac70-110">String</span></span>                            | <span data-ttu-id="8ac70-p101">Уникальный идентификатор экземпляра диска, содержащего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ac70-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>                                 |
| <span data-ttu-id="8ac70-113">id</span><span class="sxs-lookup"><span data-stu-id="8ac70-113">id</span></span>            | <span data-ttu-id="8ac70-114">String</span><span class="sxs-lookup"><span data-stu-id="8ac70-114">String</span></span>                            | <span data-ttu-id="8ac70-p102">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ac70-p102">Unique identifier of the item in the drive. Read-only.</span></span>                                                     |
| <span data-ttu-id="8ac70-117">name</span><span class="sxs-lookup"><span data-stu-id="8ac70-117">name</span></span>          | <span data-ttu-id="8ac70-118">Строка</span><span class="sxs-lookup"><span data-stu-id="8ac70-118">String</span></span>                            | <span data-ttu-id="8ac70-p103">Имя элемента, на который направлена ссылка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ac70-p103">The name of the item being referenced. Read-only.</span></span>                                                          |
| <span data-ttu-id="8ac70-121">path</span><span class="sxs-lookup"><span data-stu-id="8ac70-121">path</span></span>          | <span data-ttu-id="8ac70-122">String</span><span class="sxs-lookup"><span data-stu-id="8ac70-122">String</span></span>                            | <span data-ttu-id="8ac70-p104">Путь, по которому можно перейти к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ac70-p104">Path that can be used to navigate to the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="8ac70-125">shareId</span><span class="sxs-lookup"><span data-stu-id="8ac70-125">shareId</span></span>       | <span data-ttu-id="8ac70-126">String</span><span class="sxs-lookup"><span data-stu-id="8ac70-126">String</span></span>                            | <span data-ttu-id="8ac70-127">Уникальный идентификатор общего ресурса, доступ к которому можно получить с помощью API [Shares](../api/shares_get.md).</span><span class="sxs-lookup"><span data-stu-id="8ac70-127">A unique identifier for a shared resource that can be accessed via the [Shares](../api/shares_get.md) API.</span></span> |
| <span data-ttu-id="8ac70-128">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="8ac70-128">sharepointIds</span></span> | [<span data-ttu-id="8ac70-129">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="8ac70-129">sharepointIds</span></span>](sharepointids.md) | <span data-ttu-id="8ac70-p105">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ac70-p105">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                   |

## <a name="remarks"></a><span data-ttu-id="8ac70-132">Заметки</span><span class="sxs-lookup"><span data-stu-id="8ac70-132">Remarks</span></span>

<span data-ttu-id="8ac70-133">Чтобы обратиться к элементу **driveItem** из ресурса **itemReference**, составьте URL-адрес в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="8ac70-133">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="8ac70-134">Значение **path** — это путь к API относительно целевого диска, например: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="8ac70-134">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="8ac70-135">Чтобы получить удобочитаемый путь для навигации, вы можете пропустить все до первого символа `:` в строке пути.</span><span class="sxs-lookup"><span data-stu-id="8ac70-135">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
