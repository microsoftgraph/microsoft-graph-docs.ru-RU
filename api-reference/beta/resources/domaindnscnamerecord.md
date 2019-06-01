---
title: Тип ресурса Домаинднскнамерекорд
description: Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4de771a543459ffa1529cb2a6bb11e480d645e43
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657849"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="2d6e1-104">Тип ресурса Домаинднскнамерекорд</span><span class="sxs-lookup"><span data-stu-id="2d6e1-104">domainDnsCnameRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d6e1-105">Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2d6e1-105">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="2d6e1-106">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="2d6e1-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="2d6e1-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2d6e1-107">Methods</span></span>
<span data-ttu-id="2d6e1-108">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="2d6e1-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="2d6e1-109">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="2d6e1-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="2d6e1-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d6e1-110">Properties</span></span>
| <span data-ttu-id="2d6e1-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d6e1-111">Property</span></span>     | <span data-ttu-id="2d6e1-112">Тип</span><span class="sxs-lookup"><span data-stu-id="2d6e1-112">Type</span></span>   |<span data-ttu-id="2d6e1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="2d6e1-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d6e1-114">Каноникалнаме</span><span class="sxs-lookup"><span data-stu-id="2d6e1-114">canonicalName</span></span>|<span data-ttu-id="2d6e1-115">String</span><span class="sxs-lookup"><span data-stu-id="2d6e1-115">String</span></span>| <span data-ttu-id="2d6e1-116">Каноническое имя записи CNAME.</span><span class="sxs-lookup"><span data-stu-id="2d6e1-116">The canonical name of the CNAME record.</span></span> <span data-ttu-id="2d6e1-117">Используется для настройки записи CNAME на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="2d6e1-117">Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="2d6e1-118">id</span><span class="sxs-lookup"><span data-stu-id="2d6e1-118">id</span></span>|<span data-ttu-id="2d6e1-119">String</span><span class="sxs-lookup"><span data-stu-id="2d6e1-119">String</span></span>| <span data-ttu-id="2d6e1-120">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="2d6e1-120">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="2d6e1-121">Не допускает значение null, доступно только для чтения</span><span class="sxs-lookup"><span data-stu-id="2d6e1-121">Not nullable, Read-only</span></span>|
|<span data-ttu-id="2d6e1-122">Переключатель</span><span class="sxs-lookup"><span data-stu-id="2d6e1-122">isOptional</span></span>|<span data-ttu-id="2d6e1-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d6e1-123">Boolean</span></span>| <span data-ttu-id="2d6e1-124">Если значение равно false, запись CNAME должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="2d6e1-124">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> <span data-ttu-id="2d6e1-125">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="2d6e1-125">Not nullable</span></span> |
|<span data-ttu-id="2d6e1-126">label</span><span class="sxs-lookup"><span data-stu-id="2d6e1-126">label</span></span>|<span data-ttu-id="2d6e1-127">String</span><span class="sxs-lookup"><span data-stu-id="2d6e1-127">String</span></span>| <span data-ttu-id="2d6e1-128">Значение, используемое при настройке *псевдонима/узла или имени* записи CNAME на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="2d6e1-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="2d6e1-129">recordType</span><span class="sxs-lookup"><span data-stu-id="2d6e1-129">recordType</span></span>|<span data-ttu-id="2d6e1-130">String</span><span class="sxs-lookup"><span data-stu-id="2d6e1-130">String</span></span>| <span data-ttu-id="2d6e1-131">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="2d6e1-131">Type of DNS record.</span></span> <span data-ttu-id="2d6e1-132">Значение всегда равно *CNAME*.</span><span class="sxs-lookup"><span data-stu-id="2d6e1-132">The value is always *CName*.</span></span> <span data-ttu-id="2d6e1-133">Key</span><span class="sxs-lookup"><span data-stu-id="2d6e1-133">Key</span></span>|
|<span data-ttu-id="2d6e1-134">Суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="2d6e1-134">supportedService</span></span>|<span data-ttu-id="2d6e1-135">String</span><span class="sxs-lookup"><span data-stu-id="2d6e1-135">String</span></span>| <span data-ttu-id="2d6e1-136">Служба или компонент Microsoft Online, который имеет зависимость от этой записи CNAME.</span><span class="sxs-lookup"><span data-stu-id="2d6e1-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="2d6e1-137">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, \*SharePointPublic \*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="2d6e1-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="2d6e1-138">используем</span><span class="sxs-lookup"><span data-stu-id="2d6e1-138">ttl</span></span>|<span data-ttu-id="2d6e1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2d6e1-139">Int32</span></span>| <span data-ttu-id="2d6e1-140">Значение, используемое при настройке свойства срока жизни (TTL) записи CNAME на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="2d6e1-140">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host.</span></span> <span data-ttu-id="2d6e1-141">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="2d6e1-141">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="2d6e1-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="2d6e1-142">Relationships</span></span>
<span data-ttu-id="2d6e1-143">Нет</span><span class="sxs-lookup"><span data-stu-id="2d6e1-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2d6e1-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d6e1-144">JSON representation</span></span>
<span data-ttu-id="2d6e1-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d6e1-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
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
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
