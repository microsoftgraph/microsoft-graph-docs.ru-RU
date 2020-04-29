---
title: Тип ресурса Домаинднсмксрекорд
description: Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: af95edfde834e04449398b1a9b306fe29529a15d
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181653"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="2e668-103">Тип ресурса Домаинднсмксрекорд</span><span class="sxs-lookup"><span data-stu-id="2e668-103">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="2e668-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e668-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e668-105">Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2e668-105">Represents a MX record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="2e668-106">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="2e668-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="2e668-107">Methods</span><span class="sxs-lookup"><span data-stu-id="2e668-107">Methods</span></span>
<span data-ttu-id="2e668-108">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="2e668-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="2e668-109">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="2e668-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="2e668-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e668-110">Properties</span></span>
| <span data-ttu-id="2e668-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e668-111">Property</span></span>     | <span data-ttu-id="2e668-112">Тип</span><span class="sxs-lookup"><span data-stu-id="2e668-112">Type</span></span>   |<span data-ttu-id="2e668-113">Описание</span><span class="sxs-lookup"><span data-stu-id="2e668-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e668-114">id</span><span class="sxs-lookup"><span data-stu-id="2e668-114">id</span></span>|<span data-ttu-id="2e668-115">String</span><span class="sxs-lookup"><span data-stu-id="2e668-115">String</span></span>| <span data-ttu-id="2e668-116">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="2e668-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="2e668-117">Не допускает значения NULL и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e668-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="2e668-118">Переключатель</span><span class="sxs-lookup"><span data-stu-id="2e668-118">isOptional</span></span>|<span data-ttu-id="2e668-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e668-119">Boolean</span></span>| <span data-ttu-id="2e668-120">Если задано значение false, запись MX должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="2e668-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="2e668-121">label</span><span class="sxs-lookup"><span data-stu-id="2e668-121">label</span></span>|<span data-ttu-id="2e668-122">String</span><span class="sxs-lookup"><span data-stu-id="2e668-122">String</span></span>| <span data-ttu-id="2e668-123">Значение, используемое при настройке свойства *Alias/Host/Name* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="2e668-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="2e668-124">маилексчанже</span><span class="sxs-lookup"><span data-stu-id="2e668-124">mailExchange</span></span>|<span data-ttu-id="2e668-125">String</span><span class="sxs-lookup"><span data-stu-id="2e668-125">String</span></span>| <span data-ttu-id="2e668-126">Значение, используемое при настройке *ответа/назначения/значения* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="2e668-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="2e668-127">параметров</span><span class="sxs-lookup"><span data-stu-id="2e668-127">preference</span></span>|<span data-ttu-id="2e668-128">Int32</span><span class="sxs-lookup"><span data-stu-id="2e668-128">Int32</span></span>| <span data-ttu-id="2e668-129">Значение, используемое при настройке свойства *предпочтения/приоритета* записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="2e668-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="2e668-130">recordType</span><span class="sxs-lookup"><span data-stu-id="2e668-130">recordType</span></span>|<span data-ttu-id="2e668-131">String</span><span class="sxs-lookup"><span data-stu-id="2e668-131">String</span></span>| <span data-ttu-id="2e668-132">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="2e668-132">Type of DNS record.</span></span> <span data-ttu-id="2e668-133">Значение — это всегда *MX*.</span><span class="sxs-lookup"><span data-stu-id="2e668-133">The value is always *Mx*.</span></span> <span data-ttu-id="2e668-134">Key</span><span class="sxs-lookup"><span data-stu-id="2e668-134">Key</span></span> |
|<span data-ttu-id="2e668-135">суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="2e668-135">supportedService</span></span>|<span data-ttu-id="2e668-136">String</span><span class="sxs-lookup"><span data-stu-id="2e668-136">String</span></span>| <span data-ttu-id="2e668-137">Служба или компонент Microsoft Online, который имеет зависимость от этой записи MX.</span><span class="sxs-lookup"><span data-stu-id="2e668-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="2e668-138">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="2e668-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="2e668-139">используем</span><span class="sxs-lookup"><span data-stu-id="2e668-139">ttl</span></span>|<span data-ttu-id="2e668-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2e668-140">Int32</span></span>| <span data-ttu-id="2e668-141">Значение, используемое при настройке свойства срока *жизни (TTL)* записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="2e668-141">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="2e668-142">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="2e668-142">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="2e668-143">Связи</span><span class="sxs-lookup"><span data-stu-id="2e668-143">Relationships</span></span>
<span data-ttu-id="2e668-144">Нет</span><span class="sxs-lookup"><span data-stu-id="2e668-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e668-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e668-145">JSON representation</span></span>
<span data-ttu-id="2e668-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e668-146">Here is a JSON representation of the resource.</span></span>

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
