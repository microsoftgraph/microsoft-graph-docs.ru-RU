---
title: Тип ресурса Домаинднсткстрекорд
description: Представляет запись TXT, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8694a0a64926f545dcc7ab5e8251961e53638c62
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657618"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="d92e2-104">Тип ресурса Домаинднсткстрекорд</span><span class="sxs-lookup"><span data-stu-id="d92e2-104">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="d92e2-105">Представляет запись TXT, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d92e2-105">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="d92e2-106">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="d92e2-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="d92e2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d92e2-107">Methods</span></span>
<span data-ttu-id="d92e2-108">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="d92e2-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="d92e2-109">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="d92e2-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="d92e2-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="d92e2-110">Properties</span></span>
| <span data-ttu-id="d92e2-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="d92e2-111">Property</span></span>     | <span data-ttu-id="d92e2-112">Тип</span><span class="sxs-lookup"><span data-stu-id="d92e2-112">Type</span></span>   |<span data-ttu-id="d92e2-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d92e2-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d92e2-114">id</span><span class="sxs-lookup"><span data-stu-id="d92e2-114">id</span></span>|<span data-ttu-id="d92e2-115">String</span><span class="sxs-lookup"><span data-stu-id="d92e2-115">String</span></span>| <span data-ttu-id="d92e2-116">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="d92e2-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="d92e2-117">Не допускает значения NULL и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d92e2-117">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="d92e2-118">Переключатель</span><span class="sxs-lookup"><span data-stu-id="d92e2-118">isOptional</span></span>|<span data-ttu-id="d92e2-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="d92e2-119">Boolean</span></span>| <span data-ttu-id="d92e2-120">Если этот параметр имеет значение false, запись TXT должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="d92e2-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="d92e2-121">label</span><span class="sxs-lookup"><span data-stu-id="d92e2-121">label</span></span>|<span data-ttu-id="d92e2-122">String</span><span class="sxs-lookup"><span data-stu-id="d92e2-122">String</span></span>| <span data-ttu-id="d92e2-123">Значение, используемое при настройке свойства *Name* записи TXT на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="d92e2-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="d92e2-124">recordType</span><span class="sxs-lookup"><span data-stu-id="d92e2-124">recordType</span></span>|<span data-ttu-id="d92e2-125">String</span><span class="sxs-lookup"><span data-stu-id="d92e2-125">String</span></span>| <span data-ttu-id="d92e2-126">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="d92e2-126">Type of DNS record.</span></span> <span data-ttu-id="d92e2-127">Значение всегда является *txt*.</span><span class="sxs-lookup"><span data-stu-id="d92e2-127">The value is always *Txt*.</span></span> <span data-ttu-id="d92e2-128">Key</span><span class="sxs-lookup"><span data-stu-id="d92e2-128">Key</span></span> |
|<span data-ttu-id="d92e2-129">Суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="d92e2-129">supportedService</span></span>|<span data-ttu-id="d92e2-130">String</span><span class="sxs-lookup"><span data-stu-id="d92e2-130">String</span></span>| <span data-ttu-id="d92e2-131">Служба или компонент Microsoft Online, зависящие от этой записи TXT.</span><span class="sxs-lookup"><span data-stu-id="d92e2-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="d92e2-132">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, \*SharePointPublic \*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="d92e2-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="d92e2-133">текст</span><span class="sxs-lookup"><span data-stu-id="d92e2-133">text</span></span>|<span data-ttu-id="d92e2-134">String</span><span class="sxs-lookup"><span data-stu-id="d92e2-134">String</span></span>| <span data-ttu-id="d92e2-135">Значение, используемое при настройке свойства *Text* на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="d92e2-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="d92e2-136">используем</span><span class="sxs-lookup"><span data-stu-id="d92e2-136">ttl</span></span>|<span data-ttu-id="d92e2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d92e2-137">Int32</span></span>| <span data-ttu-id="d92e2-138">Значение, используемое при настройке свойства срока *жизни (TTL)* записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="d92e2-138">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="d92e2-139">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="d92e2-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="d92e2-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="d92e2-140">Relationships</span></span>
<span data-ttu-id="d92e2-141">Нет</span><span class="sxs-lookup"><span data-stu-id="d92e2-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d92e2-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d92e2-142">JSON representation</span></span>
<span data-ttu-id="d92e2-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d92e2-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
