# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="d854a-101">Тип ресурса domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="d854a-101">domainDnsRecord resource type</span></span>

<span data-ttu-id="d854a-p101">Для работы служб Microsoft Online Services с доменом необходимо добавить записи DNS в файл зоны DNS домена. Объект **DomainDnsRecord** представляет такие записи DNS. Базовый объект для объектов [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) и [DomainDnsSrvRecord](domaindnssrvrecord.md).</span><span class="sxs-lookup"><span data-stu-id="d854a-p101">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services. The **DomainDnsRecord** entity is used to present such DNS records. Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="d854a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d854a-105">Methods</span></span>
<span data-ttu-id="d854a-p102">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="d854a-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="d854a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d854a-108">Properties</span></span>
| <span data-ttu-id="d854a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d854a-109">Property</span></span>     | <span data-ttu-id="d854a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d854a-110">Type</span></span>   |<span data-ttu-id="d854a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d854a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d854a-112">id</span><span class="sxs-lookup"><span data-stu-id="d854a-112">id</span></span>|<span data-ttu-id="d854a-113">String (строка​)</span><span class="sxs-lookup"><span data-stu-id="d854a-113">String</span></span>| <span data-ttu-id="d854a-p103">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d854a-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="d854a-116">isOptional</span><span class="sxs-lookup"><span data-stu-id="d854a-116">isOptional</span></span>|<span data-ttu-id="d854a-117">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="d854a-117">Boolean</span></span>| <span data-ttu-id="d854a-118">Если указано значение false, для правильной работы служб Microsoft Online Services с доменом клиент должен настроить эту запись на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="d854a-118">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="d854a-119">label</span><span class="sxs-lookup"><span data-stu-id="d854a-119">label</span></span>|<span data-ttu-id="d854a-120">String (строка​)</span><span class="sxs-lookup"><span data-stu-id="d854a-120">String</span></span>| <span data-ttu-id="d854a-121">Значение, используемое при настройке имени записи DNS на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="d854a-121">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="d854a-122">recordType</span><span class="sxs-lookup"><span data-stu-id="d854a-122">recordType</span></span>|<span data-ttu-id="d854a-123">String (строка​)</span><span class="sxs-lookup"><span data-stu-id="d854a-123">String</span></span>| <span data-ttu-id="d854a-124">Указывает, какой тип записи DNS представляет этот объект.</span><span class="sxs-lookup"><span data-stu-id="d854a-124">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="d854a-125">Возможные значения: *CName*, *Mx*, *Srv*, *Txt*.</span><span class="sxs-lookup"><span data-stu-id="d854a-125">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="d854a-126">Ключ</span><span class="sxs-lookup"><span data-stu-id="d854a-126">Key</span></span> |
|<span data-ttu-id="d854a-127">supportedService</span><span class="sxs-lookup"><span data-stu-id="d854a-127">supportedService</span></span>|<span data-ttu-id="d854a-128">String (строка​)</span><span class="sxs-lookup"><span data-stu-id="d854a-128">String</span></span>| <span data-ttu-id="d854a-129">Веб-служба или функция Майкрософт, зависящая от этой записи DNS.</span><span class="sxs-lookup"><span data-stu-id="d854a-129">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="d854a-130">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="d854a-130">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="d854a-131">ttl</span><span class="sxs-lookup"><span data-stu-id="d854a-131">ttl</span></span>|<span data-ttu-id="d854a-132">Int32</span><span class="sxs-lookup"><span data-stu-id="d854a-132">Int32</span></span>| <span data-ttu-id="d854a-p104">Значение, используемое при настройке свойства срока жизни (ttl) записи DNS на узле DNS. Не допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="d854a-p104">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="d854a-135">Связи</span><span class="sxs-lookup"><span data-stu-id="d854a-135">Relationships</span></span>
<span data-ttu-id="d854a-136">Нет</span><span class="sxs-lookup"><span data-stu-id="d854a-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d854a-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d854a-137">JSON representation</span></span>
<span data-ttu-id="d854a-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d854a-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->