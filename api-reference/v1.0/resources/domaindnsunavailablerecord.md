---
title: Тип ресурса domainDnsUnavailableRecord
description: При запросе свойство навигации **serviceConfigurationRecords** для сущности домена, может получать один или несколько DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord или DomainDnsTxtRecord сущности. Эти сущности указывает, какие записи DNS, необходимо добавить в файл зоны домена, прежде чем домена можно использовать с Microsoft Online Services. Когда не возможно для создания таких сущностей, возвращается DomainDnsUnavailableRecord сущности. Наследуется от DomainDnsRecord сущности.
localization_priority: Normal
ms.openlocfilehash: 064fd294a89b48f6b7cfba58fa3d1076bf74a7ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836185"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="9b45d-106">Тип ресурса domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="9b45d-106">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="9b45d-p102">Когда вы запрашиваете объект [Domain](domain.md) в свойстве навигации **serviceConfigurationRecords**, то может быть возвращен один или несколько объектов [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) или [DomainDnsTxtRecord](domaindnstxtrecord.md). Эти объекты указывают, какие записи DNS необходимо добавить в файл зоны домена, чтобы службы Microsoft Online Services могли использовать этот домен. Если не удается создать такие объекты, то вместо них будет возвращен объект DomainDnsUnavailableRecord. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="9b45d-p102">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="9b45d-111">Методы</span><span class="sxs-lookup"><span data-stu-id="9b45d-111">Methods</span></span>
<span data-ttu-id="9b45d-p103">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="9b45d-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="9b45d-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b45d-114">Properties</span></span>
| <span data-ttu-id="9b45d-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b45d-115">Property</span></span>     | <span data-ttu-id="9b45d-116">Тип</span><span class="sxs-lookup"><span data-stu-id="9b45d-116">Type</span></span>   |<span data-ttu-id="9b45d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="9b45d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b45d-118">описание</span><span class="sxs-lookup"><span data-stu-id="9b45d-118">description</span></span>|<span data-ttu-id="9b45d-119">String</span><span class="sxs-lookup"><span data-stu-id="9b45d-119">String</span></span>|<span data-ttu-id="9b45d-120">Указывает причину, по которой возвращен объект **DomainDnsUnavailableRecord**.</span><span class="sxs-lookup"><span data-stu-id="9b45d-120">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9b45d-121">Связи</span><span class="sxs-lookup"><span data-stu-id="9b45d-121">Relationships</span></span>
<span data-ttu-id="9b45d-122">Нет</span><span class="sxs-lookup"><span data-stu-id="9b45d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b45d-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b45d-123">JSON representation</span></span>
<span data-ttu-id="9b45d-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b45d-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "description": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
