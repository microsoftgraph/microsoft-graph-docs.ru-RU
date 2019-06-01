---
title: Тип ресурса domainDnsUnavailableRecord
description: Когда вы запрашиваете свойство навигации **serviceConfigurationRecords** для объекта Domain, вы можете получить одну или несколько сущностей Домаинднскнамерекорд, Домаинднсмксрекорд, домаинднссрврекорд и/или домаинднсткстрекорд. Эти сущности указывают, какие записи DNS необходимо добавить в файл зоны домена, прежде чем домен можно будет использовать в Microsoft Online Services. Если невозможно создать такие сущности, возвращается сущность DomainDnsUnavailableRecord. Наследуется от объекта DomainDnsRecord.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6ebe73224936d456c4f860e7cf2ea7e1b689a11e
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34658059"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="4a982-106">Тип ресурса domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="4a982-106">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="4a982-107">Когда вы запрашиваете свойство навигации **serviceConfigurationRecords** для объекта [domain](domain.md) , вы можете получить один или несколько [домаинднскнамерекорд](domaindnscnamerecord.md), [домаинднсмксрекорд](domaindnsmxrecord.md), [домаинднссрврекорд](domaindnssrvrecord.md)и/или [ Сущности Домаинднсткстрекорд](domaindnstxtrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="4a982-107">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="4a982-108">Эти сущности указывают, какие записи DNS необходимо добавить в файл зоны домена, прежде чем домен можно будет использовать в Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="4a982-108">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="4a982-109">Если невозможно создать такие сущности, возвращается сущность DomainDnsUnavailableRecord.</span><span class="sxs-lookup"><span data-stu-id="4a982-109">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="4a982-110">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="4a982-110">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="4a982-111">Методы</span><span class="sxs-lookup"><span data-stu-id="4a982-111">Methods</span></span>
<span data-ttu-id="4a982-112">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="4a982-112">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="4a982-113">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="4a982-113">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="4a982-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a982-114">Properties</span></span>
| <span data-ttu-id="4a982-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a982-115">Property</span></span>     | <span data-ttu-id="4a982-116">Тип</span><span class="sxs-lookup"><span data-stu-id="4a982-116">Type</span></span>   |<span data-ttu-id="4a982-117">Описание</span><span class="sxs-lookup"><span data-stu-id="4a982-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a982-118">description</span><span class="sxs-lookup"><span data-stu-id="4a982-118">description</span></span>|<span data-ttu-id="4a982-119">String</span><span class="sxs-lookup"><span data-stu-id="4a982-119">String</span></span>|<span data-ttu-id="4a982-120">Предоставляет причину, по которой возвращается объект **DomainDnsUnavailableRecord** .</span><span class="sxs-lookup"><span data-stu-id="4a982-120">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4a982-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="4a982-121">Relationships</span></span>
<span data-ttu-id="4a982-122">Нет</span><span class="sxs-lookup"><span data-stu-id="4a982-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a982-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a982-123">JSON representation</span></span>
<span data-ttu-id="4a982-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a982-124">Here is a JSON representation of the resource.</span></span>

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
