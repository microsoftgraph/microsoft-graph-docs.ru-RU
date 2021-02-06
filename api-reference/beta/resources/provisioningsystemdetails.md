---
title: Тип ресурса provisioningSystemDetails
description: Представляет систему, для которую пользователь был представлен или из нее.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5400088c1f239bd73e093679bbc13b8034800f28
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135340"
---
# <a name="provisioningsystemdetails-resource-type"></a><span data-ttu-id="d9038-103">Тип ресурса provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="d9038-103">provisioningSystemDetails resource type</span></span>

<span data-ttu-id="d9038-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9038-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9038-105">Представляет систему, для которую пользователь был представлен или из нее.</span><span class="sxs-lookup"><span data-stu-id="d9038-105">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="d9038-106">Например, при подготовка пользователя из Azure Active Directory (Azure AD) в ServiceNow, источником системы является Azure AD, а целевая система — ServiceNow.</span><span class="sxs-lookup"><span data-stu-id="d9038-106">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="d9038-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9038-107">Properties</span></span>

| <span data-ttu-id="d9038-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9038-108">Property</span></span>     | <span data-ttu-id="d9038-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d9038-109">Type</span></span>        | <span data-ttu-id="d9038-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d9038-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9038-111">details</span><span class="sxs-lookup"><span data-stu-id="d9038-111">details</span></span>|[<span data-ttu-id="d9038-112">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="d9038-112">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="d9038-113">Сведения о системе.</span><span class="sxs-lookup"><span data-stu-id="d9038-113">Details of the system.</span></span>|
|<span data-ttu-id="d9038-114">displayName</span><span class="sxs-lookup"><span data-stu-id="d9038-114">displayName</span></span>|<span data-ttu-id="d9038-115">Строка</span><span class="sxs-lookup"><span data-stu-id="d9038-115">String</span></span>|<span data-ttu-id="d9038-116">Имя системы, в которую или из нее был вошел пользователь.</span><span class="sxs-lookup"><span data-stu-id="d9038-116">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="d9038-117">id</span><span class="sxs-lookup"><span data-stu-id="d9038-117">id</span></span>|<span data-ttu-id="d9038-118">Строка</span><span class="sxs-lookup"><span data-stu-id="d9038-118">String</span></span>|<span data-ttu-id="d9038-119">Идентификатор системы, в которую или из нее был вошел пользователь.</span><span class="sxs-lookup"><span data-stu-id="d9038-119">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9038-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d9038-120">JSON representation</span></span>

<span data-ttu-id="d9038-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9038-121">The following is a JSON representation of the resource.</span></span>

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


