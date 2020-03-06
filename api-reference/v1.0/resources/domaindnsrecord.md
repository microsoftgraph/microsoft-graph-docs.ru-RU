---
title: Тип ресурса domainDnsRecord
description: Для каждого домена в клиенте может потребоваться добавить записи DNS в файл зоны DNS домена, чтобы домен можно было использовать в Microsoft Online Services. Объект **DomainDnsRecord** используется для представления таких DNS-записей. Базовый объект для сущностей Домаинднскнамерекорд, Домаинднсмксрекорд, Домаинднссрврекорд и Домаинднсткстрекорд.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9402ec0785da87236fa94a9749f8b400f3164e1e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531603"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="157c4-105">Тип ресурса domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="157c4-105">domainDnsRecord resource type</span></span>

<span data-ttu-id="157c4-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="157c4-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="157c4-107">Для каждого домена в клиенте может потребоваться добавить записи DNS в файл зоны DNS домена, чтобы домен можно было использовать в Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="157c4-107">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="157c4-108">Объект **DomainDnsRecord** используется для представления таких DNS-записей.</span><span class="sxs-lookup"><span data-stu-id="157c4-108">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="157c4-109">Базовый объект для сущностей [домаинднскнамерекорд](domaindnscnamerecord.md), [домаинднсмксрекорд](domaindnsmxrecord.md), [домаинднссрврекорд](domaindnssrvrecord.md) и [домаинднсткстрекорд](domaindnstxtrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="157c4-109">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="157c4-110">Методы</span><span class="sxs-lookup"><span data-stu-id="157c4-110">Methods</span></span>
<span data-ttu-id="157c4-111">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="157c4-111">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="157c4-112">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="157c4-112">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="157c4-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="157c4-113">Properties</span></span>
| <span data-ttu-id="157c4-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="157c4-114">Property</span></span>     | <span data-ttu-id="157c4-115">Тип</span><span class="sxs-lookup"><span data-stu-id="157c4-115">Type</span></span>   |<span data-ttu-id="157c4-116">Описание</span><span class="sxs-lookup"><span data-stu-id="157c4-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="157c4-117">id</span><span class="sxs-lookup"><span data-stu-id="157c4-117">id</span></span>|<span data-ttu-id="157c4-118">Строка</span><span class="sxs-lookup"><span data-stu-id="157c4-118">String</span></span>| <span data-ttu-id="157c4-119">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="157c4-119">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="157c4-120">Не допускает значения NULL и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="157c4-120">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="157c4-121">Переключатель</span><span class="sxs-lookup"><span data-stu-id="157c4-121">isOptional</span></span>|<span data-ttu-id="157c4-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="157c4-122">Boolean</span></span>| <span data-ttu-id="157c4-123">Если задано значение false, эта запись должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="157c4-123">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="157c4-124">label</span><span class="sxs-lookup"><span data-stu-id="157c4-124">label</span></span>|<span data-ttu-id="157c4-125">Строка</span><span class="sxs-lookup"><span data-stu-id="157c4-125">String</span></span>| <span data-ttu-id="157c4-126">Значение, используемое при настройке имени DNS-записи на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="157c4-126">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="157c4-127">recordType</span><span class="sxs-lookup"><span data-stu-id="157c4-127">recordType</span></span>|<span data-ttu-id="157c4-128">Строка</span><span class="sxs-lookup"><span data-stu-id="157c4-128">String</span></span>| <span data-ttu-id="157c4-129">Указывает, какой тип записи DNS представляет эта сущность.</span><span class="sxs-lookup"><span data-stu-id="157c4-129">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="157c4-130">Может принимать одно из следующих значений: *CNAME*, *MX*, *SRV*, *txt* .</span><span class="sxs-lookup"><span data-stu-id="157c4-130">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="157c4-131">Key</span><span class="sxs-lookup"><span data-stu-id="157c4-131">Key</span></span> |
|<span data-ttu-id="157c4-132">суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="157c4-132">supportedService</span></span>|<span data-ttu-id="157c4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="157c4-133">String</span></span>| <span data-ttu-id="157c4-134">Служба или компонент Microsoft Online, зависящие от этой записи DNS.</span><span class="sxs-lookup"><span data-stu-id="157c4-134">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="157c4-135">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="157c4-135">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="157c4-136">используем</span><span class="sxs-lookup"><span data-stu-id="157c4-136">ttl</span></span>|<span data-ttu-id="157c4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="157c4-137">Int32</span></span>| <span data-ttu-id="157c4-138">Значение, используемое при настройке свойства срока жизни (TTL) записи DNS на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="157c4-138">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="157c4-139">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="157c4-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="157c4-140">Связи</span><span class="sxs-lookup"><span data-stu-id="157c4-140">Relationships</span></span>
<span data-ttu-id="157c4-141">Нет</span><span class="sxs-lookup"><span data-stu-id="157c4-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="157c4-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="157c4-142">JSON representation</span></span>
<span data-ttu-id="157c4-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="157c4-143">Here is a JSON representation of the resource.</span></span>

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
