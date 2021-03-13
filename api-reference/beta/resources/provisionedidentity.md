---
title: тип ресурса provisionedIdentity
description: Описывает удостоверение, связанное с сводным событием объекта подготовка.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 2de68bdce990a6a541a5c284672541669cfdebea
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761109"
---
# <a name="provisionedidentity-resource-type"></a><span data-ttu-id="50982-103">тип ресурса provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="50982-103">provisionedIdentity resource type</span></span>

<span data-ttu-id="50982-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50982-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50982-105">Описывает удостоверение, связанное с сводным событием объекта подготовка.</span><span class="sxs-lookup"><span data-stu-id="50982-105">Describes the identity associated with the provisioning object summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="50982-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="50982-106">Properties</span></span>

| <span data-ttu-id="50982-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="50982-107">Property</span></span>     | <span data-ttu-id="50982-108">Тип</span><span class="sxs-lookup"><span data-stu-id="50982-108">Type</span></span>        | <span data-ttu-id="50982-109">Описание</span><span class="sxs-lookup"><span data-stu-id="50982-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="50982-110">подробности</span><span class="sxs-lookup"><span data-stu-id="50982-110">details</span></span>|[<span data-ttu-id="50982-111">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="50982-111">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="50982-112">Сведения о удостоверении.</span><span class="sxs-lookup"><span data-stu-id="50982-112">Details of the identity.</span></span>|
|<span data-ttu-id="50982-113">displayName</span><span class="sxs-lookup"><span data-stu-id="50982-113">displayName</span></span>|<span data-ttu-id="50982-114">String</span><span class="sxs-lookup"><span data-stu-id="50982-114">String</span></span>|<span data-ttu-id="50982-115">Отображение имени удостоверения.</span><span class="sxs-lookup"><span data-stu-id="50982-115">Display name of the identity.</span></span> |
|<span data-ttu-id="50982-116">id</span><span class="sxs-lookup"><span data-stu-id="50982-116">id</span></span>|<span data-ttu-id="50982-117">String</span><span class="sxs-lookup"><span data-stu-id="50982-117">String</span></span>|<span data-ttu-id="50982-118">Уникально идентифицирует удостоверение.</span><span class="sxs-lookup"><span data-stu-id="50982-118">Uniquely identifies the identity.</span></span>|
|<span data-ttu-id="50982-119">identityType</span><span class="sxs-lookup"><span data-stu-id="50982-119">identityType</span></span>|<span data-ttu-id="50982-120">String</span><span class="sxs-lookup"><span data-stu-id="50982-120">String</span></span>|<span data-ttu-id="50982-121">Тип предварительного удостоверения, например "пользователь" или "группа".</span><span class="sxs-lookup"><span data-stu-id="50982-121">Type of identity that has been provisioned, such as 'user' or 'group'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50982-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50982-122">JSON representation</span></span>

<span data-ttu-id="50982-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50982-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedIdentity",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String",
  "identityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


