---
title: Тип ресурса domainDnsUnavailableRecord
description: Указывает, что serviceConfigurationRecords не может быть создан.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3f9c8010b0e07a16d2a982c3ddbc7ef40c614583
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181759"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="dcc0f-103">Тип ресурса domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="dcc0f-103">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="dcc0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcc0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcc0f-105">Когда вы запрашиваете свойство навигации **serviceConfigurationRecords** для объекта [domain](domain.md) , вы можете получить одну или несколько сущностей [домаинднскнамерекорд](domaindnscnamerecord.md), [домаинднсмксрекорд](domaindnsmxrecord.md), [домаинднссрврекорд](domaindnssrvrecord.md)и/или [домаинднсткстрекорд](domaindnstxtrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="dcc0f-105">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="dcc0f-106">Эти сущности указывают, какие записи DNS необходимо добавить в файл зоны домена, прежде чем домен можно будет использовать в Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="dcc0f-106">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="dcc0f-107">Если невозможно создать такие сущности, возвращается сущность DomainDnsUnavailableRecord.</span><span class="sxs-lookup"><span data-stu-id="dcc0f-107">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="dcc0f-108">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="dcc0f-108">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="dcc0f-109">Methods</span><span class="sxs-lookup"><span data-stu-id="dcc0f-109">Methods</span></span>
<span data-ttu-id="dcc0f-110">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="dcc0f-110">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="dcc0f-111">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="dcc0f-111">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="dcc0f-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="dcc0f-112">Properties</span></span>
| <span data-ttu-id="dcc0f-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="dcc0f-113">Property</span></span>     | <span data-ttu-id="dcc0f-114">Тип</span><span class="sxs-lookup"><span data-stu-id="dcc0f-114">Type</span></span>   |<span data-ttu-id="dcc0f-115">Описание</span><span class="sxs-lookup"><span data-stu-id="dcc0f-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dcc0f-116">description</span><span class="sxs-lookup"><span data-stu-id="dcc0f-116">description</span></span>|<span data-ttu-id="dcc0f-117">String</span><span class="sxs-lookup"><span data-stu-id="dcc0f-117">String</span></span>|<span data-ttu-id="dcc0f-118">Предоставляет причину, по которой возвращается объект **DomainDnsUnavailableRecord** .</span><span class="sxs-lookup"><span data-stu-id="dcc0f-118">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dcc0f-119">Связи</span><span class="sxs-lookup"><span data-stu-id="dcc0f-119">Relationships</span></span>
<span data-ttu-id="dcc0f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="dcc0f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcc0f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dcc0f-121">JSON representation</span></span>
<span data-ttu-id="dcc0f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcc0f-122">Here is a JSON representation of the resource.</span></span>

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
