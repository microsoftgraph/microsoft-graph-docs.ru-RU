---
title: Тип ресурса domainDnsRecord
description: Объект DomainDnsRecord используется для представления записей DNS.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6e2b64a15f49e31384045adcfe85758af06e1e92
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181646"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="b7ced-103">Тип ресурса domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="b7ced-103">domainDnsRecord resource type</span></span>

<span data-ttu-id="b7ced-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7ced-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b7ced-105">Для каждого домена в клиенте может потребоваться добавить записи DNS в файл зоны DNS домена, чтобы домен можно было использовать в Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="b7ced-105">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="b7ced-106">Объект **DomainDnsRecord** используется для представления таких DNS-записей.</span><span class="sxs-lookup"><span data-stu-id="b7ced-106">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="b7ced-107">Базовый объект для сущностей [домаинднскнамерекорд](domaindnscnamerecord.md), [домаинднсмксрекорд](domaindnsmxrecord.md), [домаинднссрврекорд](domaindnssrvrecord.md) и [домаинднсткстрекорд](domaindnstxtrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="b7ced-107">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="b7ced-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b7ced-108">Methods</span></span>
<span data-ttu-id="b7ced-109">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="b7ced-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="b7ced-110">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="b7ced-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="b7ced-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7ced-111">Properties</span></span>
| <span data-ttu-id="b7ced-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7ced-112">Property</span></span>     | <span data-ttu-id="b7ced-113">Тип</span><span class="sxs-lookup"><span data-stu-id="b7ced-113">Type</span></span>   |<span data-ttu-id="b7ced-114">Описание</span><span class="sxs-lookup"><span data-stu-id="b7ced-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7ced-115">id</span><span class="sxs-lookup"><span data-stu-id="b7ced-115">id</span></span>|<span data-ttu-id="b7ced-116">String</span><span class="sxs-lookup"><span data-stu-id="b7ced-116">String</span></span>| <span data-ttu-id="b7ced-117">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="b7ced-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="b7ced-118">Не допускает значения NULL и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b7ced-118">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="b7ced-119">Переключатель</span><span class="sxs-lookup"><span data-stu-id="b7ced-119">isOptional</span></span>|<span data-ttu-id="b7ced-120">Логический</span><span class="sxs-lookup"><span data-stu-id="b7ced-120">Boolean</span></span>| <span data-ttu-id="b7ced-121">Если задано значение false, эта запись должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="b7ced-121">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="b7ced-122">label</span><span class="sxs-lookup"><span data-stu-id="b7ced-122">label</span></span>|<span data-ttu-id="b7ced-123">String</span><span class="sxs-lookup"><span data-stu-id="b7ced-123">String</span></span>| <span data-ttu-id="b7ced-124">Значение, используемое при настройке имени DNS-записи на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="b7ced-124">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="b7ced-125">recordType</span><span class="sxs-lookup"><span data-stu-id="b7ced-125">recordType</span></span>|<span data-ttu-id="b7ced-126">String</span><span class="sxs-lookup"><span data-stu-id="b7ced-126">String</span></span>| <span data-ttu-id="b7ced-127">Указывает, какой тип записи DNS представляет эта сущность.</span><span class="sxs-lookup"><span data-stu-id="b7ced-127">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="b7ced-128">Может принимать одно из следующих значений: *CNAME*, *MX*, *SRV*, *txt* .</span><span class="sxs-lookup"><span data-stu-id="b7ced-128">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="b7ced-129">Key</span><span class="sxs-lookup"><span data-stu-id="b7ced-129">Key</span></span> |
|<span data-ttu-id="b7ced-130">суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="b7ced-130">supportedService</span></span>|<span data-ttu-id="b7ced-131">String</span><span class="sxs-lookup"><span data-stu-id="b7ced-131">String</span></span>| <span data-ttu-id="b7ced-132">Служба или компонент Microsoft Online, зависящие от этой записи DNS.</span><span class="sxs-lookup"><span data-stu-id="b7ced-132">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="b7ced-133">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="b7ced-133">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="b7ced-134">используем</span><span class="sxs-lookup"><span data-stu-id="b7ced-134">ttl</span></span>|<span data-ttu-id="b7ced-135">Int32</span><span class="sxs-lookup"><span data-stu-id="b7ced-135">Int32</span></span>| <span data-ttu-id="b7ced-136">Значение, используемое при настройке свойства срока жизни (TTL) записи DNS на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="b7ced-136">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="b7ced-137">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="b7ced-137">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="b7ced-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="b7ced-138">Relationships</span></span>
<span data-ttu-id="b7ced-139">Нет</span><span class="sxs-lookup"><span data-stu-id="b7ced-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7ced-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7ced-140">JSON representation</span></span>
<span data-ttu-id="b7ced-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7ced-141">Here is a JSON representation of the resource.</span></span>

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
