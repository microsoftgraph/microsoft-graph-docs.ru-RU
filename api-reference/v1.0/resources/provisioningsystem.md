---
title: тип ресурсов provisioningSystem
description: Представляет систему, в которую пользователь был предварительно или из нее.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d52429fbaa641b1ee0be5208ddf7d85e0830b6c6
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241544"
---
# <a name="provisioningsystem-resource-type"></a><span data-ttu-id="4a975-103">тип ресурсов provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="4a975-103">provisioningSystem resource type</span></span>

<span data-ttu-id="4a975-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a975-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="4a975-105">Представляет систему, в которую пользователь был предварительно или из нее.</span><span class="sxs-lookup"><span data-stu-id="4a975-105">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="4a975-106">Например, при предоставлении пользователю Azure Active Directory (Azure AD) в ServiceNow, источником системы является Azure AD, а целевой системой является ServiceNow.</span><span class="sxs-lookup"><span data-stu-id="4a975-106">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="4a975-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a975-107">Properties</span></span>

| <span data-ttu-id="4a975-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a975-108">Property</span></span>     | <span data-ttu-id="4a975-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4a975-109">Type</span></span>        | <span data-ttu-id="4a975-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4a975-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a975-111">подробности</span><span class="sxs-lookup"><span data-stu-id="4a975-111">details</span></span>|[<span data-ttu-id="4a975-112">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="4a975-112">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="4a975-113">Сведения о системе.</span><span class="sxs-lookup"><span data-stu-id="4a975-113">Details of the system.</span></span>|
|<span data-ttu-id="4a975-114">displayName</span><span class="sxs-lookup"><span data-stu-id="4a975-114">displayName</span></span>|<span data-ttu-id="4a975-115">Строка</span><span class="sxs-lookup"><span data-stu-id="4a975-115">String</span></span>|<span data-ttu-id="4a975-116">Имя системы, в которую пользователь был предварительно или из нее.</span><span class="sxs-lookup"><span data-stu-id="4a975-116">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="4a975-117">id</span><span class="sxs-lookup"><span data-stu-id="4a975-117">id</span></span>|<span data-ttu-id="4a975-118">Строка</span><span class="sxs-lookup"><span data-stu-id="4a975-118">String</span></span>|<span data-ttu-id="4a975-119">Идентификатор системы, в которую пользователь был предварительно или из нее.</span><span class="sxs-lookup"><span data-stu-id="4a975-119">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a975-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4a975-120">JSON representation</span></span>

<span data-ttu-id="4a975-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a975-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningSystem",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningSystem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


