# <a name="recipient-resource-type"></a><span data-ttu-id="a0209-101">Тип ресурса recipient</span><span class="sxs-lookup"><span data-stu-id="a0209-101">recipient resource type</span></span>

<span data-ttu-id="a0209-102">Представляет сведения о пользователе, который отправляет или получает событие, сообщение или запись в группе.</span><span class="sxs-lookup"><span data-stu-id="a0209-102">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="a0209-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0209-103">Properties</span></span>
| <span data-ttu-id="a0209-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0209-104">Property</span></span>     | <span data-ttu-id="a0209-105">Тип</span><span class="sxs-lookup"><span data-stu-id="a0209-105">Type</span></span>   |<span data-ttu-id="a0209-106">Описание</span><span class="sxs-lookup"><span data-stu-id="a0209-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0209-107">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a0209-107">emailAddress</span></span>|[<span data-ttu-id="a0209-108">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="a0209-108">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="a0209-109">Электронный адрес получателя.</span><span class="sxs-lookup"><span data-stu-id="a0209-109">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0209-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0209-110">JSON representation</span></span>

<span data-ttu-id="a0209-111">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0209-111">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->