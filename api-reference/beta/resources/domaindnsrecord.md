---
title: Тип ресурса domainDnsRecord
description: Для работы служб Microsoft Online Services с доменом необходимо добавить записи DNS в файл зоны DNS домена. Объект **DomainDnsRecord** представляет такие записи DNS. Базовый объект для объектов DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord и DomainDnsSrvRecord.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b7b04e65da67bc61e3f3b91ed3dae7cba70a3d27
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519285"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="4a052-105">Тип ресурса domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="4a052-105">domainDnsRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a052-p102">Для работы служб Microsoft Online Services с доменом необходимо добавить записи DNS в файл зоны DNS домена. Объект **DomainDnsRecord** представляет такие записи DNS. Базовый объект для объектов [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) и [DomainDnsSrvRecord](domaindnssrvrecord.md).</span><span class="sxs-lookup"><span data-stu-id="4a052-p102">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services. The **DomainDnsRecord** entity is used to present such DNS records. Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="4a052-109">Методы</span><span class="sxs-lookup"><span data-stu-id="4a052-109">Methods</span></span>
<span data-ttu-id="4a052-p103">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="4a052-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="4a052-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a052-112">Properties</span></span>
| <span data-ttu-id="4a052-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a052-113">Property</span></span>     | <span data-ttu-id="4a052-114">Тип</span><span class="sxs-lookup"><span data-stu-id="4a052-114">Type</span></span>   |<span data-ttu-id="4a052-115">Описание</span><span class="sxs-lookup"><span data-stu-id="4a052-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a052-116">id</span><span class="sxs-lookup"><span data-stu-id="4a052-116">id</span></span>|<span data-ttu-id="4a052-117">String</span><span class="sxs-lookup"><span data-stu-id="4a052-117">String</span></span>| <span data-ttu-id="4a052-p104">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a052-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="4a052-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="4a052-120">isOptional</span></span>|<span data-ttu-id="4a052-121">Логический</span><span class="sxs-lookup"><span data-stu-id="4a052-121">Boolean</span></span>| <span data-ttu-id="4a052-122">Если указано значение false, для правильной работы служб Microsoft Online Services с доменом клиент должен настроить эту запись на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="4a052-122">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="4a052-123">label</span><span class="sxs-lookup"><span data-stu-id="4a052-123">label</span></span>|<span data-ttu-id="4a052-124">String</span><span class="sxs-lookup"><span data-stu-id="4a052-124">String</span></span>| <span data-ttu-id="4a052-125">Значение, используемое при настройке имени записи DNS на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="4a052-125">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="4a052-126">recordType</span><span class="sxs-lookup"><span data-stu-id="4a052-126">recordType</span></span>|<span data-ttu-id="4a052-127">String</span><span class="sxs-lookup"><span data-stu-id="4a052-127">String</span></span>| <span data-ttu-id="4a052-128">Указывает, какой тип записи DNS представляет этот объект.</span><span class="sxs-lookup"><span data-stu-id="4a052-128">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="4a052-129">Возможные значения: *CName*, *Mx*, *Srv*, *Txt*.</span><span class="sxs-lookup"><span data-stu-id="4a052-129">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="4a052-130">Ключ</span><span class="sxs-lookup"><span data-stu-id="4a052-130">Key</span></span> |
|<span data-ttu-id="4a052-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="4a052-131">supportedService</span></span>|<span data-ttu-id="4a052-132">Строка</span><span class="sxs-lookup"><span data-stu-id="4a052-132">String</span></span>| <span data-ttu-id="4a052-133">Веб-служба или функция Майкрософт, зависящая от этой записи DNS.</span><span class="sxs-lookup"><span data-stu-id="4a052-133">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="4a052-134">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="4a052-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="4a052-135">ttl</span><span class="sxs-lookup"><span data-stu-id="4a052-135">ttl</span></span>|<span data-ttu-id="4a052-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4a052-136">Int32</span></span>| <span data-ttu-id="4a052-p105">Значение, используемое при настройке свойства срока жизни (ttl) записи DNS на узле DNS. Не допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="4a052-p105">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="4a052-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="4a052-139">Relationships</span></span>
<span data-ttu-id="4a052-140">Нет</span><span class="sxs-lookup"><span data-stu-id="4a052-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a052-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a052-141">JSON representation</span></span>
<span data-ttu-id="4a052-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a052-142">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnsrecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
