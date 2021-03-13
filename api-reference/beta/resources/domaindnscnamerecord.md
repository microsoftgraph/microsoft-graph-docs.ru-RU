---
title: тип ресурса domainDnsCnameRecord
description: Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ecbe5c0dd1d547a6abb116c5152a8d21f0ee3fd8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760885"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="8b50f-103">тип ресурса domainDnsCnameRecord</span><span class="sxs-lookup"><span data-stu-id="8b50f-103">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="8b50f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b50f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b50f-105">Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="8b50f-105">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="8b50f-106">Наследуется от [объекта DomainDnsRecord.](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="8b50f-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="8b50f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8b50f-107">Methods</span></span>
<span data-ttu-id="8b50f-108">Прямые запросы на этот ресурс не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="8b50f-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="8b50f-109">Сведения о [том,](domain.md) как запрашивать записи службы домена, см. в разделе домен.</span><span class="sxs-lookup"><span data-stu-id="8b50f-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="8b50f-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b50f-110">Properties</span></span>
| <span data-ttu-id="8b50f-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b50f-111">Property</span></span>     | <span data-ttu-id="8b50f-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8b50f-112">Type</span></span>   |<span data-ttu-id="8b50f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8b50f-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b50f-114">canonicalName</span><span class="sxs-lookup"><span data-stu-id="8b50f-114">canonicalName</span></span>|<span data-ttu-id="8b50f-115">String</span><span class="sxs-lookup"><span data-stu-id="8b50f-115">String</span></span>| <span data-ttu-id="8b50f-116">Каноническое имя записи CNAME.</span><span class="sxs-lookup"><span data-stu-id="8b50f-116">The canonical name of the CNAME record.</span></span> <span data-ttu-id="8b50f-117">Используется для настройки записи CNAME в DNS-хозяйке.</span><span class="sxs-lookup"><span data-stu-id="8b50f-117">Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="8b50f-118">id</span><span class="sxs-lookup"><span data-stu-id="8b50f-118">id</span></span>|<span data-ttu-id="8b50f-119">String</span><span class="sxs-lookup"><span data-stu-id="8b50f-119">String</span></span>| <span data-ttu-id="8b50f-120">Уникальный идентификатор, присвоенный этому объекту.</span><span class="sxs-lookup"><span data-stu-id="8b50f-120">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="8b50f-121">Не является недействительным, только для чтения</span><span class="sxs-lookup"><span data-stu-id="8b50f-121">Not nullable, Read-only</span></span>|
|<span data-ttu-id="8b50f-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="8b50f-122">isOptional</span></span>|<span data-ttu-id="8b50f-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b50f-123">Boolean</span></span>| <span data-ttu-id="8b50f-124">Если это не так, запись CNAME должна быть настроена клиентом в хосте DNS, чтобы Microsoft Online Services правильно работать с доменом.</span><span class="sxs-lookup"><span data-stu-id="8b50f-124">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> <span data-ttu-id="8b50f-125">Не является недействительным</span><span class="sxs-lookup"><span data-stu-id="8b50f-125">Not nullable</span></span> |
|<span data-ttu-id="8b50f-126">label</span><span class="sxs-lookup"><span data-stu-id="8b50f-126">label</span></span>|<span data-ttu-id="8b50f-127">String</span><span class="sxs-lookup"><span data-stu-id="8b50f-127">String</span></span>| <span data-ttu-id="8b50f-128">Значение, используемого при настройке *псевдонима/хоста/имени* записи CNAME в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="8b50f-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="8b50f-129">recordType</span><span class="sxs-lookup"><span data-stu-id="8b50f-129">recordType</span></span>|<span data-ttu-id="8b50f-130">String</span><span class="sxs-lookup"><span data-stu-id="8b50f-130">String</span></span>| <span data-ttu-id="8b50f-131">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="8b50f-131">Type of DNS record.</span></span> <span data-ttu-id="8b50f-132">Значение всегда *CName*.</span><span class="sxs-lookup"><span data-stu-id="8b50f-132">The value is always *CName*.</span></span> <span data-ttu-id="8b50f-133">Key</span><span class="sxs-lookup"><span data-stu-id="8b50f-133">Key</span></span>|
|<span data-ttu-id="8b50f-134">supportedService</span><span class="sxs-lookup"><span data-stu-id="8b50f-134">supportedService</span></span>|<span data-ttu-id="8b50f-135">String</span><span class="sxs-lookup"><span data-stu-id="8b50f-135">String</span></span>| <span data-ttu-id="8b50f-136">Microsoft Online Service или функция, зависимая от этой записи CNAME.</span><span class="sxs-lookup"><span data-stu-id="8b50f-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="8b50f-137">Может быть одним из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="8b50f-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="8b50f-138">ttl</span><span class="sxs-lookup"><span data-stu-id="8b50f-138">ttl</span></span>|<span data-ttu-id="8b50f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8b50f-139">Int32</span></span>| <span data-ttu-id="8b50f-140">Значение, используемого при настройке свойства "время на жизнь" записи CNAME в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="8b50f-140">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host.</span></span> <span data-ttu-id="8b50f-141">Не является недействительным</span><span class="sxs-lookup"><span data-stu-id="8b50f-141">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="8b50f-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="8b50f-142">Relationships</span></span>
<span data-ttu-id="8b50f-143">Нет</span><span class="sxs-lookup"><span data-stu-id="8b50f-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8b50f-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b50f-144">JSON representation</span></span>
<span data-ttu-id="8b50f-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b50f-145">Here is a JSON representation of the resource.</span></span>

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


