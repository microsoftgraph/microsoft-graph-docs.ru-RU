---
title: Тип ресурса domainDnsTxtRecord
description: Представляет запись типа TXT, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4bdcddc0ec81d8a7fc76e2113155fdc7ee871161
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522247"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="0d945-104">Тип ресурса domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="0d945-104">domainDnsTxtRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d945-p102">Представляет запись типа TXT, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="0d945-p102">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="0d945-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0d945-107">Methods</span></span>
<span data-ttu-id="0d945-p103">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="0d945-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="0d945-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d945-110">Properties</span></span>
| <span data-ttu-id="0d945-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d945-111">Property</span></span>     | <span data-ttu-id="0d945-112">Тип</span><span class="sxs-lookup"><span data-stu-id="0d945-112">Type</span></span>   |<span data-ttu-id="0d945-113">Описание</span><span class="sxs-lookup"><span data-stu-id="0d945-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d945-114">id</span><span class="sxs-lookup"><span data-stu-id="0d945-114">id</span></span>|<span data-ttu-id="0d945-115">String</span><span class="sxs-lookup"><span data-stu-id="0d945-115">String</span></span>| <span data-ttu-id="0d945-p104">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d945-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="0d945-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="0d945-118">isOptional</span></span>|<span data-ttu-id="0d945-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d945-119">Boolean</span></span>| <span data-ttu-id="0d945-120">Если имеет значение false, пользователю необходимо настроить запись типа TXT на узле DNS, чтобы службы Microsoft Online Services правильно работали с доменом.</span><span class="sxs-lookup"><span data-stu-id="0d945-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="0d945-121">label</span><span class="sxs-lookup"><span data-stu-id="0d945-121">label</span></span>|<span data-ttu-id="0d945-122">String</span><span class="sxs-lookup"><span data-stu-id="0d945-122">String</span></span>| <span data-ttu-id="0d945-123">Значение, используемое при настройке свойства *name* для записи типа TXT на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="0d945-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="0d945-124">recordType</span><span class="sxs-lookup"><span data-stu-id="0d945-124">recordType</span></span>|<span data-ttu-id="0d945-125">String</span><span class="sxs-lookup"><span data-stu-id="0d945-125">String</span></span>| <span data-ttu-id="0d945-p105">Тип записи DNS. Это свойство всегда имеет значение *Txt*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="0d945-p105">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="0d945-129">supportedService</span><span class="sxs-lookup"><span data-stu-id="0d945-129">supportedService</span></span>|<span data-ttu-id="0d945-130">Строка</span><span class="sxs-lookup"><span data-stu-id="0d945-130">String</span></span>| <span data-ttu-id="0d945-131">Служба или компонент Microsoft Online Services, зависящие от этой записи типа TXT.</span><span class="sxs-lookup"><span data-stu-id="0d945-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="0d945-132">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="0d945-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="0d945-133">text</span><span class="sxs-lookup"><span data-stu-id="0d945-133">text</span></span>|<span data-ttu-id="0d945-134">String</span><span class="sxs-lookup"><span data-stu-id="0d945-134">String</span></span>| <span data-ttu-id="0d945-135">Значение, используемое при настройке свойства *text* на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="0d945-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="0d945-136">ttl</span><span class="sxs-lookup"><span data-stu-id="0d945-136">ttl</span></span>|<span data-ttu-id="0d945-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0d945-137">Int32</span></span>| <span data-ttu-id="0d945-p106">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи MX на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="0d945-p106">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="0d945-140">Связи</span><span class="sxs-lookup"><span data-stu-id="0d945-140">Relationships</span></span>
<span data-ttu-id="0d945-141">Нет</span><span class="sxs-lookup"><span data-stu-id="0d945-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0d945-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d945-142">JSON representation</span></span>
<span data-ttu-id="0d945-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d945-143">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnstxtrecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
