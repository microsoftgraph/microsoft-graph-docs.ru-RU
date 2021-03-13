---
title: тип ресурса domainDnsUnavailableRecord
description: Указывает, что службыConfigurationRecords не могут быть созданы.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6cb35152b6d31e313342f7bfea99bfc98c51635b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761376"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="bbb03-103">тип ресурса domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="bbb03-103">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="bbb03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbb03-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bbb03-105">При запросе службы свойств навигацииConfigurationRecords для объекта домена вы можете получить обратно одно или несколько объектов [DomainDnsCnameRecord,](domaindnscnamerecord.md) [DomainDnsMxRecord,](domaindnsmxrecord.md) [DomainDnsSrvRecord](domaindnssrvrecord.md)и/или  [](domain.md) [объекты DomainDnsTxtRecord.](domaindnstxtrecord.md)</span><span class="sxs-lookup"><span data-stu-id="bbb03-105">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="bbb03-106">Эти сущности указывают, какие записи DNS необходимо добавить в файл зоны домена, прежде чем домен может использоваться Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="bbb03-106">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="bbb03-107">Если создание таких сущностей невозможно, возвращается объект DomainDnsUnavailableRecord.</span><span class="sxs-lookup"><span data-stu-id="bbb03-107">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="bbb03-108">Наследуется от [объекта DomainDnsRecord.](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="bbb03-108">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="bbb03-109">Методы</span><span class="sxs-lookup"><span data-stu-id="bbb03-109">Methods</span></span>
<span data-ttu-id="bbb03-110">Прямые запросы на этот ресурс не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="bbb03-110">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="bbb03-111">Сведения о [том,](domain.md) как запрашивать записи службы домена, см. в разделе домен.</span><span class="sxs-lookup"><span data-stu-id="bbb03-111">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="bbb03-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbb03-112">Properties</span></span>
| <span data-ttu-id="bbb03-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbb03-113">Property</span></span>     | <span data-ttu-id="bbb03-114">Тип</span><span class="sxs-lookup"><span data-stu-id="bbb03-114">Type</span></span>   |<span data-ttu-id="bbb03-115">Описание</span><span class="sxs-lookup"><span data-stu-id="bbb03-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbb03-116">description</span><span class="sxs-lookup"><span data-stu-id="bbb03-116">description</span></span>|<span data-ttu-id="bbb03-117">String</span><span class="sxs-lookup"><span data-stu-id="bbb03-117">String</span></span>|<span data-ttu-id="bbb03-118">Предоставляет причину, по которой **возвращается объект DomainDnsUnavailableRecord.**</span><span class="sxs-lookup"><span data-stu-id="bbb03-118">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bbb03-119">Связи</span><span class="sxs-lookup"><span data-stu-id="bbb03-119">Relationships</span></span>
<span data-ttu-id="bbb03-120">Нет</span><span class="sxs-lookup"><span data-stu-id="bbb03-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbb03-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbb03-121">JSON representation</span></span>
<span data-ttu-id="bbb03-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbb03-122">Here is a JSON representation of the resource.</span></span>

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

