---
title: Тип ресурса Домаинднсмксрекорд
description: Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d0c7324f5c0760ff62cb3b835f7e011dd8a0a5a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531607"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="776ec-104">Тип ресурса Домаинднсмксрекорд</span><span class="sxs-lookup"><span data-stu-id="776ec-104">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="776ec-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="776ec-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="776ec-106">Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="776ec-106">Represents a MX record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="776ec-107">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="776ec-107">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="776ec-108">Методы</span><span class="sxs-lookup"><span data-stu-id="776ec-108">Methods</span></span>
<span data-ttu-id="776ec-109">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="776ec-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="776ec-110">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="776ec-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="776ec-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="776ec-111">Properties</span></span>
| <span data-ttu-id="776ec-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="776ec-112">Property</span></span>     | <span data-ttu-id="776ec-113">Тип</span><span class="sxs-lookup"><span data-stu-id="776ec-113">Type</span></span>   |<span data-ttu-id="776ec-114">Описание</span><span class="sxs-lookup"><span data-stu-id="776ec-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="776ec-115">id</span><span class="sxs-lookup"><span data-stu-id="776ec-115">id</span></span>|<span data-ttu-id="776ec-116">Строка</span><span class="sxs-lookup"><span data-stu-id="776ec-116">String</span></span>| <span data-ttu-id="776ec-117">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="776ec-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="776ec-118">Не допускает значения NULL и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="776ec-118">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="776ec-119">Переключатель</span><span class="sxs-lookup"><span data-stu-id="776ec-119">isOptional</span></span>|<span data-ttu-id="776ec-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="776ec-120">Boolean</span></span>| <span data-ttu-id="776ec-121">Если задано значение false, запись MX должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="776ec-121">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="776ec-122">label</span><span class="sxs-lookup"><span data-stu-id="776ec-122">label</span></span>|<span data-ttu-id="776ec-123">Строка</span><span class="sxs-lookup"><span data-stu-id="776ec-123">String</span></span>| <span data-ttu-id="776ec-124">Значение, используемое при настройке свойства *Alias/Host/Name* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="776ec-124">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="776ec-125">маилексчанже</span><span class="sxs-lookup"><span data-stu-id="776ec-125">mailExchange</span></span>|<span data-ttu-id="776ec-126">Строка</span><span class="sxs-lookup"><span data-stu-id="776ec-126">String</span></span>| <span data-ttu-id="776ec-127">Значение, используемое при настройке *ответа/назначения/значения* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="776ec-127">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="776ec-128">параметров</span><span class="sxs-lookup"><span data-stu-id="776ec-128">preference</span></span>|<span data-ttu-id="776ec-129">Int32</span><span class="sxs-lookup"><span data-stu-id="776ec-129">Int32</span></span>| <span data-ttu-id="776ec-130">Значение, используемое при настройке свойства *предпочтения/приоритета* записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="776ec-130">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="776ec-131">recordType</span><span class="sxs-lookup"><span data-stu-id="776ec-131">recordType</span></span>|<span data-ttu-id="776ec-132">Строка</span><span class="sxs-lookup"><span data-stu-id="776ec-132">String</span></span>| <span data-ttu-id="776ec-133">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="776ec-133">Type of DNS record.</span></span> <span data-ttu-id="776ec-134">Значение — это всегда *MX*.</span><span class="sxs-lookup"><span data-stu-id="776ec-134">The value is always *Mx*.</span></span> <span data-ttu-id="776ec-135">Key</span><span class="sxs-lookup"><span data-stu-id="776ec-135">Key</span></span> |
|<span data-ttu-id="776ec-136">суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="776ec-136">supportedService</span></span>|<span data-ttu-id="776ec-137">Строка</span><span class="sxs-lookup"><span data-stu-id="776ec-137">String</span></span>| <span data-ttu-id="776ec-138">Служба или компонент Microsoft Online, который имеет зависимость от этой записи MX.</span><span class="sxs-lookup"><span data-stu-id="776ec-138">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="776ec-139">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="776ec-139">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="776ec-140">используем</span><span class="sxs-lookup"><span data-stu-id="776ec-140">ttl</span></span>|<span data-ttu-id="776ec-141">Int32</span><span class="sxs-lookup"><span data-stu-id="776ec-141">Int32</span></span>| <span data-ttu-id="776ec-142">Значение, используемое при настройке свойства срока *жизни (TTL)* записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="776ec-142">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="776ec-143">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="776ec-143">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="776ec-144">Связи</span><span class="sxs-lookup"><span data-stu-id="776ec-144">Relationships</span></span>
<span data-ttu-id="776ec-145">Нет</span><span class="sxs-lookup"><span data-stu-id="776ec-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="776ec-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="776ec-146">JSON representation</span></span>
<span data-ttu-id="776ec-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="776ec-147">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
