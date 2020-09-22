---
title: Тип ресурса Домаинднскнамерекорд
description: Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5dc5c70952f24463c0b483a290d41823f8904576
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095592"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="bb78d-103">Тип ресурса Домаинднскнамерекорд</span><span class="sxs-lookup"><span data-stu-id="bb78d-103">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="bb78d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb78d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb78d-105">Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="bb78d-105">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="bb78d-106">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="bb78d-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="bb78d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bb78d-107">Methods</span></span>
<span data-ttu-id="bb78d-108">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="bb78d-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="bb78d-109">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="bb78d-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="bb78d-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb78d-110">Properties</span></span>
| <span data-ttu-id="bb78d-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb78d-111">Property</span></span>     | <span data-ttu-id="bb78d-112">Тип</span><span class="sxs-lookup"><span data-stu-id="bb78d-112">Type</span></span>   |<span data-ttu-id="bb78d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="bb78d-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb78d-114">каноникалнаме</span><span class="sxs-lookup"><span data-stu-id="bb78d-114">canonicalName</span></span>|<span data-ttu-id="bb78d-115">Строка</span><span class="sxs-lookup"><span data-stu-id="bb78d-115">String</span></span>| <span data-ttu-id="bb78d-116">Каноническое имя записи CNAME.</span><span class="sxs-lookup"><span data-stu-id="bb78d-116">The canonical name of the CNAME record.</span></span> <span data-ttu-id="bb78d-117">Используется для настройки записи CNAME на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="bb78d-117">Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="bb78d-118">id</span><span class="sxs-lookup"><span data-stu-id="bb78d-118">id</span></span>|<span data-ttu-id="bb78d-119">Строка</span><span class="sxs-lookup"><span data-stu-id="bb78d-119">String</span></span>| <span data-ttu-id="bb78d-120">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="bb78d-120">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="bb78d-121">Не допускает значение null, доступно только для чтения</span><span class="sxs-lookup"><span data-stu-id="bb78d-121">Not nullable, Read-only</span></span>|
|<span data-ttu-id="bb78d-122">Переключатель</span><span class="sxs-lookup"><span data-stu-id="bb78d-122">isOptional</span></span>|<span data-ttu-id="bb78d-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb78d-123">Boolean</span></span>| <span data-ttu-id="bb78d-124">Если значение равно false, запись CNAME должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="bb78d-124">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> <span data-ttu-id="bb78d-125">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="bb78d-125">Not nullable</span></span> |
|<span data-ttu-id="bb78d-126">label</span><span class="sxs-lookup"><span data-stu-id="bb78d-126">label</span></span>|<span data-ttu-id="bb78d-127">Строка</span><span class="sxs-lookup"><span data-stu-id="bb78d-127">String</span></span>| <span data-ttu-id="bb78d-128">Значение, используемое при настройке *псевдонима/узла или имени* записи CNAME на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="bb78d-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="bb78d-129">recordType</span><span class="sxs-lookup"><span data-stu-id="bb78d-129">recordType</span></span>|<span data-ttu-id="bb78d-130">Строка</span><span class="sxs-lookup"><span data-stu-id="bb78d-130">String</span></span>| <span data-ttu-id="bb78d-131">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="bb78d-131">Type of DNS record.</span></span> <span data-ttu-id="bb78d-132">Значение всегда равно *CNAME*.</span><span class="sxs-lookup"><span data-stu-id="bb78d-132">The value is always *CName*.</span></span> <span data-ttu-id="bb78d-133">Key</span><span class="sxs-lookup"><span data-stu-id="bb78d-133">Key</span></span>|
|<span data-ttu-id="bb78d-134">суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="bb78d-134">supportedService</span></span>|<span data-ttu-id="bb78d-135">Строка</span><span class="sxs-lookup"><span data-stu-id="bb78d-135">String</span></span>| <span data-ttu-id="bb78d-136">Служба или компонент Microsoft Online, который имеет зависимость от этой записи CNAME.</span><span class="sxs-lookup"><span data-stu-id="bb78d-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="bb78d-137">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="bb78d-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="bb78d-138">используем</span><span class="sxs-lookup"><span data-stu-id="bb78d-138">ttl</span></span>|<span data-ttu-id="bb78d-139">Int32</span><span class="sxs-lookup"><span data-stu-id="bb78d-139">Int32</span></span>| <span data-ttu-id="bb78d-140">Значение, используемое при настройке свойства срока жизни (TTL) записи CNAME на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="bb78d-140">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host.</span></span> <span data-ttu-id="bb78d-141">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="bb78d-141">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="bb78d-142">Связи</span><span class="sxs-lookup"><span data-stu-id="bb78d-142">Relationships</span></span>
<span data-ttu-id="bb78d-143">Нет</span><span class="sxs-lookup"><span data-stu-id="bb78d-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bb78d-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb78d-144">JSON representation</span></span>
<span data-ttu-id="bb78d-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb78d-145">Here is a JSON representation of the resource.</span></span>

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


