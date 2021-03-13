---
title: тип ресурса domainDnsTxtRecord
description: Представляет запись TXT, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9e59c38028b414208744793945ed480dc708bf6c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760906"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="f3838-103">тип ресурса domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="f3838-103">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="f3838-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3838-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3838-105">Представляет запись TXT, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="f3838-105">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="f3838-106">Наследуется от [объекта DomainDnsRecord.](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="f3838-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="f3838-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f3838-107">Methods</span></span>
<span data-ttu-id="f3838-108">Прямые запросы на этот ресурс не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="f3838-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="f3838-109">Сведения о [том,](domain.md) как запрашивать записи службы домена, см. в разделе домен.</span><span class="sxs-lookup"><span data-stu-id="f3838-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="f3838-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3838-110">Properties</span></span>
| <span data-ttu-id="f3838-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3838-111">Property</span></span>     | <span data-ttu-id="f3838-112">Тип</span><span class="sxs-lookup"><span data-stu-id="f3838-112">Type</span></span>   |<span data-ttu-id="f3838-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f3838-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3838-114">id</span><span class="sxs-lookup"><span data-stu-id="f3838-114">id</span></span>|<span data-ttu-id="f3838-115">String</span><span class="sxs-lookup"><span data-stu-id="f3838-115">String</span></span>| <span data-ttu-id="f3838-116">Уникальный идентификатор, присвоенный этому объекту.</span><span class="sxs-lookup"><span data-stu-id="f3838-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="f3838-117">Не является недействительным, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3838-117">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="f3838-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="f3838-118">isOptional</span></span>|<span data-ttu-id="f3838-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3838-119">Boolean</span></span>| <span data-ttu-id="f3838-120">Если это неверно, запись TXT должна быть настроена клиентом на хост DNS, чтобы Microsoft Online Services правильно работать с доменом.</span><span class="sxs-lookup"><span data-stu-id="f3838-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="f3838-121">label</span><span class="sxs-lookup"><span data-stu-id="f3838-121">label</span></span>|<span data-ttu-id="f3838-122">String</span><span class="sxs-lookup"><span data-stu-id="f3838-122">String</span></span>| <span data-ttu-id="f3838-123">Значение, которое необходимо  использовать при настройке свойства имени записи TXT в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="f3838-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="f3838-124">recordType</span><span class="sxs-lookup"><span data-stu-id="f3838-124">recordType</span></span>|<span data-ttu-id="f3838-125">String</span><span class="sxs-lookup"><span data-stu-id="f3838-125">String</span></span>| <span data-ttu-id="f3838-126">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="f3838-126">Type of DNS record.</span></span> <span data-ttu-id="f3838-127">Значение всегда *Txt*.</span><span class="sxs-lookup"><span data-stu-id="f3838-127">The value is always *Txt*.</span></span> <span data-ttu-id="f3838-128">Key</span><span class="sxs-lookup"><span data-stu-id="f3838-128">Key</span></span> |
|<span data-ttu-id="f3838-129">supportedService</span><span class="sxs-lookup"><span data-stu-id="f3838-129">supportedService</span></span>|<span data-ttu-id="f3838-130">String</span><span class="sxs-lookup"><span data-stu-id="f3838-130">String</span></span>| <span data-ttu-id="f3838-131">Microsoft Online Service или функция, зависимая от этой записи TXT.</span><span class="sxs-lookup"><span data-stu-id="f3838-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="f3838-132">Может быть одним из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="f3838-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="f3838-133">текст</span><span class="sxs-lookup"><span data-stu-id="f3838-133">text</span></span>|<span data-ttu-id="f3838-134">String</span><span class="sxs-lookup"><span data-stu-id="f3838-134">String</span></span>| <span data-ttu-id="f3838-135">Значение, используемее при настройке *свойства текста* в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="f3838-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="f3838-136">ttl</span><span class="sxs-lookup"><span data-stu-id="f3838-136">ttl</span></span>|<span data-ttu-id="f3838-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f3838-137">Int32</span></span>| <span data-ttu-id="f3838-138">Значение, используемого при настройке свойства времени для жизни *(ttl)* записи MX в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="f3838-138">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="f3838-139">Не является недействительным</span><span class="sxs-lookup"><span data-stu-id="f3838-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="f3838-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="f3838-140">Relationships</span></span>
<span data-ttu-id="f3838-141">Нет</span><span class="sxs-lookup"><span data-stu-id="f3838-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f3838-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3838-142">JSON representation</span></span>
<span data-ttu-id="f3838-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3838-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
  "canonicalName": "String",
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
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


