# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="eb700-101">Тип ресурса domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="eb700-101">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="eb700-p101">Представляет запись типа TXT, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="eb700-p101">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="eb700-104">Методы</span><span class="sxs-lookup"><span data-stu-id="eb700-104">Methods</span></span>
<span data-ttu-id="eb700-p102">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="eb700-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="eb700-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb700-107">Properties</span></span>
| <span data-ttu-id="eb700-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb700-108">Property</span></span>     | <span data-ttu-id="eb700-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eb700-109">Type</span></span>   |<span data-ttu-id="eb700-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eb700-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb700-111">id</span><span class="sxs-lookup"><span data-stu-id="eb700-111">id</span></span>|<span data-ttu-id="eb700-112">String</span><span class="sxs-lookup"><span data-stu-id="eb700-112">String</span></span>| <span data-ttu-id="eb700-p103">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb700-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="eb700-115">isOptional</span><span class="sxs-lookup"><span data-stu-id="eb700-115">isOptional</span></span>|<span data-ttu-id="eb700-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb700-116">Boolean</span></span>| <span data-ttu-id="eb700-117">Если имеет значение false, пользователю необходимо настроить запись типа TXT на узле DNS, чтобы службы Microsoft Online Services правильно работали с доменом.</span><span class="sxs-lookup"><span data-stu-id="eb700-117">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="eb700-118">label</span><span class="sxs-lookup"><span data-stu-id="eb700-118">label</span></span>|<span data-ttu-id="eb700-119">String</span><span class="sxs-lookup"><span data-stu-id="eb700-119">String</span></span>| <span data-ttu-id="eb700-120">Значение, используемое при настройке свойства *name* для записи типа TXT на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="eb700-120">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="eb700-121">recordType</span><span class="sxs-lookup"><span data-stu-id="eb700-121">recordType</span></span>|<span data-ttu-id="eb700-122">String</span><span class="sxs-lookup"><span data-stu-id="eb700-122">String</span></span>| <span data-ttu-id="eb700-p104">Тип записи DNS. Это свойство всегда имеет значение *Txt*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="eb700-p104">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="eb700-126">supportedService</span><span class="sxs-lookup"><span data-stu-id="eb700-126">supportedService</span></span>|<span data-ttu-id="eb700-127">String</span><span class="sxs-lookup"><span data-stu-id="eb700-127">String</span></span>| <span data-ttu-id="eb700-128">Служба или компонент Microsoft Online Services, зависящие от этой записи типа TXT.</span><span class="sxs-lookup"><span data-stu-id="eb700-128">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="eb700-129">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="eb700-129">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="eb700-130">text</span><span class="sxs-lookup"><span data-stu-id="eb700-130">text</span></span>|<span data-ttu-id="eb700-131">String</span><span class="sxs-lookup"><span data-stu-id="eb700-131">String</span></span>| <span data-ttu-id="eb700-132">Значение, используемое при настройке свойства *text* на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="eb700-132">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="eb700-133">ttl</span><span class="sxs-lookup"><span data-stu-id="eb700-133">ttl</span></span>|<span data-ttu-id="eb700-134">Int32</span><span class="sxs-lookup"><span data-stu-id="eb700-134">Int32</span></span>| <span data-ttu-id="eb700-p105">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи MX на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="eb700-p105">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="eb700-137">Связи</span><span class="sxs-lookup"><span data-stu-id="eb700-137">Relationships</span></span>
<span data-ttu-id="eb700-138">Нет</span><span class="sxs-lookup"><span data-stu-id="eb700-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="eb700-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb700-139">JSON representation</span></span>
<span data-ttu-id="eb700-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb700-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
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
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->