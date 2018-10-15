# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="4c5b8-101">Тип ресурса domainDnsMxRecord</span><span class="sxs-lookup"><span data-stu-id="4c5b8-101">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="4c5b8-p101">Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="4c5b8-p101">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="4c5b8-104">Методы</span><span class="sxs-lookup"><span data-stu-id="4c5b8-104">Methods</span></span>
<span data-ttu-id="4c5b8-p102">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="4c5b8-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="4c5b8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c5b8-107">Properties</span></span>
| <span data-ttu-id="4c5b8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c5b8-108">Property</span></span>     | <span data-ttu-id="4c5b8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4c5b8-109">Type</span></span>   |<span data-ttu-id="4c5b8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4c5b8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c5b8-111">id</span><span class="sxs-lookup"><span data-stu-id="4c5b8-111">id</span></span>|<span data-ttu-id="4c5b8-112">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4c5b8-112">String</span></span>| <span data-ttu-id="4c5b8-p103">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="4c5b8-115">isOptional</span><span class="sxs-lookup"><span data-stu-id="4c5b8-115">isOptional</span></span>|<span data-ttu-id="4c5b8-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c5b8-116">Boolean</span></span>| <span data-ttu-id="4c5b8-117">Если указано значение false, для правильной работы Microsoft Online Services с доменом пользователь должен настроить запись MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-117">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="4c5b8-118">label</span><span class="sxs-lookup"><span data-stu-id="4c5b8-118">label</span></span>|<span data-ttu-id="4c5b8-119">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4c5b8-119">String</span></span>| <span data-ttu-id="4c5b8-120">Значение, используемое при настройке свойства *псевдонима, узла или имени* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-120">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="4c5b8-121">mailExchange</span><span class="sxs-lookup"><span data-stu-id="4c5b8-121">mailExchange</span></span>|<span data-ttu-id="4c5b8-122">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4c5b8-122">String</span></span>| <span data-ttu-id="4c5b8-123">Значение, используемое при настройке *значения, ответа или целевого объекта* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-123">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="4c5b8-124">preference</span><span class="sxs-lookup"><span data-stu-id="4c5b8-124">preference</span></span>|<span data-ttu-id="4c5b8-125">Int32</span><span class="sxs-lookup"><span data-stu-id="4c5b8-125">Int32</span></span>| <span data-ttu-id="4c5b8-126">Значение, используемое при настройке свойства *приоритета или предпочтения* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-126">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="4c5b8-127">recordType</span><span class="sxs-lookup"><span data-stu-id="4c5b8-127">recordType</span></span>|<span data-ttu-id="4c5b8-128">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4c5b8-128">String</span></span>| <span data-ttu-id="4c5b8-p104">Тип записи DNS. Это свойство всегда имеет значение *Mx*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-p104">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="4c5b8-132">supportedService</span><span class="sxs-lookup"><span data-stu-id="4c5b8-132">supportedService</span></span>|<span data-ttu-id="4c5b8-133">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4c5b8-133">String</span></span>| <span data-ttu-id="4c5b8-134">Служба или компонент Microsoft Online Services, зависящие от этой записи типа MX.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-134">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="4c5b8-135">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-135">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="4c5b8-136">ttl</span><span class="sxs-lookup"><span data-stu-id="4c5b8-136">ttl</span></span>|<span data-ttu-id="4c5b8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4c5b8-137">Int32</span></span>| <span data-ttu-id="4c5b8-p105">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи MX на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-p105">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="4c5b8-140">Связи</span><span class="sxs-lookup"><span data-stu-id="4c5b8-140">Relationships</span></span>
<span data-ttu-id="4c5b8-141">Нет</span><span class="sxs-lookup"><span data-stu-id="4c5b8-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c5b8-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c5b8-142">JSON representation</span></span>
<span data-ttu-id="4c5b8-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->