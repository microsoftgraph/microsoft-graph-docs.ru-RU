# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="9761b-101">Тип ресурса domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="9761b-101">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="9761b-p101">Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="9761b-p101">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="9761b-104">Методы</span><span class="sxs-lookup"><span data-stu-id="9761b-104">Methods</span></span>
<span data-ttu-id="9761b-p102">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="9761b-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="9761b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9761b-107">Properties</span></span>
| <span data-ttu-id="9761b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9761b-108">Property</span></span>     | <span data-ttu-id="9761b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9761b-109">Type</span></span>   |<span data-ttu-id="9761b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9761b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9761b-111">id</span><span class="sxs-lookup"><span data-stu-id="9761b-111">id</span></span>|<span data-ttu-id="9761b-112">Строка</span><span class="sxs-lookup"><span data-stu-id="9761b-112">String</span></span>| <span data-ttu-id="9761b-p103">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9761b-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="9761b-115">isOptional</span><span class="sxs-lookup"><span data-stu-id="9761b-115">isOptional</span></span>|<span data-ttu-id="9761b-116">Логический</span><span class="sxs-lookup"><span data-stu-id="9761b-116">Boolean</span></span>| <span data-ttu-id="9761b-117">Если указано значение false, для правильной работы Microsoft Online Services с доменом пользователь должен настроить запись SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="9761b-117">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="9761b-118">label</span><span class="sxs-lookup"><span data-stu-id="9761b-118">label</span></span>|<span data-ttu-id="9761b-119">Строка</span><span class="sxs-lookup"><span data-stu-id="9761b-119">String</span></span>| <span data-ttu-id="9761b-120">Значение, используемое при настройке свойства *name* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="9761b-120">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="9761b-121">nameTarget</span><span class="sxs-lookup"><span data-stu-id="9761b-121">nameTarget</span></span>|<span data-ttu-id="9761b-122">Строка</span><span class="sxs-lookup"><span data-stu-id="9761b-122">String</span></span>| <span data-ttu-id="9761b-123">Значение, используемое при настройке свойства *Target* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="9761b-123">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="9761b-124">port</span><span class="sxs-lookup"><span data-stu-id="9761b-124">port</span></span>|<span data-ttu-id="9761b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9761b-125">Int32</span></span>| <span data-ttu-id="9761b-126">Значение, используемое при настройке свойства *port* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="9761b-126">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="9761b-127">priority</span><span class="sxs-lookup"><span data-stu-id="9761b-127">priority</span></span>|<span data-ttu-id="9761b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9761b-128">Int32</span></span>| <span data-ttu-id="9761b-129">Значение, используемое при настройке свойства *priority* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="9761b-129">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="9761b-130">protocol</span><span class="sxs-lookup"><span data-stu-id="9761b-130">protocol</span></span>|<span data-ttu-id="9761b-131">Строка</span><span class="sxs-lookup"><span data-stu-id="9761b-131">String</span></span>| <span data-ttu-id="9761b-132">Значение, используемое при настройке свойства *protocol* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="9761b-132">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="9761b-133">recordType</span><span class="sxs-lookup"><span data-stu-id="9761b-133">recordType</span></span>|<span data-ttu-id="9761b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9761b-134">String</span></span>|  <span data-ttu-id="9761b-p104">Тип записи DNS. Это свойство всегда имеет значение *Srv*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="9761b-p104">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="9761b-138">service</span><span class="sxs-lookup"><span data-stu-id="9761b-138">service</span></span>|<span data-ttu-id="9761b-139">Строка</span><span class="sxs-lookup"><span data-stu-id="9761b-139">String</span></span>| <span data-ttu-id="9761b-140">Значение, используемое при настройке свойства *service* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="9761b-140">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="9761b-141">supportedService</span><span class="sxs-lookup"><span data-stu-id="9761b-141">supportedService</span></span>|<span data-ttu-id="9761b-142">Строка</span><span class="sxs-lookup"><span data-stu-id="9761b-142">String</span></span>| <span data-ttu-id="9761b-143">Служба или компонент Microsoft Online Services, зависящие от этой записи типа SRV.</span><span class="sxs-lookup"><span data-stu-id="9761b-143">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="9761b-144">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="9761b-144">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="9761b-145">ttl</span><span class="sxs-lookup"><span data-stu-id="9761b-145">ttl</span></span>|<span data-ttu-id="9761b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9761b-146">Int32</span></span>| <span data-ttu-id="9761b-p105">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи SRV на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="9761b-p105">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="9761b-149">weight</span><span class="sxs-lookup"><span data-stu-id="9761b-149">weight</span></span>|<span data-ttu-id="9761b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9761b-150">Int32</span></span>| <span data-ttu-id="9761b-151">Значение, используемое при настройке свойства *weight* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="9761b-151">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9761b-152">Связи</span><span class="sxs-lookup"><span data-stu-id="9761b-152">Relationships</span></span>
<span data-ttu-id="9761b-153">Нет</span><span class="sxs-lookup"><span data-stu-id="9761b-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9761b-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9761b-154">JSON representation</span></span>
<span data-ttu-id="9761b-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9761b-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->