# <a name="emailaddress-resource-type"></a><span data-ttu-id="e4259-101">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="e4259-101">emailAddress resource type</span></span>

<span data-ttu-id="e4259-102">Имя и электронный адрес контакта или получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="e4259-102">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="e4259-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4259-103">Properties</span></span>
| <span data-ttu-id="e4259-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4259-104">Property</span></span>     | <span data-ttu-id="e4259-105">Тип</span><span class="sxs-lookup"><span data-stu-id="e4259-105">Type</span></span>   |<span data-ttu-id="e4259-106">Описание</span><span class="sxs-lookup"><span data-stu-id="e4259-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4259-107">address</span><span class="sxs-lookup"><span data-stu-id="e4259-107">address</span></span>|<span data-ttu-id="e4259-108">String</span><span class="sxs-lookup"><span data-stu-id="e4259-108">String</span></span>|<span data-ttu-id="e4259-109">Электронный адрес человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="e4259-109">The email address of the person or entity.</span></span>|
|<span data-ttu-id="e4259-110">name</span><span class="sxs-lookup"><span data-stu-id="e4259-110">name</span></span>|<span data-ttu-id="e4259-111">String</span><span class="sxs-lookup"><span data-stu-id="e4259-111">String</span></span>|<span data-ttu-id="e4259-112">Отображаемое имя человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="e4259-112">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4259-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4259-113">JSON representation</span></span>

<span data-ttu-id="e4259-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4259-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
