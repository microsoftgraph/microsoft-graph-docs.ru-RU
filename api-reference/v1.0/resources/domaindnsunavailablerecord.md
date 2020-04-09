---
title: Тип ресурса domainDnsUnavailableRecord
description: Указывает, что serviceConfigurationRecords не может быть создан.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 67871266e6a51101ea6ad718ab9959b6daff2a1d
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181625"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="c3e82-103">Тип ресурса domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="c3e82-103">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="c3e82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3e82-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3e82-105">Когда вы запрашиваете свойство навигации **serviceConfigurationRecords** для объекта [domain](domain.md) , вы можете получить одну или несколько сущностей [домаинднскнамерекорд](domaindnscnamerecord.md), [домаинднсмксрекорд](domaindnsmxrecord.md), [домаинднссрврекорд](domaindnssrvrecord.md)и/или [домаинднсткстрекорд](domaindnstxtrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="c3e82-105">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="c3e82-106">Эти сущности указывают, какие записи DNS необходимо добавить в файл зоны домена, прежде чем домен можно будет использовать в Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="c3e82-106">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="c3e82-107">Если невозможно создать такие сущности, возвращается сущность DomainDnsUnavailableRecord.</span><span class="sxs-lookup"><span data-stu-id="c3e82-107">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="c3e82-108">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="c3e82-108">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="c3e82-109">Методы</span><span class="sxs-lookup"><span data-stu-id="c3e82-109">Methods</span></span>
<span data-ttu-id="c3e82-110">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="c3e82-110">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="c3e82-111">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="c3e82-111">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="c3e82-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3e82-112">Properties</span></span>
| <span data-ttu-id="c3e82-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3e82-113">Property</span></span>     | <span data-ttu-id="c3e82-114">Тип</span><span class="sxs-lookup"><span data-stu-id="c3e82-114">Type</span></span>   |<span data-ttu-id="c3e82-115">Описание</span><span class="sxs-lookup"><span data-stu-id="c3e82-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3e82-116">description</span><span class="sxs-lookup"><span data-stu-id="c3e82-116">description</span></span>|<span data-ttu-id="c3e82-117">String</span><span class="sxs-lookup"><span data-stu-id="c3e82-117">String</span></span>|<span data-ttu-id="c3e82-118">Предоставляет причину, по которой возвращается объект **DomainDnsUnavailableRecord** .</span><span class="sxs-lookup"><span data-stu-id="c3e82-118">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c3e82-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="c3e82-119">Relationships</span></span>
<span data-ttu-id="c3e82-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c3e82-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3e82-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3e82-121">JSON representation</span></span>
<span data-ttu-id="c3e82-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3e82-122">Here is a JSON representation of the resource.</span></span>

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
