---
title: тип ресурса azureActiveDirectoryTenant
description: Тип azureActiveDirectoryTenant определяет другого клиента Azure Active Directory как источник удостоверений для связанной организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d7a36c8c737866b20585518e1dc34e6944c97885
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896587"
---
# <a name="azureactivedirectorytenant-resource-type"></a><span data-ttu-id="d9909-103">тип ресурса azureActiveDirectoryTenant</span><span class="sxs-lookup"><span data-stu-id="d9909-103">azureActiveDirectoryTenant resource type</span></span>

<span data-ttu-id="d9909-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9909-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9909-105">Используется в источниках удостоверений [подключеннойорганизации.](connectedOrganization.md)</span><span class="sxs-lookup"><span data-stu-id="d9909-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="d9909-106">Это значение указывает, что этот тип определяет другого клиента Azure Active Directory как источник удостоверений `@odata.type` `#microsoft.graph.azureActiveDirectoryTenant` для связанной организации.</span><span class="sxs-lookup"><span data-stu-id="d9909-106">The `@odata.type` value `#microsoft.graph.azureActiveDirectoryTenant` indicates that this type identifies another Azure Active Directory tenant as an identity source for a connected organization.</span></span>

<span data-ttu-id="d9909-107">При [](../api/connectedorganization-post.md)создании новой подключеннойорганизации, если вызывающий вызов предоставляет в коллекции identitySources домен DomainIdentitySource и домен соответствует зарегистрированным доменам клиента Azure Active Directory, то создаемая подключеннаяорганизация будет иметь коллекцию identitySources, содержащую одного члена типа [azureActiveDirectoryTenant.](azureactivedirectorytenant.md)</span><span class="sxs-lookup"><span data-stu-id="d9909-107">When [creating a new connectedOrganization](../api/connectedorganization-post.md), if the caller provides in the identitySources collection a domainIdentitySource and the domain corresponds to a registered domain of an Azure Active Directory tenant, then the resulting connectedOrganization that is created will have an identitySources collection containing a single member of the [azureActiveDirectoryTenant](azureactivedirectorytenant.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="d9909-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9909-108">Properties</span></span>

| <span data-ttu-id="d9909-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9909-109">Property</span></span>                     | <span data-ttu-id="d9909-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d9909-110">Type</span></span>                      | <span data-ttu-id="d9909-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d9909-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="d9909-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d9909-112">displayName</span></span> |<span data-ttu-id="d9909-113">String</span><span class="sxs-lookup"><span data-stu-id="d9909-113">String</span></span> | <span data-ttu-id="d9909-114">Имя клиента Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d9909-114">The name of the Azure Active Directory tenant.</span></span> <span data-ttu-id="d9909-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9909-115">Read only.</span></span> |
| <span data-ttu-id="d9909-116">tenantId</span><span class="sxs-lookup"><span data-stu-id="d9909-116">tenantId</span></span> |<span data-ttu-id="d9909-117">String</span><span class="sxs-lookup"><span data-stu-id="d9909-117">String</span></span> | <span data-ttu-id="d9909-118">ID клиента Azure Active Directory клиента.</span><span class="sxs-lookup"><span data-stu-id="d9909-118">The ID of the Azure Active Directory tenant.</span></span> <span data-ttu-id="d9909-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9909-119">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d9909-120">Связи</span><span class="sxs-lookup"><span data-stu-id="d9909-120">Relationships</span></span>

<span data-ttu-id="d9909-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d9909-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9909-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d9909-122">JSON representation</span></span>

<span data-ttu-id="d9909-123">Ниже приводится представление JSON этого типа.</span><span class="sxs-lookup"><span data-stu-id="d9909-123">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "tenantId": "String (identifier)",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "azureActiveDirectoryTenant resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


