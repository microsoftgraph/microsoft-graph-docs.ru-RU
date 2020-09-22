---
title: Тип ресурса Домаинднсткстрекорд
description: Представляет запись TXT, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4bc495a1cd7cc5381e75e1db3eefc87228b667b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018650"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="6b861-103">Тип ресурса Домаинднсткстрекорд</span><span class="sxs-lookup"><span data-stu-id="6b861-103">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="6b861-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b861-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b861-105">Представляет запись TXT, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6b861-105">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="6b861-106">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="6b861-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="6b861-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6b861-107">Methods</span></span>
<span data-ttu-id="6b861-108">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="6b861-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="6b861-109">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="6b861-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="6b861-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b861-110">Properties</span></span>
| <span data-ttu-id="6b861-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b861-111">Property</span></span>     | <span data-ttu-id="6b861-112">Тип</span><span class="sxs-lookup"><span data-stu-id="6b861-112">Type</span></span>   |<span data-ttu-id="6b861-113">Описание</span><span class="sxs-lookup"><span data-stu-id="6b861-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b861-114">id</span><span class="sxs-lookup"><span data-stu-id="6b861-114">id</span></span>|<span data-ttu-id="6b861-115">String</span><span class="sxs-lookup"><span data-stu-id="6b861-115">String</span></span>| <span data-ttu-id="6b861-116">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="6b861-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="6b861-117">Не допускает значения NULL и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b861-117">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="6b861-118">Переключатель</span><span class="sxs-lookup"><span data-stu-id="6b861-118">isOptional</span></span>|<span data-ttu-id="6b861-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b861-119">Boolean</span></span>| <span data-ttu-id="6b861-120">Если этот параметр имеет значение false, запись TXT должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="6b861-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="6b861-121">label</span><span class="sxs-lookup"><span data-stu-id="6b861-121">label</span></span>|<span data-ttu-id="6b861-122">String</span><span class="sxs-lookup"><span data-stu-id="6b861-122">String</span></span>| <span data-ttu-id="6b861-123">Значение, используемое при настройке свойства *Name* записи TXT на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="6b861-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="6b861-124">recordType</span><span class="sxs-lookup"><span data-stu-id="6b861-124">recordType</span></span>|<span data-ttu-id="6b861-125">String</span><span class="sxs-lookup"><span data-stu-id="6b861-125">String</span></span>| <span data-ttu-id="6b861-126">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="6b861-126">Type of DNS record.</span></span> <span data-ttu-id="6b861-127">Значение всегда является *txt*.</span><span class="sxs-lookup"><span data-stu-id="6b861-127">The value is always *Txt*.</span></span> <span data-ttu-id="6b861-128">Key</span><span class="sxs-lookup"><span data-stu-id="6b861-128">Key</span></span> |
|<span data-ttu-id="6b861-129">суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="6b861-129">supportedService</span></span>|<span data-ttu-id="6b861-130">String</span><span class="sxs-lookup"><span data-stu-id="6b861-130">String</span></span>| <span data-ttu-id="6b861-131">Служба или компонент Microsoft Online, зависящие от этой записи TXT.</span><span class="sxs-lookup"><span data-stu-id="6b861-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="6b861-132">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="6b861-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="6b861-133">текст</span><span class="sxs-lookup"><span data-stu-id="6b861-133">text</span></span>|<span data-ttu-id="6b861-134">String</span><span class="sxs-lookup"><span data-stu-id="6b861-134">String</span></span>| <span data-ttu-id="6b861-135">Значение, используемое при настройке свойства *Text* на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="6b861-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="6b861-136">используем</span><span class="sxs-lookup"><span data-stu-id="6b861-136">ttl</span></span>|<span data-ttu-id="6b861-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6b861-137">Int32</span></span>| <span data-ttu-id="6b861-138">Значение, используемое при настройке свойства срока *жизни (TTL)* записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="6b861-138">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="6b861-139">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="6b861-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="6b861-140">Связи</span><span class="sxs-lookup"><span data-stu-id="6b861-140">Relationships</span></span>
<span data-ttu-id="6b861-141">Нет</span><span class="sxs-lookup"><span data-stu-id="6b861-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6b861-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b861-142">JSON representation</span></span>
<span data-ttu-id="6b861-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b861-143">Here is a JSON representation of the resource.</span></span>

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

