# <a name="verifieddomain-resource-type"></a><span data-ttu-id="2d1fe-101">Тип ресурса verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="2d1fe-101">verifiedDomain resource type</span></span>

<span data-ttu-id="2d1fe-p101">Задает домен клиента. Свойство **verifiedDomains** объекта [organization](organization.md) представляет собой коллекцию объектов **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="2d1fe-p101">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="2d1fe-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d1fe-104">Properties</span></span>
| <span data-ttu-id="2d1fe-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d1fe-105">Property</span></span>     | <span data-ttu-id="2d1fe-106">Тип</span><span class="sxs-lookup"><span data-stu-id="2d1fe-106">Type</span></span>   |<span data-ttu-id="2d1fe-107">Описание</span><span class="sxs-lookup"><span data-stu-id="2d1fe-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d1fe-108">capabilities</span><span class="sxs-lookup"><span data-stu-id="2d1fe-108">capabilities</span></span>|<span data-ttu-id="2d1fe-109">String</span><span class="sxs-lookup"><span data-stu-id="2d1fe-109">String</span></span>|<span data-ttu-id="2d1fe-110">Примеры: “Email”, “OfficeCommunicationsOnline”.</span><span class="sxs-lookup"><span data-stu-id="2d1fe-110">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="2d1fe-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="2d1fe-111">isDefault</span></span>|<span data-ttu-id="2d1fe-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d1fe-112">Boolean</span></span>|                <span data-ttu-id="2d1fe-113">Значение **true** указывает, что это связанный с клиентом домен по умолчанию. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="2d1fe-113">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="2d1fe-114">isInitial</span><span class="sxs-lookup"><span data-stu-id="2d1fe-114">isInitial</span></span>|<span data-ttu-id="2d1fe-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d1fe-115">Boolean</span></span>|<span data-ttu-id="2d1fe-116">Значение **true** указывает, что это первоначальный домен, связанный с клиентом. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="2d1fe-116">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="2d1fe-117">name</span><span class="sxs-lookup"><span data-stu-id="2d1fe-117">name</span></span>|<span data-ttu-id="2d1fe-118">String</span><span class="sxs-lookup"><span data-stu-id="2d1fe-118">String</span></span>|<span data-ttu-id="2d1fe-119">Доменное имя, например "contoso.onmicrosoft.com"</span><span class="sxs-lookup"><span data-stu-id="2d1fe-119">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="2d1fe-120">type</span><span class="sxs-lookup"><span data-stu-id="2d1fe-120">type</span></span>|<span data-ttu-id="2d1fe-121">String</span><span class="sxs-lookup"><span data-stu-id="2d1fe-121">String</span></span>|<span data-ttu-id="2d1fe-122">Пример: "Managed".</span><span class="sxs-lookup"><span data-stu-id="2d1fe-122">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d1fe-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d1fe-123">JSON representation</span></span>

<span data-ttu-id="2d1fe-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d1fe-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
