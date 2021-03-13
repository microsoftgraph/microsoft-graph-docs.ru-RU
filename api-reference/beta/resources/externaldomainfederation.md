---
title: тип ресурса externalDomainFederation
description: Тип externalDomainFederation определяет домен, не нанимаемый клиентом, с настроенным поставщиком удостоверений в качестве источника удостоверений для связанной организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: df88fef22c2acb86cadcfaed9a8f5be25da70f9d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760990"
---
# <a name="externaldomainfederation-resource-type"></a><span data-ttu-id="1b527-103">тип ресурса externalDomainFederation</span><span class="sxs-lookup"><span data-stu-id="1b527-103">externalDomainFederation resource type</span></span>

<span data-ttu-id="1b527-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b527-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b527-105">Используется в источниках удостоверений [подключеннойорганизации.](connectedOrganization.md)</span><span class="sxs-lookup"><span data-stu-id="1b527-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="1b527-106">Значение указывает, что этот тип определяет домен с настроенным поставщиком удостоверений в качестве источника удостоверений `@odata.type` `#microsoft.graph.externalDomainFederation` для связанной организации.</span><span class="sxs-lookup"><span data-stu-id="1b527-106">The `@odata.type` value `#microsoft.graph.externalDomainFederation` indicates that this type identifies a domain with a configured identity provider as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="1b527-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b527-107">Properties</span></span>

| <span data-ttu-id="1b527-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b527-108">Property</span></span>                     | <span data-ttu-id="1b527-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1b527-109">Type</span></span>                      | <span data-ttu-id="1b527-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1b527-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="1b527-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1b527-111">displayName</span></span> |<span data-ttu-id="1b527-112">String</span><span class="sxs-lookup"><span data-stu-id="1b527-112">String</span></span> | <span data-ttu-id="1b527-113">Имя источника удостоверений, как правило, также доменное имя.</span><span class="sxs-lookup"><span data-stu-id="1b527-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="1b527-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b527-114">Read only.</span></span> |
| <span data-ttu-id="1b527-115">domainName</span><span class="sxs-lookup"><span data-stu-id="1b527-115">domainName</span></span> |<span data-ttu-id="1b527-116">String</span><span class="sxs-lookup"><span data-stu-id="1b527-116">String</span></span> | <span data-ttu-id="1b527-117">Доменное имя.</span><span class="sxs-lookup"><span data-stu-id="1b527-117">The domain name.</span></span> <span data-ttu-id="1b527-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b527-118">Read only.</span></span> |
| <span data-ttu-id="1b527-119">issuerUri</span><span class="sxs-lookup"><span data-stu-id="1b527-119">issuerUri</span></span> |<span data-ttu-id="1b527-120">String</span><span class="sxs-lookup"><span data-stu-id="1b527-120">String</span></span> | <span data-ttu-id="1b527-121">IssuerURI входящих федераций.</span><span class="sxs-lookup"><span data-stu-id="1b527-121">The issuerURI of the incoming federation.</span></span> <span data-ttu-id="1b527-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b527-122">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1b527-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="1b527-123">Relationships</span></span>

<span data-ttu-id="1b527-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1b527-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b527-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1b527-125">JSON representation</span></span>

<span data-ttu-id="1b527-126">Ниже приводится представление JSON этого типа.</span><span class="sxs-lookup"><span data-stu-id="1b527-126">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalDomainFederation",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String",
  "issuerUri": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalDomainFederation resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


