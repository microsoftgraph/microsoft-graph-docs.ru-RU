---
title: Тип ресурса Домаинднсткстрекорд
description: Представляет запись TXT, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5555fa6f02e0639f1e126112918c39168b445945
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505849"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="3feac-104">Тип ресурса Домаинднсткстрекорд</span><span class="sxs-lookup"><span data-stu-id="3feac-104">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="3feac-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3feac-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3feac-106">Представляет запись TXT, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3feac-106">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="3feac-107">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="3feac-107">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="3feac-108">Методы</span><span class="sxs-lookup"><span data-stu-id="3feac-108">Methods</span></span>
<span data-ttu-id="3feac-109">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="3feac-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="3feac-110">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="3feac-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="3feac-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="3feac-111">Properties</span></span>
| <span data-ttu-id="3feac-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="3feac-112">Property</span></span>     | <span data-ttu-id="3feac-113">Тип</span><span class="sxs-lookup"><span data-stu-id="3feac-113">Type</span></span>   |<span data-ttu-id="3feac-114">Описание</span><span class="sxs-lookup"><span data-stu-id="3feac-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3feac-115">id</span><span class="sxs-lookup"><span data-stu-id="3feac-115">id</span></span>|<span data-ttu-id="3feac-116">String</span><span class="sxs-lookup"><span data-stu-id="3feac-116">String</span></span>| <span data-ttu-id="3feac-117">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="3feac-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="3feac-118">Не допускает значения NULL и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3feac-118">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="3feac-119">Переключатель</span><span class="sxs-lookup"><span data-stu-id="3feac-119">isOptional</span></span>|<span data-ttu-id="3feac-120">Логический</span><span class="sxs-lookup"><span data-stu-id="3feac-120">Boolean</span></span>| <span data-ttu-id="3feac-121">Если этот параметр имеет значение false, запись TXT должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="3feac-121">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="3feac-122">label</span><span class="sxs-lookup"><span data-stu-id="3feac-122">label</span></span>|<span data-ttu-id="3feac-123">String</span><span class="sxs-lookup"><span data-stu-id="3feac-123">String</span></span>| <span data-ttu-id="3feac-124">Значение, используемое при настройке свойства *Name* записи TXT на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="3feac-124">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="3feac-125">recordType</span><span class="sxs-lookup"><span data-stu-id="3feac-125">recordType</span></span>|<span data-ttu-id="3feac-126">String</span><span class="sxs-lookup"><span data-stu-id="3feac-126">String</span></span>| <span data-ttu-id="3feac-127">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="3feac-127">Type of DNS record.</span></span> <span data-ttu-id="3feac-128">Значение всегда является *txt*.</span><span class="sxs-lookup"><span data-stu-id="3feac-128">The value is always *Txt*.</span></span> <span data-ttu-id="3feac-129">Key</span><span class="sxs-lookup"><span data-stu-id="3feac-129">Key</span></span> |
|<span data-ttu-id="3feac-130">суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="3feac-130">supportedService</span></span>|<span data-ttu-id="3feac-131">String</span><span class="sxs-lookup"><span data-stu-id="3feac-131">String</span></span>| <span data-ttu-id="3feac-132">Служба или компонент Microsoft Online, зависящие от этой записи TXT.</span><span class="sxs-lookup"><span data-stu-id="3feac-132">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="3feac-133">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="3feac-133">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="3feac-134">текст</span><span class="sxs-lookup"><span data-stu-id="3feac-134">text</span></span>|<span data-ttu-id="3feac-135">String</span><span class="sxs-lookup"><span data-stu-id="3feac-135">String</span></span>| <span data-ttu-id="3feac-136">Значение, используемое при настройке свойства *Text* на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="3feac-136">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="3feac-137">используем</span><span class="sxs-lookup"><span data-stu-id="3feac-137">ttl</span></span>|<span data-ttu-id="3feac-138">Int32</span><span class="sxs-lookup"><span data-stu-id="3feac-138">Int32</span></span>| <span data-ttu-id="3feac-139">Значение, используемое при настройке свойства срока *жизни (TTL)* записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="3feac-139">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="3feac-140">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="3feac-140">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="3feac-141">Связи</span><span class="sxs-lookup"><span data-stu-id="3feac-141">Relationships</span></span>
<span data-ttu-id="3feac-142">Нет</span><span class="sxs-lookup"><span data-stu-id="3feac-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3feac-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3feac-143">JSON representation</span></span>
<span data-ttu-id="3feac-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3feac-144">Here is a JSON representation of the resource.</span></span>

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
