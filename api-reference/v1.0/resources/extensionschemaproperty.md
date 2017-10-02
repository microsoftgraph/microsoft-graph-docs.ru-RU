# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="1696a-101">Тип ресурса extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="1696a-101">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="1696a-102">Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="1696a-102">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="1696a-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="1696a-103">Properties</span></span>
| <span data-ttu-id="1696a-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="1696a-104">Property</span></span>     | <span data-ttu-id="1696a-105">Тип</span><span class="sxs-lookup"><span data-stu-id="1696a-105">Type</span></span>   |<span data-ttu-id="1696a-106">Описание</span><span class="sxs-lookup"><span data-stu-id="1696a-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1696a-107">name</span><span class="sxs-lookup"><span data-stu-id="1696a-107">name</span></span>|<span data-ttu-id="1696a-108">String</span><span class="sxs-lookup"><span data-stu-id="1696a-108">String</span></span>| <span data-ttu-id="1696a-109">Имя строго типизированного свойства, определенного в качестве части расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="1696a-109">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="1696a-110">type</span><span class="sxs-lookup"><span data-stu-id="1696a-110">type</span></span>|<span data-ttu-id="1696a-111">Строка</span><span class="sxs-lookup"><span data-stu-id="1696a-111">String</span></span>| <span data-ttu-id="1696a-p101">Тип свойства, определенного в качестве части расширения схемы.  Разрешенные значения: *Binary, Boolean, DateTime, Integer* или *String*.  Дополнительные сведения см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="1696a-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="1696a-115">Поддерживаемые типы данных свойств</span><span class="sxs-lookup"><span data-stu-id="1696a-115">Supported property data types</span></span> 
<span data-ttu-id="1696a-116">При определении свойства в расширении схемы поддерживаются следующие типы данных:</span><span class="sxs-lookup"><span data-stu-id="1696a-116">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="1696a-117">Тип свойства</span><span class="sxs-lookup"><span data-stu-id="1696a-117">Property Type</span></span> | <span data-ttu-id="1696a-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="1696a-118">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="1696a-119">Binary</span><span class="sxs-lookup"><span data-stu-id="1696a-119">Binary</span></span> | <span data-ttu-id="1696a-120">Не более 256 байт.</span><span class="sxs-lookup"><span data-stu-id="1696a-120">256 bytes maximum.</span></span> |
| <span data-ttu-id="1696a-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="1696a-121">Boolean</span></span> | <span data-ttu-id="1696a-122">Не поддерживается для ресурсов contact, message, event и post.</span><span class="sxs-lookup"><span data-stu-id="1696a-122">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="1696a-123">DateTime</span><span class="sxs-lookup"><span data-stu-id="1696a-123">DateTime</span></span> | <span data-ttu-id="1696a-p102">Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="1696a-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="1696a-126">Integer</span><span class="sxs-lookup"><span data-stu-id="1696a-126">Integer</span></span> | <span data-ttu-id="1696a-127">32-разрядное значение.</span><span class="sxs-lookup"><span data-stu-id="1696a-127">A 32-bit integer value.</span></span> <span data-ttu-id="1696a-128">Не поддерживается для ресурсов contact, message, event и post.</span><span class="sxs-lookup"><span data-stu-id="1696a-128">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="1696a-129">String</span><span class="sxs-lookup"><span data-stu-id="1696a-129">String</span></span> | <span data-ttu-id="1696a-130">Не более 256 символов.</span><span class="sxs-lookup"><span data-stu-id="1696a-130">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1696a-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1696a-131">JSON representation</span></span>
<span data-ttu-id="1696a-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1696a-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
