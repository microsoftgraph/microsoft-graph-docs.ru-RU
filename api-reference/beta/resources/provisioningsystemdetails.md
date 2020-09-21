---
title: Тип ресурса Провисионингсистемдетаилс
description: Представляет систему, в которую были подготовлены пользователи.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6880214614047000fcc5a793faf4be3e5a88a5e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026448"
---
# <a name="provisioningsystemdetails-resource-type"></a><span data-ttu-id="4e140-103">Тип ресурса Провисионингсистемдетаилс</span><span class="sxs-lookup"><span data-stu-id="4e140-103">provisioningSystemDetails resource type</span></span>

<span data-ttu-id="4e140-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e140-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e140-105">Представляет систему, в которую были подготовлены пользователи.</span><span class="sxs-lookup"><span data-stu-id="4e140-105">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="4e140-106">Например, при подготовке пользователя из Azure Active Directory (Azure AD) к ServiceNow система является системой Azure AD, а целевой системой является ServiceNow.</span><span class="sxs-lookup"><span data-stu-id="4e140-106">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="4e140-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e140-107">Properties</span></span>

| <span data-ttu-id="4e140-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e140-108">Property</span></span>     | <span data-ttu-id="4e140-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4e140-109">Type</span></span>        | <span data-ttu-id="4e140-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4e140-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4e140-111">details</span><span class="sxs-lookup"><span data-stu-id="4e140-111">details</span></span>|[<span data-ttu-id="4e140-112">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="4e140-112">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="4e140-113">Сведения о системе.</span><span class="sxs-lookup"><span data-stu-id="4e140-113">Details of the system.</span></span>|
|<span data-ttu-id="4e140-114">displayName</span><span class="sxs-lookup"><span data-stu-id="4e140-114">displayName</span></span>|<span data-ttu-id="4e140-115">String</span><span class="sxs-lookup"><span data-stu-id="4e140-115">String</span></span>|<span data-ttu-id="4e140-116">Имя системы, в которую были подготовлены пользователи.</span><span class="sxs-lookup"><span data-stu-id="4e140-116">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="4e140-117">id</span><span class="sxs-lookup"><span data-stu-id="4e140-117">id</span></span>|<span data-ttu-id="4e140-118">String</span><span class="sxs-lookup"><span data-stu-id="4e140-118">String</span></span>|<span data-ttu-id="4e140-119">Идентификатор системы, в которую были подготовлены пользователи.</span><span class="sxs-lookup"><span data-stu-id="4e140-119">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e140-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e140-120">JSON representation</span></span>

<span data-ttu-id="4e140-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e140-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningSystemDetails",
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
  "description": "provisioningSystemDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


