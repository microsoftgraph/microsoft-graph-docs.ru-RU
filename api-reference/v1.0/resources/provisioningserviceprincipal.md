---
title: тип ресурса provisioningServicePrincipal
description: Представляет принцип службы, используемый для обеспечения.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 0a16985c398bb18058c11ac81d7fed3d5b468208
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241556"
---
# <a name="provisioningserviceprincipal-resource-type"></a><span data-ttu-id="2f4aa-103">тип ресурса provisioningServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="2f4aa-103">provisioningServicePrincipal resource type</span></span>

<span data-ttu-id="2f4aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f4aa-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="2f4aa-105">Представляет принцип службы, используемый для обеспечения.</span><span class="sxs-lookup"><span data-stu-id="2f4aa-105">Represents the service principal used for provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="2f4aa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f4aa-106">Properties</span></span>

| <span data-ttu-id="2f4aa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f4aa-107">Property</span></span>     | <span data-ttu-id="2f4aa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2f4aa-108">Type</span></span>        | <span data-ttu-id="2f4aa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2f4aa-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2f4aa-110">id</span><span class="sxs-lookup"><span data-stu-id="2f4aa-110">id</span></span>|<span data-ttu-id="2f4aa-111">Строка</span><span class="sxs-lookup"><span data-stu-id="2f4aa-111">String</span></span>|<span data-ttu-id="2f4aa-112">Уникально определяет **службуPrincipal, используемую** для предварительного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="2f4aa-112">Uniquely identifies the **servicePrincipal** used for provisioning.</span></span>|
|<span data-ttu-id="2f4aa-113">name</span><span class="sxs-lookup"><span data-stu-id="2f4aa-113">name</span></span>|<span data-ttu-id="2f4aa-114">String</span><span class="sxs-lookup"><span data-stu-id="2f4aa-114">String</span></span>| <span data-ttu-id="2f4aa-115">Имя, определенное клиентом **для службыPrincipal.**</span><span class="sxs-lookup"><span data-stu-id="2f4aa-115">Customer-defined name for the **servicePrincipal**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f4aa-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2f4aa-116">JSON representation</span></span>

<span data-ttu-id="2f4aa-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f4aa-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningServicePrincipal",
  "baseType": null
}-->

```json
{
  "id": "String",
  "name": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


