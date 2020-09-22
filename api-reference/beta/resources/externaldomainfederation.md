---
title: Тип ресурса Екстерналдомаинфедератион
description: Тип Екстерналдомаинфедератион определяет домен, не относящийся к клиенту, с настроенным поставщиком удостоверений в качестве источника удостоверений для подключенной Организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d81255a3687bf3d6aafe9369f901b209f5827b77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026917"
---
# <a name="externaldomainfederation-resource-type"></a><span data-ttu-id="20a6b-103">Тип ресурса Екстерналдомаинфедератион</span><span class="sxs-lookup"><span data-stu-id="20a6b-103">externalDomainFederation resource type</span></span>

<span data-ttu-id="20a6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20a6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20a6b-105">Используется в источниках удостоверений [коннектедорганизатион](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="20a6b-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="20a6b-106">`@odata.type`Значение `#microsoft.graph.externalDomainFederation` указывает на то, что этот тип определяет домен с настроенным поставщиком удостоверений в качестве источника удостоверений для подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="20a6b-106">The `@odata.type` value `#microsoft.graph.externalDomainFederation` indicates that this type identifies a domain with a configured identity provider as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="20a6b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="20a6b-107">Properties</span></span>

| <span data-ttu-id="20a6b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="20a6b-108">Property</span></span>                     | <span data-ttu-id="20a6b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="20a6b-109">Type</span></span>                      | <span data-ttu-id="20a6b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="20a6b-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="20a6b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="20a6b-111">displayName</span></span> |<span data-ttu-id="20a6b-112">String</span><span class="sxs-lookup"><span data-stu-id="20a6b-112">String</span></span> | <span data-ttu-id="20a6b-113">Имя источника удостоверений, как правило, также доменное имя.</span><span class="sxs-lookup"><span data-stu-id="20a6b-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="20a6b-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20a6b-114">Read only.</span></span> |
| <span data-ttu-id="20a6b-115">domainName</span><span class="sxs-lookup"><span data-stu-id="20a6b-115">domainName</span></span> |<span data-ttu-id="20a6b-116">String</span><span class="sxs-lookup"><span data-stu-id="20a6b-116">String</span></span> | <span data-ttu-id="20a6b-117">Доменное имя.</span><span class="sxs-lookup"><span data-stu-id="20a6b-117">The domain name.</span></span> <span data-ttu-id="20a6b-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20a6b-118">Read only.</span></span> |
| <span data-ttu-id="20a6b-119">иссуерури</span><span class="sxs-lookup"><span data-stu-id="20a6b-119">issuerUri</span></span> |<span data-ttu-id="20a6b-120">String</span><span class="sxs-lookup"><span data-stu-id="20a6b-120">String</span></span> | <span data-ttu-id="20a6b-121">Иссуерури входящей Федерации.</span><span class="sxs-lookup"><span data-stu-id="20a6b-121">The issuerURI of the incoming federation.</span></span> <span data-ttu-id="20a6b-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20a6b-122">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="20a6b-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="20a6b-123">Relationships</span></span>

<span data-ttu-id="20a6b-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="20a6b-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="20a6b-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="20a6b-125">JSON representation</span></span>

<span data-ttu-id="20a6b-126">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20a6b-126">The following is a JSON representation of the type.</span></span>

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


