---
title: Тип ресурса domainDnsRecord
description: Для каждого домена в клиенте может потребоваться добавить записи DNS в файл зоны DNS домена, чтобы домен можно было использовать в Microsoft Online Services. Объект **DomainDnsRecord** используется для представления таких DNS-записей. Базовый объект для сущностей Домаинднскнамерекорд, Домаинднсмксрекорд, Домаинднссрврекорд и Домаинднссрврекорд.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a590895a905852b37c7cc14b0390573c7b57e72f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029430"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="6950b-105">Тип ресурса domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="6950b-105">domainDnsRecord resource type</span></span>

<span data-ttu-id="6950b-106">Для каждого домена в клиенте может потребоваться добавить записи DNS в файл зоны DNS домена, чтобы домен можно было использовать в Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="6950b-106">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="6950b-107">Объект **DomainDnsRecord** используется для представления таких DNS-записей.</span><span class="sxs-lookup"><span data-stu-id="6950b-107">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="6950b-108">Базовый объект для сущностей [домаинднскнамерекорд](domaindnscnamerecord.md), [домаинднсмксрекорд](domaindnsmxrecord.md), [домаинднссрврекорд](domaindnssrvrecord.md) и [домаинднссрврекорд](domaindnssrvrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="6950b-108">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="6950b-109">Методы</span><span class="sxs-lookup"><span data-stu-id="6950b-109">Methods</span></span>
<span data-ttu-id="6950b-110">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="6950b-110">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="6950b-111">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="6950b-111">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="6950b-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="6950b-112">Properties</span></span>
| <span data-ttu-id="6950b-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="6950b-113">Property</span></span>     | <span data-ttu-id="6950b-114">Тип</span><span class="sxs-lookup"><span data-stu-id="6950b-114">Type</span></span>   |<span data-ttu-id="6950b-115">Описание</span><span class="sxs-lookup"><span data-stu-id="6950b-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6950b-116">id</span><span class="sxs-lookup"><span data-stu-id="6950b-116">id</span></span>|<span data-ttu-id="6950b-117">String</span><span class="sxs-lookup"><span data-stu-id="6950b-117">String</span></span>| <span data-ttu-id="6950b-118">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="6950b-118">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="6950b-119">Не допускает значения NULL и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6950b-119">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="6950b-120">Переключатель</span><span class="sxs-lookup"><span data-stu-id="6950b-120">isOptional</span></span>|<span data-ttu-id="6950b-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="6950b-121">Boolean</span></span>| <span data-ttu-id="6950b-122">Если задано значение false, эта запись должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="6950b-122">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="6950b-123">label</span><span class="sxs-lookup"><span data-stu-id="6950b-123">label</span></span>|<span data-ttu-id="6950b-124">String</span><span class="sxs-lookup"><span data-stu-id="6950b-124">String</span></span>| <span data-ttu-id="6950b-125">Значение, используемое при настройке имени DNS-записи на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="6950b-125">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="6950b-126">recordType</span><span class="sxs-lookup"><span data-stu-id="6950b-126">recordType</span></span>|<span data-ttu-id="6950b-127">String</span><span class="sxs-lookup"><span data-stu-id="6950b-127">String</span></span>| <span data-ttu-id="6950b-128">Указывает, какой тип записи DNS представляет эта сущность.</span><span class="sxs-lookup"><span data-stu-id="6950b-128">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="6950b-129">Может принимать одно из следующих значений: *CNAME*, *MX*, *SRV*, *txt* .</span><span class="sxs-lookup"><span data-stu-id="6950b-129">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="6950b-130">Key</span><span class="sxs-lookup"><span data-stu-id="6950b-130">Key</span></span> |
|<span data-ttu-id="6950b-131">Суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="6950b-131">supportedService</span></span>|<span data-ttu-id="6950b-132">String</span><span class="sxs-lookup"><span data-stu-id="6950b-132">String</span></span>| <span data-ttu-id="6950b-133">Служба или компонент Microsoft Online, зависящие от этой записи DNS.</span><span class="sxs-lookup"><span data-stu-id="6950b-133">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="6950b-134">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, \*SharePointPublic \*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="6950b-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="6950b-135">используем</span><span class="sxs-lookup"><span data-stu-id="6950b-135">ttl</span></span>|<span data-ttu-id="6950b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6950b-136">Int32</span></span>| <span data-ttu-id="6950b-137">Значение, используемое при настройке свойства срока жизни (TTL) записи DNS на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="6950b-137">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="6950b-138">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="6950b-138">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="6950b-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="6950b-139">Relationships</span></span>
<span data-ttu-id="6950b-140">Нет</span><span class="sxs-lookup"><span data-stu-id="6950b-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6950b-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6950b-141">JSON representation</span></span>
<span data-ttu-id="6950b-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6950b-142">Here is a JSON representation of the resource.</span></span>

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
