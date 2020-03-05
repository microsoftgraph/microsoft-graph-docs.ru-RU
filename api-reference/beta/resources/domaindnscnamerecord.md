---
title: Тип ресурса Домаинднскнамерекорд
description: Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9b3a957197821bfb010aed5de071ec1e89192828
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42506367"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="161be-104">Тип ресурса Домаинднскнамерекорд</span><span class="sxs-lookup"><span data-stu-id="161be-104">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="161be-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="161be-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="161be-106">Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="161be-106">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="161be-107">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="161be-107">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="161be-108">Методы</span><span class="sxs-lookup"><span data-stu-id="161be-108">Methods</span></span>
<span data-ttu-id="161be-109">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="161be-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="161be-110">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="161be-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="161be-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="161be-111">Properties</span></span>
| <span data-ttu-id="161be-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="161be-112">Property</span></span>     | <span data-ttu-id="161be-113">Тип</span><span class="sxs-lookup"><span data-stu-id="161be-113">Type</span></span>   |<span data-ttu-id="161be-114">Описание</span><span class="sxs-lookup"><span data-stu-id="161be-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="161be-115">каноникалнаме</span><span class="sxs-lookup"><span data-stu-id="161be-115">canonicalName</span></span>|<span data-ttu-id="161be-116">String</span><span class="sxs-lookup"><span data-stu-id="161be-116">String</span></span>| <span data-ttu-id="161be-117">Каноническое имя записи CNAME.</span><span class="sxs-lookup"><span data-stu-id="161be-117">The canonical name of the CNAME record.</span></span> <span data-ttu-id="161be-118">Используется для настройки записи CNAME на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="161be-118">Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="161be-119">id</span><span class="sxs-lookup"><span data-stu-id="161be-119">id</span></span>|<span data-ttu-id="161be-120">String</span><span class="sxs-lookup"><span data-stu-id="161be-120">String</span></span>| <span data-ttu-id="161be-121">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="161be-121">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="161be-122">Не допускает значение null, доступно только для чтения</span><span class="sxs-lookup"><span data-stu-id="161be-122">Not nullable, Read-only</span></span>|
|<span data-ttu-id="161be-123">Переключатель</span><span class="sxs-lookup"><span data-stu-id="161be-123">isOptional</span></span>|<span data-ttu-id="161be-124">Логический</span><span class="sxs-lookup"><span data-stu-id="161be-124">Boolean</span></span>| <span data-ttu-id="161be-125">Если значение равно false, запись CNAME должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="161be-125">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> <span data-ttu-id="161be-126">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="161be-126">Not nullable</span></span> |
|<span data-ttu-id="161be-127">label</span><span class="sxs-lookup"><span data-stu-id="161be-127">label</span></span>|<span data-ttu-id="161be-128">String</span><span class="sxs-lookup"><span data-stu-id="161be-128">String</span></span>| <span data-ttu-id="161be-129">Значение, используемое при настройке *псевдонима/узла или имени* записи CNAME на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="161be-129">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="161be-130">recordType</span><span class="sxs-lookup"><span data-stu-id="161be-130">recordType</span></span>|<span data-ttu-id="161be-131">String</span><span class="sxs-lookup"><span data-stu-id="161be-131">String</span></span>| <span data-ttu-id="161be-132">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="161be-132">Type of DNS record.</span></span> <span data-ttu-id="161be-133">Значение всегда равно *CNAME*.</span><span class="sxs-lookup"><span data-stu-id="161be-133">The value is always *CName*.</span></span> <span data-ttu-id="161be-134">Key</span><span class="sxs-lookup"><span data-stu-id="161be-134">Key</span></span>|
|<span data-ttu-id="161be-135">суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="161be-135">supportedService</span></span>|<span data-ttu-id="161be-136">String</span><span class="sxs-lookup"><span data-stu-id="161be-136">String</span></span>| <span data-ttu-id="161be-137">Служба или компонент Microsoft Online, который имеет зависимость от этой записи CNAME.</span><span class="sxs-lookup"><span data-stu-id="161be-137">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="161be-138">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="161be-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="161be-139">используем</span><span class="sxs-lookup"><span data-stu-id="161be-139">ttl</span></span>|<span data-ttu-id="161be-140">Int32</span><span class="sxs-lookup"><span data-stu-id="161be-140">Int32</span></span>| <span data-ttu-id="161be-141">Значение, используемое при настройке свойства срока жизни (TTL) записи CNAME на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="161be-141">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host.</span></span> <span data-ttu-id="161be-142">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="161be-142">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="161be-143">Связи</span><span class="sxs-lookup"><span data-stu-id="161be-143">Relationships</span></span>
<span data-ttu-id="161be-144">Нет</span><span class="sxs-lookup"><span data-stu-id="161be-144">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="161be-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="161be-145">JSON representation</span></span>
<span data-ttu-id="161be-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="161be-146">Here is a JSON representation of the resource.</span></span>

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
