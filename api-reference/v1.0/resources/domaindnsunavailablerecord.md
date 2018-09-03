# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="67c8e-101">Тип ресурса domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="67c8e-101">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="67c8e-p101">Когда вы запрашиваете объект [Domain](domain.md) в свойстве навигации **serviceConfigurationRecords**, то может быть возвращен один или несколько объектов [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) или [DomainDnsTxtRecord](domaindnstxtrecord.md). Эти объекты указывают, какие записи DNS необходимо добавить в файл зоны домена, чтобы службы Microsoft Online Services могли использовать этот домен. Если не удается создать такие объекты, то вместо них будет возвращен объект DomainDnsUnavailableRecord. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="67c8e-p101">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="67c8e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="67c8e-106">Methods</span></span>
<span data-ttu-id="67c8e-p102">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="67c8e-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="67c8e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="67c8e-109">Properties</span></span>
| <span data-ttu-id="67c8e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="67c8e-110">Property</span></span>     | <span data-ttu-id="67c8e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="67c8e-111">Type</span></span>   |<span data-ttu-id="67c8e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="67c8e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67c8e-113">description</span><span class="sxs-lookup"><span data-stu-id="67c8e-113">description</span></span>|<span data-ttu-id="67c8e-114">Строка</span><span class="sxs-lookup"><span data-stu-id="67c8e-114">String</span></span>|<span data-ttu-id="67c8e-115">Указывает причину, по которой возвращен объект **DomainDnsUnavailableRecord**.</span><span class="sxs-lookup"><span data-stu-id="67c8e-115">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="67c8e-116">Связи</span><span class="sxs-lookup"><span data-stu-id="67c8e-116">Relationships</span></span>
<span data-ttu-id="67c8e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="67c8e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67c8e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67c8e-118">JSON representation</span></span>
<span data-ttu-id="67c8e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67c8e-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "description": "String"
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