# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="bb9b5-101">Тип ресурса domainDnsCnameRecord</span><span class="sxs-lookup"><span data-stu-id="bb9b5-101">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="bb9b5-p101">Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="bb9b5-p101">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="bb9b5-104">Методы</span><span class="sxs-lookup"><span data-stu-id="bb9b5-104">Methods</span></span>
<span data-ttu-id="bb9b5-p102">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="bb9b5-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="bb9b5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb9b5-107">Properties</span></span>
| <span data-ttu-id="bb9b5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb9b5-108">Property</span></span>     | <span data-ttu-id="bb9b5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bb9b5-109">Type</span></span>   |<span data-ttu-id="bb9b5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bb9b5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb9b5-111">canonicalName</span><span class="sxs-lookup"><span data-stu-id="bb9b5-111">canonicalName</span></span>|<span data-ttu-id="bb9b5-112">String (строка)</span><span class="sxs-lookup"><span data-stu-id="bb9b5-112">String</span></span>| <span data-ttu-id="bb9b5-p103">Каноническое имя записи CNAME. Используется для настройки записи CNAME в узле DNS.</span><span class="sxs-lookup"><span data-stu-id="bb9b5-p103">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="bb9b5-115">id</span><span class="sxs-lookup"><span data-stu-id="bb9b5-115">id</span></span>|<span data-ttu-id="bb9b5-116">String (строка)</span><span class="sxs-lookup"><span data-stu-id="bb9b5-116">String</span></span>| <span data-ttu-id="bb9b5-p104">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb9b5-p104">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="bb9b5-119">isOptional</span><span class="sxs-lookup"><span data-stu-id="bb9b5-119">isOptional</span></span>|<span data-ttu-id="bb9b5-120">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="bb9b5-120">Boolean</span></span>| <span data-ttu-id="bb9b5-p105">Если имеет значение false, пользователю необходимо настроить запись CNAME на узле DNS, чтобы службы Microsoft Online Services правильно работали с доменом. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="bb9b5-p105">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="bb9b5-123">label</span><span class="sxs-lookup"><span data-stu-id="bb9b5-123">label</span></span>|<span data-ttu-id="bb9b5-124">String (строка)</span><span class="sxs-lookup"><span data-stu-id="bb9b5-124">String</span></span>| <span data-ttu-id="bb9b5-125">Значение, используемое при настройке *псевдонима, узла и имени* для записи CNAME на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="bb9b5-125">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="bb9b5-126">recordType</span><span class="sxs-lookup"><span data-stu-id="bb9b5-126">recordType</span></span>|<span data-ttu-id="bb9b5-127">String (строка)</span><span class="sxs-lookup"><span data-stu-id="bb9b5-127">String</span></span>| <span data-ttu-id="bb9b5-p106">Тип записи DNS. Это свойство всегда имеет значение *CName*. Ключевое.</span><span class="sxs-lookup"><span data-stu-id="bb9b5-p106">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="bb9b5-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="bb9b5-131">supportedService</span></span>|<span data-ttu-id="bb9b5-132">String (строка)</span><span class="sxs-lookup"><span data-stu-id="bb9b5-132">String</span></span>| <span data-ttu-id="bb9b5-133">Служба или функция Microsoft Online, имеющая зависимость от этой записи CNAME.</span><span class="sxs-lookup"><span data-stu-id="bb9b5-133">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="bb9b5-134">Может иметь одно из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer* или *Intune*.</span><span class="sxs-lookup"><span data-stu-id="bb9b5-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="bb9b5-135">ttl</span><span class="sxs-lookup"><span data-stu-id="bb9b5-135">ttl</span></span>|<span data-ttu-id="bb9b5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9b5-136">Int32</span></span>| <span data-ttu-id="bb9b5-p107">Значение, используемое при настройке свойства срока жизни (ttl) записи CNAME на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="bb9b5-p107">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="bb9b5-139">Связи</span><span class="sxs-lookup"><span data-stu-id="bb9b5-139">Relationships</span></span>
<span data-ttu-id="bb9b5-140">Нет</span><span class="sxs-lookup"><span data-stu-id="bb9b5-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bb9b5-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb9b5-141">JSON representation</span></span>
<span data-ttu-id="bb9b5-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb9b5-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
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
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->