---
title: тип ресурса domainDnsMxRecord
description: Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 001f831bfa3d86c0df2f6bddcf6df5e6afe9344a
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761334"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="8d23e-103">тип ресурса domainDnsMxRecord</span><span class="sxs-lookup"><span data-stu-id="8d23e-103">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="8d23e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d23e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d23e-105">Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="8d23e-105">Represents a MX record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="8d23e-106">Наследуется от [объекта DomainDnsRecord.](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="8d23e-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="8d23e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8d23e-107">Methods</span></span>
<span data-ttu-id="8d23e-108">Прямые запросы на этот ресурс не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="8d23e-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="8d23e-109">Сведения о [том,](domain.md) как запрашивать записи службы домена, см. в разделе домен.</span><span class="sxs-lookup"><span data-stu-id="8d23e-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="8d23e-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d23e-110">Properties</span></span>
| <span data-ttu-id="8d23e-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d23e-111">Property</span></span>     | <span data-ttu-id="8d23e-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8d23e-112">Type</span></span>   |<span data-ttu-id="8d23e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8d23e-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d23e-114">id</span><span class="sxs-lookup"><span data-stu-id="8d23e-114">id</span></span>|<span data-ttu-id="8d23e-115">String</span><span class="sxs-lookup"><span data-stu-id="8d23e-115">String</span></span>| <span data-ttu-id="8d23e-116">Уникальный идентификатор, присвоенный этому объекту.</span><span class="sxs-lookup"><span data-stu-id="8d23e-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="8d23e-117">Не является недействительным, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8d23e-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="8d23e-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="8d23e-118">isOptional</span></span>|<span data-ttu-id="8d23e-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d23e-119">Boolean</span></span>| <span data-ttu-id="8d23e-120">Если это не так, запись MX должна быть настроена клиентом в хосте DNS, чтобы Microsoft Online Services правильно работать с доменом.</span><span class="sxs-lookup"><span data-stu-id="8d23e-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="8d23e-121">label</span><span class="sxs-lookup"><span data-stu-id="8d23e-121">label</span></span>|<span data-ttu-id="8d23e-122">String</span><span class="sxs-lookup"><span data-stu-id="8d23e-122">String</span></span>| <span data-ttu-id="8d23e-123">Значение, используемого при настройке свойства *псевдонима/хоста/имени* записи MX в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="8d23e-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="8d23e-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="8d23e-124">mailExchange</span></span>|<span data-ttu-id="8d23e-125">String</span><span class="sxs-lookup"><span data-stu-id="8d23e-125">String</span></span>| <span data-ttu-id="8d23e-126">Значение, используемого при настройке *ответа/назначения/значения* записи MX в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="8d23e-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="8d23e-127">предпочтение</span><span class="sxs-lookup"><span data-stu-id="8d23e-127">preference</span></span>|<span data-ttu-id="8d23e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="8d23e-128">Int32</span></span>| <span data-ttu-id="8d23e-129">Значение, используемое при настройке свойства *Preference/Priority* записи MX в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="8d23e-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="8d23e-130">recordType</span><span class="sxs-lookup"><span data-stu-id="8d23e-130">recordType</span></span>|<span data-ttu-id="8d23e-131">String</span><span class="sxs-lookup"><span data-stu-id="8d23e-131">String</span></span>| <span data-ttu-id="8d23e-132">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="8d23e-132">Type of DNS record.</span></span> <span data-ttu-id="8d23e-133">Значение всегда *Mx*.</span><span class="sxs-lookup"><span data-stu-id="8d23e-133">The value is always *Mx*.</span></span> <span data-ttu-id="8d23e-134">Key</span><span class="sxs-lookup"><span data-stu-id="8d23e-134">Key</span></span> |
|<span data-ttu-id="8d23e-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="8d23e-135">supportedService</span></span>|<span data-ttu-id="8d23e-136">String</span><span class="sxs-lookup"><span data-stu-id="8d23e-136">String</span></span>| <span data-ttu-id="8d23e-137">Microsoft Online Service или функция, зависимая от этой записи MX.</span><span class="sxs-lookup"><span data-stu-id="8d23e-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="8d23e-138">Может быть одним из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="8d23e-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="8d23e-139">ttl</span><span class="sxs-lookup"><span data-stu-id="8d23e-139">ttl</span></span>|<span data-ttu-id="8d23e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8d23e-140">Int32</span></span>| <span data-ttu-id="8d23e-141">Значение, используемого при настройке свойства времени для жизни *(ttl)* записи MX в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="8d23e-141">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="8d23e-142">Не является недействительным</span><span class="sxs-lookup"><span data-stu-id="8d23e-142">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="8d23e-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="8d23e-143">Relationships</span></span>
<span data-ttu-id="8d23e-144">Нет</span><span class="sxs-lookup"><span data-stu-id="8d23e-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d23e-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d23e-145">JSON representation</span></span>
<span data-ttu-id="8d23e-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d23e-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "canonicalName": "String",
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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


