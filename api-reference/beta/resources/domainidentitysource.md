---
title: тип ресурса domainIdentitySource
description: Тип domainIdentitySource определяет домен, не связанный с клиентом, в качестве источника удостоверений для связанной организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2c558213b7198da65eaacdbf0ac42915f3638c56
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896174"
---
# <a name="domainidentitysource-resource-type"></a><span data-ttu-id="05478-103">тип ресурса domainIdentitySource</span><span class="sxs-lookup"><span data-stu-id="05478-103">domainIdentitySource resource type</span></span>

<span data-ttu-id="05478-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05478-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05478-105">Используется в источниках удостоверений [подключеннойорганизации.](connectedOrganization.md)</span><span class="sxs-lookup"><span data-stu-id="05478-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="05478-106">Это значение указывает на то, что этот тип определяет домен как источник удостоверений `@odata.type` `#microsoft.graph.domainIdentitySource` для связанной организации.</span><span class="sxs-lookup"><span data-stu-id="05478-106">The `@odata.type` value `#microsoft.graph.domainIdentitySource` indicates that this type identifies a domain as an identity source for a connected organization.</span></span>

<span data-ttu-id="05478-107">При [](../api/connectedorganization-post.md)создании новой подключеннойорганизации, если вызывающий вызов предоставляет в коллекции identitySources домен DomainIdentitySource и домен соответствует зарегистрированным доменам клиента Azure Active Directory, то создаемая подключеннаяорганизация будет иметь коллекцию identitySources, содержащую одного члена типа [azureActiveDirectoryTenant.](azureactivedirectorytenant.md)</span><span class="sxs-lookup"><span data-stu-id="05478-107">When [creating a new connectedOrganization](../api/connectedorganization-post.md), if the caller provides in the identitySources collection a domainIdentitySource and the domain corresponds to a registered domain of an Azure Active Directory tenant, then the resulting connectedOrganization that is created will have an identitySources collection containing a single member of the [azureActiveDirectoryTenant](azureactivedirectorytenant.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="05478-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="05478-108">Properties</span></span>

| <span data-ttu-id="05478-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="05478-109">Property</span></span>                     | <span data-ttu-id="05478-110">Тип</span><span class="sxs-lookup"><span data-stu-id="05478-110">Type</span></span>                      | <span data-ttu-id="05478-111">Описание</span><span class="sxs-lookup"><span data-stu-id="05478-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="05478-112">displayName</span><span class="sxs-lookup"><span data-stu-id="05478-112">displayName</span></span> |<span data-ttu-id="05478-113">String</span><span class="sxs-lookup"><span data-stu-id="05478-113">String</span></span> | <span data-ttu-id="05478-114">Имя источника удостоверений, как правило, также доменное имя.</span><span class="sxs-lookup"><span data-stu-id="05478-114">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="05478-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="05478-115">Read only.</span></span> |
| <span data-ttu-id="05478-116">domainName</span><span class="sxs-lookup"><span data-stu-id="05478-116">domainName</span></span> |<span data-ttu-id="05478-117">String</span><span class="sxs-lookup"><span data-stu-id="05478-117">String</span></span> | <span data-ttu-id="05478-118">Доменное имя.</span><span class="sxs-lookup"><span data-stu-id="05478-118">The domain name.</span></span> <span data-ttu-id="05478-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="05478-119">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="05478-120">Связи</span><span class="sxs-lookup"><span data-stu-id="05478-120">Relationships</span></span>

<span data-ttu-id="05478-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="05478-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05478-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="05478-122">JSON representation</span></span>

<span data-ttu-id="05478-123">Ниже приводится представление JSON этого типа.</span><span class="sxs-lookup"><span data-stu-id="05478-123">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainIdentitySource",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainIdentitySource resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


