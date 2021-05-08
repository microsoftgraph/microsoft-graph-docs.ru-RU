---
title: тип ресурса provisionedIdentity
description: Описывает удостоверение, связанное с сводным событием объекта подготовка.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 083609787920d840d8576d1c2a7cd5e39945768c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241580"
---
# <a name="provisionedidentity-resource-type"></a><span data-ttu-id="d047c-103">тип ресурса provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="d047c-103">provisionedIdentity resource type</span></span>

<span data-ttu-id="d047c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d047c-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="d047c-105">Описывает удостоверение, связанное с сводным событием объекта подготовка.</span><span class="sxs-lookup"><span data-stu-id="d047c-105">Describes the identity associated with the provisioning object summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="d047c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d047c-106">Properties</span></span>

| <span data-ttu-id="d047c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d047c-107">Property</span></span>     | <span data-ttu-id="d047c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d047c-108">Type</span></span>        | <span data-ttu-id="d047c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d047c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d047c-110">подробности</span><span class="sxs-lookup"><span data-stu-id="d047c-110">details</span></span>|[<span data-ttu-id="d047c-111">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="d047c-111">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="d047c-112">Сведения о удостоверении.</span><span class="sxs-lookup"><span data-stu-id="d047c-112">Details of the identity.</span></span>|
|<span data-ttu-id="d047c-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d047c-113">displayName</span></span>|<span data-ttu-id="d047c-114">Строка</span><span class="sxs-lookup"><span data-stu-id="d047c-114">String</span></span>|<span data-ttu-id="d047c-115">Отображение имени удостоверения.</span><span class="sxs-lookup"><span data-stu-id="d047c-115">Display name of the identity.</span></span> |
|<span data-ttu-id="d047c-116">id</span><span class="sxs-lookup"><span data-stu-id="d047c-116">id</span></span>|<span data-ttu-id="d047c-117">Строка</span><span class="sxs-lookup"><span data-stu-id="d047c-117">String</span></span>|<span data-ttu-id="d047c-118">Уникально идентифицирует удостоверение.</span><span class="sxs-lookup"><span data-stu-id="d047c-118">Uniquely identifies the identity.</span></span>|
|<span data-ttu-id="d047c-119">identityType</span><span class="sxs-lookup"><span data-stu-id="d047c-119">identityType</span></span>|<span data-ttu-id="d047c-120">Строка</span><span class="sxs-lookup"><span data-stu-id="d047c-120">String</span></span>|<span data-ttu-id="d047c-121">Тип предварительного удостоверения, например "пользователь" или "группа".</span><span class="sxs-lookup"><span data-stu-id="d047c-121">Type of identity that has been provisioned, such as 'user' or 'group'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d047c-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d047c-122">JSON representation</span></span>

<span data-ttu-id="d047c-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d047c-123">The following is a JSON representation of the resource.</span></span>

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


