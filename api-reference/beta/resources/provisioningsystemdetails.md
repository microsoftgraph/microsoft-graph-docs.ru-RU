---
title: Тип ресурса Провисионингсистемдетаилс
description: Представляет систему, в которую были подготовлены пользователи.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e84af77ac7d2b14fb25ce07939bc1a542102fb19
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349447"
---
# <a name="provisioningsystemdetails-resource-type"></a><span data-ttu-id="b1117-103">Тип ресурса Провисионингсистемдетаилс</span><span class="sxs-lookup"><span data-stu-id="b1117-103">provisioningSystemDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1117-104">Представляет систему, в которую были подготовлены пользователи.</span><span class="sxs-lookup"><span data-stu-id="b1117-104">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="b1117-105">Например, при подготовке пользователя из Azure Active Directory (Azure AD) к ServiceNow система является системой Azure AD, а целевой системой является ServiceNow.</span><span class="sxs-lookup"><span data-stu-id="b1117-105">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="b1117-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1117-106">Properties</span></span>

| <span data-ttu-id="b1117-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1117-107">Property</span></span>     | <span data-ttu-id="b1117-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b1117-108">Type</span></span>        | <span data-ttu-id="b1117-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b1117-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1117-110">details</span><span class="sxs-lookup"><span data-stu-id="b1117-110">details</span></span>|[<span data-ttu-id="b1117-111">Детаилсинфо</span><span class="sxs-lookup"><span data-stu-id="b1117-111">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="b1117-112">Сведения о системе.</span><span class="sxs-lookup"><span data-stu-id="b1117-112">Details of the system.</span></span>|
|<span data-ttu-id="b1117-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b1117-113">displayName</span></span>|<span data-ttu-id="b1117-114">Строка</span><span class="sxs-lookup"><span data-stu-id="b1117-114">String</span></span>|<span data-ttu-id="b1117-115">Имя системы, в которую были подготовлены пользователи.</span><span class="sxs-lookup"><span data-stu-id="b1117-115">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="b1117-116">id</span><span class="sxs-lookup"><span data-stu-id="b1117-116">id</span></span>|<span data-ttu-id="b1117-117">String</span><span class="sxs-lookup"><span data-stu-id="b1117-117">String</span></span>|<span data-ttu-id="b1117-118">Идентификатор системы, в которую были подготовлены пользователи.</span><span class="sxs-lookup"><span data-stu-id="b1117-118">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1117-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1117-119">JSON representation</span></span>

<span data-ttu-id="b1117-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1117-120">The following is a JSON representation of the resource.</span></span>

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
