# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="5a644-101">Тип ресурса WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="5a644-101">WorksheetProtection resource type</span></span>

<span data-ttu-id="5a644-102">Представляет защиту объекта листа.</span><span class="sxs-lookup"><span data-stu-id="5a644-102">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="5a644-103">Методы</span><span class="sxs-lookup"><span data-stu-id="5a644-103">Methods</span></span>

| <span data-ttu-id="5a644-104">Метод</span><span class="sxs-lookup"><span data-stu-id="5a644-104">Method</span></span>           | <span data-ttu-id="5a644-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5a644-105">Return Type</span></span>    |<span data-ttu-id="5a644-106">Описание</span><span class="sxs-lookup"><span data-stu-id="5a644-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5a644-107">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="5a644-107">Get WorksheetProtection</span></span>](../api/worksheetprotection_get.md) | [<span data-ttu-id="5a644-108">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="5a644-108">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="5a644-109">Чтение свойств и связей объекта worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="5a644-109">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="5a644-110">Protect</span><span class="sxs-lookup"><span data-stu-id="5a644-110">Protect</span></span>](../api/worksheetprotection_protect.md)|<span data-ttu-id="5a644-111">None</span><span class="sxs-lookup"><span data-stu-id="5a644-111">None</span></span>|<span data-ttu-id="5a644-p101">Защищает лист. Выдает исключение, если лист защищен.</span><span class="sxs-lookup"><span data-stu-id="5a644-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="5a644-114">Unprotect</span><span class="sxs-lookup"><span data-stu-id="5a644-114">Unprotect</span></span>](../api/worksheetprotection_unprotect.md)|<span data-ttu-id="5a644-115">None</span><span class="sxs-lookup"><span data-stu-id="5a644-115">None</span></span>|<span data-ttu-id="5a644-116">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="5a644-116">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="5a644-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a644-117">Properties</span></span>
| <span data-ttu-id="5a644-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a644-118">Property</span></span>     | <span data-ttu-id="5a644-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5a644-119">Type</span></span>   |<span data-ttu-id="5a644-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5a644-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a644-121">options</span><span class="sxs-lookup"><span data-stu-id="5a644-121">options</span></span>|[<span data-ttu-id="5a644-122">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="5a644-122">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="5a644-p102">Параметры защиты листа. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a644-p102">Sheet protection options. Read-only.</span></span>|
|<span data-ttu-id="5a644-125">protected</span><span class="sxs-lookup"><span data-stu-id="5a644-125">protected</span></span>|<span data-ttu-id="5a644-126">boolean</span><span class="sxs-lookup"><span data-stu-id="5a644-126">boolean</span></span>|<span data-ttu-id="5a644-p103">Указывает, защищен ли лист.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a644-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a644-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a644-129">JSON representation</span></span>

<span data-ttu-id="5a644-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a644-130">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->