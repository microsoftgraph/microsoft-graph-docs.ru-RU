---
title: Тип ресурса Екстерналдомаинфедератион
description: Тип Екстерналдомаинфедератион определяет домен, не относящийся к клиенту, с настроенным поставщиком удостоверений в качестве источника удостоверений для подключенной Организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ffeaa955ac43a52a0e3485f4a561163d4d27a957
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510300"
---
# <a name="externaldomainfederation-resource-type"></a><span data-ttu-id="ede21-103">Тип ресурса Екстерналдомаинфедератион</span><span class="sxs-lookup"><span data-stu-id="ede21-103">externalDomainFederation resource type</span></span>

<span data-ttu-id="ede21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ede21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ede21-105">Используется в источниках удостоверений [коннектедорганизатион](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="ede21-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="ede21-106">`@odata.type`Значение `#microsoft.graph.externalDomainFederation` указывает на то, что этот тип определяет домен с настроенным поставщиком удостоверений в качестве источника удостоверений для подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="ede21-106">The `@odata.type` value `#microsoft.graph.externalDomainFederation` indicates that this type identifies a domain with a configured identity provider as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="ede21-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ede21-107">Properties</span></span>

| <span data-ttu-id="ede21-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ede21-108">Property</span></span>                     | <span data-ttu-id="ede21-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ede21-109">Type</span></span>                      | <span data-ttu-id="ede21-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ede21-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="ede21-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ede21-111">displayName</span></span> |<span data-ttu-id="ede21-112">Строка</span><span class="sxs-lookup"><span data-stu-id="ede21-112">String</span></span> | <span data-ttu-id="ede21-113">Имя источника удостоверений, как правило, также доменное имя.</span><span class="sxs-lookup"><span data-stu-id="ede21-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="ede21-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ede21-114">Read only.</span></span> |
| <span data-ttu-id="ede21-115">domainName</span><span class="sxs-lookup"><span data-stu-id="ede21-115">domainName</span></span> |<span data-ttu-id="ede21-116">String</span><span class="sxs-lookup"><span data-stu-id="ede21-116">String</span></span> | <span data-ttu-id="ede21-117">Доменное имя.</span><span class="sxs-lookup"><span data-stu-id="ede21-117">The domain name.</span></span> <span data-ttu-id="ede21-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ede21-118">Read only.</span></span> |
| <span data-ttu-id="ede21-119">иссуерури</span><span class="sxs-lookup"><span data-stu-id="ede21-119">issuerUri</span></span> |<span data-ttu-id="ede21-120">Строка</span><span class="sxs-lookup"><span data-stu-id="ede21-120">String</span></span> | <span data-ttu-id="ede21-121">Иссуерури входящей Федерации.</span><span class="sxs-lookup"><span data-stu-id="ede21-121">The issuerURI of the incoming federation.</span></span> <span data-ttu-id="ede21-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ede21-122">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ede21-123">Связи</span><span class="sxs-lookup"><span data-stu-id="ede21-123">Relationships</span></span>

<span data-ttu-id="ede21-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ede21-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ede21-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ede21-125">JSON representation</span></span>

<span data-ttu-id="ede21-126">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ede21-126">The following is a JSON representation of the type.</span></span>

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
