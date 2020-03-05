---
title: Тип ресурса domainDnsUnavailableRecord
description: Когда вы запрашиваете свойство навигации **serviceConfigurationRecords** для объекта Domain, вы можете получить одну или несколько сущностей Домаинднскнамерекорд, Домаинднсмксрекорд, домаинднссрврекорд и/или домаинднсткстрекорд. Эти сущности указывают, какие записи DNS необходимо добавить в файл зоны домена, прежде чем домен можно будет использовать в Microsoft Online Services. Если невозможно создать такие сущности, возвращается сущность DomainDnsUnavailableRecord. Наследуется от объекта DomainDnsRecord.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9743d1f9a4db1018f1b704b45b8236aeda6d5cd9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505814"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="de5f1-106">Тип ресурса domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="de5f1-106">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="de5f1-107">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="de5f1-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de5f1-108">Когда вы запрашиваете свойство навигации **serviceConfigurationRecords** для объекта [domain](domain.md) , вы можете получить одну или несколько сущностей [домаинднскнамерекорд](domaindnscnamerecord.md), [домаинднсмксрекорд](domaindnsmxrecord.md), [домаинднссрврекорд](domaindnssrvrecord.md)и/или [домаинднсткстрекорд](domaindnstxtrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="de5f1-108">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="de5f1-109">Эти сущности указывают, какие записи DNS необходимо добавить в файл зоны домена, прежде чем домен можно будет использовать в Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="de5f1-109">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="de5f1-110">Если невозможно создать такие сущности, возвращается сущность DomainDnsUnavailableRecord.</span><span class="sxs-lookup"><span data-stu-id="de5f1-110">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="de5f1-111">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="de5f1-111">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="de5f1-112">Методы</span><span class="sxs-lookup"><span data-stu-id="de5f1-112">Methods</span></span>
<span data-ttu-id="de5f1-113">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="de5f1-113">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="de5f1-114">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="de5f1-114">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="de5f1-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="de5f1-115">Properties</span></span>
| <span data-ttu-id="de5f1-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="de5f1-116">Property</span></span>     | <span data-ttu-id="de5f1-117">Тип</span><span class="sxs-lookup"><span data-stu-id="de5f1-117">Type</span></span>   |<span data-ttu-id="de5f1-118">Описание</span><span class="sxs-lookup"><span data-stu-id="de5f1-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de5f1-119">description</span><span class="sxs-lookup"><span data-stu-id="de5f1-119">description</span></span>|<span data-ttu-id="de5f1-120">String</span><span class="sxs-lookup"><span data-stu-id="de5f1-120">String</span></span>|<span data-ttu-id="de5f1-121">Предоставляет причину, по которой возвращается объект **DomainDnsUnavailableRecord** .</span><span class="sxs-lookup"><span data-stu-id="de5f1-121">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="de5f1-122">Связи</span><span class="sxs-lookup"><span data-stu-id="de5f1-122">Relationships</span></span>
<span data-ttu-id="de5f1-123">Нет</span><span class="sxs-lookup"><span data-stu-id="de5f1-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de5f1-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de5f1-124">JSON representation</span></span>
<span data-ttu-id="de5f1-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de5f1-125">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
