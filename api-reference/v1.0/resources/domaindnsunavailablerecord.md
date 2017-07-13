<span data-ttu-id="876a1-p102">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="876a1-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>
Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).

## <span data-ttu-id="876a1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="876a1-109">Properties</span></span>
<a id="properties" class="xliff"></a>
| <span data-ttu-id="876a1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="876a1-110">Property</span></span>     | <span data-ttu-id="876a1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="876a1-111">Type</span></span>   |<span data-ttu-id="876a1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="876a1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="876a1-113">description</span><span class="sxs-lookup"><span data-stu-id="876a1-113">description</span></span>|<span data-ttu-id="876a1-114">String</span><span class="sxs-lookup"><span data-stu-id="876a1-114">String</span></span>|<span data-ttu-id="876a1-115">Указывает причину, по которой возвращен объект **DomainDnsUnavailableRecord**.</span><span class="sxs-lookup"><span data-stu-id="876a1-115">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <span data-ttu-id="876a1-116">Связи</span><span class="sxs-lookup"><span data-stu-id="876a1-116">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="876a1-117">Нет</span><span class="sxs-lookup"><span data-stu-id="876a1-117">None</span></span>

## <span data-ttu-id="876a1-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="876a1-118">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="876a1-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="876a1-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->