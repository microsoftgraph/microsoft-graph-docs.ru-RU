# <a name="sizerange-resource-type"></a><span data-ttu-id="02d26-101">Тип ресурса sizeRange</span><span class="sxs-lookup"><span data-stu-id="02d26-101">sizeRange resource type</span></span>


<span data-ttu-id="02d26-102">Указывает максимальный и минимальный размеры (в килобайтах) входящего сообщения, при которых применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="02d26-102">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="02d26-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="02d26-103">Properties</span></span>
| <span data-ttu-id="02d26-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="02d26-104">Property</span></span>     | <span data-ttu-id="02d26-105">Тип</span><span class="sxs-lookup"><span data-stu-id="02d26-105">Type</span></span>   |<span data-ttu-id="02d26-106">Описание</span><span class="sxs-lookup"><span data-stu-id="02d26-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="02d26-107">maximumSize</span><span class="sxs-lookup"><span data-stu-id="02d26-107">maximumSize</span></span> | <span data-ttu-id="02d26-108">Int32</span><span class="sxs-lookup"><span data-stu-id="02d26-108">Int32</span></span> | <span data-ttu-id="02d26-109">Максимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="02d26-109">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="02d26-110">minimumSize</span><span class="sxs-lookup"><span data-stu-id="02d26-110">minimumSize</span></span> | <span data-ttu-id="02d26-111">Int32</span><span class="sxs-lookup"><span data-stu-id="02d26-111">Int32</span></span> | <span data-ttu-id="02d26-112">Минимальный размер (в килобайтах) входящего сообщения, при котором применяется условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="02d26-112">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="02d26-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02d26-113">JSON representation</span></span>
<span data-ttu-id="02d26-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02d26-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->