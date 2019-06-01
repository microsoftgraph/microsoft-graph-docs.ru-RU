---
title: Тип ресурса domainDnsRecord
description: Для каждого домена в клиенте может потребоваться добавить записи DNS в файл зоны DNS домена, чтобы домен можно было использовать в Microsoft Online Services. Объект **DomainDnsRecord** используется для представления таких DNS-записей. Базовый объект для сущностей Домаинднскнамерекорд, Домаинднсмксрекорд, Домаинднссрврекорд и Домаинднссрврекорд.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2c2bc889be77e2b324450bfd03ce28b3c53f8f51
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657093"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="ad7f3-105">Тип ресурса domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="ad7f3-105">domainDnsRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad7f3-106">Для каждого домена в клиенте может потребоваться добавить записи DNS в файл зоны DNS домена, чтобы домен можно было использовать в Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="ad7f3-106">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="ad7f3-107">Объект **DomainDnsRecord** используется для представления таких DNS-записей.</span><span class="sxs-lookup"><span data-stu-id="ad7f3-107">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="ad7f3-108">Базовый объект для сущностей [домаинднскнамерекорд](domaindnscnamerecord.md), [домаинднсмксрекорд](domaindnsmxrecord.md), [домаинднссрврекорд](domaindnssrvrecord.md) и [домаинднссрврекорд](domaindnssrvrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="ad7f3-108">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="ad7f3-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ad7f3-109">Methods</span></span>
<span data-ttu-id="ad7f3-110">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="ad7f3-110">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="ad7f3-111">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="ad7f3-111">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="ad7f3-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad7f3-112">Properties</span></span>
| <span data-ttu-id="ad7f3-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad7f3-113">Property</span></span>     | <span data-ttu-id="ad7f3-114">Тип</span><span class="sxs-lookup"><span data-stu-id="ad7f3-114">Type</span></span>   |<span data-ttu-id="ad7f3-115">Описание</span><span class="sxs-lookup"><span data-stu-id="ad7f3-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad7f3-116">id</span><span class="sxs-lookup"><span data-stu-id="ad7f3-116">id</span></span>|<span data-ttu-id="ad7f3-117">String</span><span class="sxs-lookup"><span data-stu-id="ad7f3-117">String</span></span>| <span data-ttu-id="ad7f3-118">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="ad7f3-118">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="ad7f3-119">Не допускает значения NULL и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad7f3-119">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="ad7f3-120">Переключатель</span><span class="sxs-lookup"><span data-stu-id="ad7f3-120">isOptional</span></span>|<span data-ttu-id="ad7f3-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad7f3-121">Boolean</span></span>| <span data-ttu-id="ad7f3-122">Если задано значение false, эта запись должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="ad7f3-122">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="ad7f3-123">label</span><span class="sxs-lookup"><span data-stu-id="ad7f3-123">label</span></span>|<span data-ttu-id="ad7f3-124">String</span><span class="sxs-lookup"><span data-stu-id="ad7f3-124">String</span></span>| <span data-ttu-id="ad7f3-125">Значение, используемое при настройке имени DNS-записи на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="ad7f3-125">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="ad7f3-126">recordType</span><span class="sxs-lookup"><span data-stu-id="ad7f3-126">recordType</span></span>|<span data-ttu-id="ad7f3-127">String</span><span class="sxs-lookup"><span data-stu-id="ad7f3-127">String</span></span>| <span data-ttu-id="ad7f3-128">Указывает, какой тип записи DNS представляет эта сущность.</span><span class="sxs-lookup"><span data-stu-id="ad7f3-128">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="ad7f3-129">Может принимать одно из следующих значений: *CNAME*, *MX*, *SRV*, *txt* .</span><span class="sxs-lookup"><span data-stu-id="ad7f3-129">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="ad7f3-130">Key</span><span class="sxs-lookup"><span data-stu-id="ad7f3-130">Key</span></span> |
|<span data-ttu-id="ad7f3-131">Суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="ad7f3-131">supportedService</span></span>|<span data-ttu-id="ad7f3-132">String</span><span class="sxs-lookup"><span data-stu-id="ad7f3-132">String</span></span>| <span data-ttu-id="ad7f3-133">Служба или компонент Microsoft Online, зависящие от этой записи DNS.</span><span class="sxs-lookup"><span data-stu-id="ad7f3-133">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="ad7f3-134">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, \*SharePointPublic \*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="ad7f3-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="ad7f3-135">используем</span><span class="sxs-lookup"><span data-stu-id="ad7f3-135">ttl</span></span>|<span data-ttu-id="ad7f3-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ad7f3-136">Int32</span></span>| <span data-ttu-id="ad7f3-137">Значение, используемое при настройке свойства срока жизни (TTL) записи DNS на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="ad7f3-137">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="ad7f3-138">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="ad7f3-138">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="ad7f3-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="ad7f3-139">Relationships</span></span>
<span data-ttu-id="ad7f3-140">Нет</span><span class="sxs-lookup"><span data-stu-id="ad7f3-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad7f3-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad7f3-141">JSON representation</span></span>
<span data-ttu-id="ad7f3-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad7f3-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
