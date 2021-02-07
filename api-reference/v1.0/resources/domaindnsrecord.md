---
title: Тип ресурса domainDnsRecord
description: Объект DomainDnsRecord используется для представить записи DNS.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ba4955c670548b3670dc90a574bc1b4fd8a11c58
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135109"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="b1098-103">Тип ресурса domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="b1098-103">domainDnsRecord resource type</span></span>

<span data-ttu-id="b1098-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1098-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1098-105">Для каждого домена в клиенте может потребоваться добавить записи DNS в DNS-файл зоны домена, прежде чем домен сможет использоваться Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="b1098-105">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="b1098-106">Объект **DomainDnsRecord используется** для представить такие записи DNS.</span><span class="sxs-lookup"><span data-stu-id="b1098-106">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="b1098-107">Базовый объект для сущностей [DomainDnsCnameRecord,](domaindnscnamerecord.md) [DomainDnsMxRecord,](domaindnsmxrecord.md) [DomainDnsSrvRecord](domaindnssrvrecord.md) и [DomainDnsTxtRecord.](domaindnstxtrecord.md)</span><span class="sxs-lookup"><span data-stu-id="b1098-107">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="b1098-108">Methods</span><span class="sxs-lookup"><span data-stu-id="b1098-108">Methods</span></span>
<span data-ttu-id="b1098-109">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="b1098-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="b1098-110">Сведения о [том,](domain.md) как запрашивать записи доменной службы, см. в разделе "Домен".</span><span class="sxs-lookup"><span data-stu-id="b1098-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="b1098-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1098-111">Properties</span></span>
| <span data-ttu-id="b1098-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1098-112">Property</span></span>     | <span data-ttu-id="b1098-113">Тип</span><span class="sxs-lookup"><span data-stu-id="b1098-113">Type</span></span>   |<span data-ttu-id="b1098-114">Описание</span><span class="sxs-lookup"><span data-stu-id="b1098-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1098-115">id</span><span class="sxs-lookup"><span data-stu-id="b1098-115">id</span></span>|<span data-ttu-id="b1098-116">String</span><span class="sxs-lookup"><span data-stu-id="b1098-116">String</span></span>| <span data-ttu-id="b1098-117">Уникальный идентификатор, присвоенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="b1098-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="b1098-118">Не имеет null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b1098-118">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="b1098-119">isOptional</span><span class="sxs-lookup"><span data-stu-id="b1098-119">isOptional</span></span>|<span data-ttu-id="b1098-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1098-120">Boolean</span></span>| <span data-ttu-id="b1098-121">Если установлено false, эта запись должна быть настроена клиентом на DNS-Microsoft Online Services для правильной работы с доменом.</span><span class="sxs-lookup"><span data-stu-id="b1098-121">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="b1098-122">label</span><span class="sxs-lookup"><span data-stu-id="b1098-122">label</span></span>|<span data-ttu-id="b1098-123">String</span><span class="sxs-lookup"><span data-stu-id="b1098-123">String</span></span>| <span data-ttu-id="b1098-124">Значение, используемого при настройке имени DNS-записи на DNS-хосте.</span><span class="sxs-lookup"><span data-stu-id="b1098-124">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="b1098-125">recordType</span><span class="sxs-lookup"><span data-stu-id="b1098-125">recordType</span></span>|<span data-ttu-id="b1098-126">String</span><span class="sxs-lookup"><span data-stu-id="b1098-126">String</span></span>| <span data-ttu-id="b1098-127">Указывает, какой тип DNS-записи представляет этот объект.</span><span class="sxs-lookup"><span data-stu-id="b1098-127">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="b1098-128">Может иметь одно из следующих значений: *CName,* *Mx,* *Srv,* *Txt*</span><span class="sxs-lookup"><span data-stu-id="b1098-128">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="b1098-129">Key</span><span class="sxs-lookup"><span data-stu-id="b1098-129">Key</span></span> |
|<span data-ttu-id="b1098-130">supportedService</span><span class="sxs-lookup"><span data-stu-id="b1098-130">supportedService</span></span>|<span data-ttu-id="b1098-131">String</span><span class="sxs-lookup"><span data-stu-id="b1098-131">String</span></span>| <span data-ttu-id="b1098-132">Microsoft Online Service или функция, которая зависит от этой записи DNS.</span><span class="sxs-lookup"><span data-stu-id="b1098-132">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="b1098-133">Может иметь одно из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="b1098-133">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="b1098-134">ttl</span><span class="sxs-lookup"><span data-stu-id="b1098-134">ttl</span></span>|<span data-ttu-id="b1098-135">Int32</span><span class="sxs-lookup"><span data-stu-id="b1098-135">Int32</span></span>| <span data-ttu-id="b1098-136">Значение, используемого при настройке свойства времени жизни (ttl) записи DNS на DNS-хосте.</span><span class="sxs-lookup"><span data-stu-id="b1098-136">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="b1098-137">Не nullable</span><span class="sxs-lookup"><span data-stu-id="b1098-137">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="b1098-138">Связи</span><span class="sxs-lookup"><span data-stu-id="b1098-138">Relationships</span></span>
<span data-ttu-id="b1098-139">Нет</span><span class="sxs-lookup"><span data-stu-id="b1098-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1098-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1098-140">JSON representation</span></span>
<span data-ttu-id="b1098-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1098-141">Here is a JSON representation of the resource.</span></span>

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

