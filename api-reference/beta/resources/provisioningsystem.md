---
title: тип ресурсов provisioningSystem
description: Представляет систему, в которую пользователь был предварительно или из нее.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 2dcc52e4b847648477313d61c8b69b168a8807b1
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232983"
---
# <a name="provisioningsystem-resource-type"></a><span data-ttu-id="c156e-103">тип ресурсов provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="c156e-103">provisioningSystem resource type</span></span>

<span data-ttu-id="c156e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c156e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c156e-105">Представляет систему, в которую пользователь был предварительно или из нее.</span><span class="sxs-lookup"><span data-stu-id="c156e-105">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="c156e-106">Например, при предоставлении пользователю Azure Active Directory (Azure AD) в ServiceNow, источником системы является Azure AD, а целевой системой является ServiceNow.</span><span class="sxs-lookup"><span data-stu-id="c156e-106">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="c156e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c156e-107">Properties</span></span>

| <span data-ttu-id="c156e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c156e-108">Property</span></span>     | <span data-ttu-id="c156e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c156e-109">Type</span></span>        | <span data-ttu-id="c156e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c156e-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c156e-111">подробности</span><span class="sxs-lookup"><span data-stu-id="c156e-111">details</span></span>|[<span data-ttu-id="c156e-112">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="c156e-112">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="c156e-113">Сведения о системе.</span><span class="sxs-lookup"><span data-stu-id="c156e-113">Details of the system.</span></span>|
|<span data-ttu-id="c156e-114">displayName</span><span class="sxs-lookup"><span data-stu-id="c156e-114">displayName</span></span>|<span data-ttu-id="c156e-115">String</span><span class="sxs-lookup"><span data-stu-id="c156e-115">String</span></span>|<span data-ttu-id="c156e-116">Имя системы, в которую пользователь был предварительно или из нее.</span><span class="sxs-lookup"><span data-stu-id="c156e-116">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="c156e-117">id</span><span class="sxs-lookup"><span data-stu-id="c156e-117">id</span></span>|<span data-ttu-id="c156e-118">String</span><span class="sxs-lookup"><span data-stu-id="c156e-118">String</span></span>|<span data-ttu-id="c156e-119">Идентификатор системы, в которую пользователь был предварительно или из нее.</span><span class="sxs-lookup"><span data-stu-id="c156e-119">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c156e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c156e-120">JSON representation</span></span>

<span data-ttu-id="c156e-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c156e-121">The following is a JSON representation of the resource.</span></span>

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


