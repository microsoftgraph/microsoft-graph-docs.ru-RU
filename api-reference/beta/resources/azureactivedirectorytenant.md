---
title: тип ресурса azureActiveDirectoryTenant
description: Тип azureActiveDirectoryTenant определяет другого клиента Azure Active Directory в качестве источника удостоверений для связанной организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: acd59c82f1968cbb161b74d1e7c1a551b6b2e397
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759911"
---
# <a name="azureactivedirectorytenant-resource-type"></a><span data-ttu-id="f6040-103">тип ресурса azureActiveDirectoryTenant</span><span class="sxs-lookup"><span data-stu-id="f6040-103">azureActiveDirectoryTenant resource type</span></span>

<span data-ttu-id="f6040-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6040-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6040-105">Используется в источниках удостоверений [подключеннойорганизации.](connectedOrganization.md)</span><span class="sxs-lookup"><span data-stu-id="f6040-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="f6040-106">Это значение указывает, что этот тип определяет другого клиента Azure Active Directory в качестве источника удостоверений `@odata.type` `#microsoft.graph.azureActiveDirectoryTenant` для связанной организации.</span><span class="sxs-lookup"><span data-stu-id="f6040-106">The `@odata.type` value `#microsoft.graph.azureActiveDirectoryTenant` indicates that this type identifies another Azure Active Directory tenant as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="f6040-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6040-107">Properties</span></span>

| <span data-ttu-id="f6040-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6040-108">Property</span></span>                     | <span data-ttu-id="f6040-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f6040-109">Type</span></span>                      | <span data-ttu-id="f6040-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f6040-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="f6040-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f6040-111">displayName</span></span> |<span data-ttu-id="f6040-112">String</span><span class="sxs-lookup"><span data-stu-id="f6040-112">String</span></span> | <span data-ttu-id="f6040-113">Имя клиента Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f6040-113">The name of the Azure Active Directory tenant.</span></span> <span data-ttu-id="f6040-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6040-114">Read only.</span></span> |
| <span data-ttu-id="f6040-115">tenantId</span><span class="sxs-lookup"><span data-stu-id="f6040-115">tenantId</span></span> |<span data-ttu-id="f6040-116">String</span><span class="sxs-lookup"><span data-stu-id="f6040-116">String</span></span> | <span data-ttu-id="f6040-117">ID клиента Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f6040-117">The ID of the Azure Active Directory tenant.</span></span> <span data-ttu-id="f6040-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6040-118">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f6040-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="f6040-119">Relationships</span></span>

<span data-ttu-id="f6040-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f6040-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6040-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f6040-121">JSON representation</span></span>

<span data-ttu-id="f6040-122">Ниже приводится представление JSON этого типа.</span><span class="sxs-lookup"><span data-stu-id="f6040-122">The following is a JSON representation of the type.</span></span>

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


