---
title: Тип ресурса domainDnsUnavailableRecord
description: При запросе свойство навигации **serviceConfigurationRecords** для сущности домена, может получать один или несколько DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord или DomainDnsTxtRecord сущности. Эти сущности указывает, какие записи DNS, необходимо добавить в файл зоны домена, прежде чем домена можно использовать с Microsoft Online Services. Когда не возможно для создания таких сущностей, возвращается DomainDnsUnavailableRecord сущности. Наследуется от DomainDnsRecord сущности.
localization_priority: Normal
ms.openlocfilehash: 3b23eab8f4efe1d23d3a179384dbab6e9c7e7773
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873425"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="1ddf2-106">Тип ресурса domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="1ddf2-106">domainDnsUnavailableRecord resource type</span></span>

> <span data-ttu-id="1ddf2-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1ddf2-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ddf2-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ddf2-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1ddf2-p103">Когда вы запрашиваете объект [Domain](domain.md) в свойстве навигации **serviceConfigurationRecords**, то может быть возвращен один или несколько объектов [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) или [DomainDnsTxtRecord](domaindnstxtrecord.md). Эти объекты указывают, какие записи DNS необходимо добавить в файл зоны домена, чтобы службы Microsoft Online Services могли использовать этот домен. Если не удается создать такие объекты, то вместо них будет возвращен объект DomainDnsUnavailableRecord. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="1ddf2-p103">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="1ddf2-113">Методы</span><span class="sxs-lookup"><span data-stu-id="1ddf2-113">Methods</span></span>
<span data-ttu-id="1ddf2-p104">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="1ddf2-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="1ddf2-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ddf2-116">Properties</span></span>
| <span data-ttu-id="1ddf2-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ddf2-117">Property</span></span>     | <span data-ttu-id="1ddf2-118">Тип</span><span class="sxs-lookup"><span data-stu-id="1ddf2-118">Type</span></span>   |<span data-ttu-id="1ddf2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1ddf2-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ddf2-120">описание</span><span class="sxs-lookup"><span data-stu-id="1ddf2-120">description</span></span>|<span data-ttu-id="1ddf2-121">String</span><span class="sxs-lookup"><span data-stu-id="1ddf2-121">String</span></span>|<span data-ttu-id="1ddf2-122">Указывает причину, по которой возвращен объект **DomainDnsUnavailableRecord**.</span><span class="sxs-lookup"><span data-stu-id="1ddf2-122">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1ddf2-123">Связи</span><span class="sxs-lookup"><span data-stu-id="1ddf2-123">Relationships</span></span>
<span data-ttu-id="1ddf2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="1ddf2-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ddf2-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ddf2-125">JSON representation</span></span>
<span data-ttu-id="1ddf2-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ddf2-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
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
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
