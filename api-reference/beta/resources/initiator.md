---
title: Тип ресурса инициатора
description: Описывает, кто и что инициировал событие предоставления.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 2aa8c3f365402569d7a9987d9152bae5e4e3c580
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130250"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="c54c7-103">Тип ресурса инициатора</span><span class="sxs-lookup"><span data-stu-id="c54c7-103">initiator resource type</span></span>

<span data-ttu-id="c54c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c54c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c54c7-105">Описывает, кто и что инициировал событие предоставления.</span><span class="sxs-lookup"><span data-stu-id="c54c7-105">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="c54c7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c54c7-106">Properties</span></span>

| <span data-ttu-id="c54c7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c54c7-107">Property</span></span>     | <span data-ttu-id="c54c7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c54c7-108">Type</span></span>        | <span data-ttu-id="c54c7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c54c7-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c54c7-110">displayName</span><span class="sxs-lookup"><span data-stu-id="c54c7-110">displayName</span></span>|<span data-ttu-id="c54c7-111">Строка</span><span class="sxs-lookup"><span data-stu-id="c54c7-111">String</span></span>|<span data-ttu-id="c54c7-112">Имя человека или службы, которая инициировала событие предоставления.</span><span class="sxs-lookup"><span data-stu-id="c54c7-112">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="c54c7-113">id</span><span class="sxs-lookup"><span data-stu-id="c54c7-113">id</span></span>|<span data-ttu-id="c54c7-114">Строка</span><span class="sxs-lookup"><span data-stu-id="c54c7-114">String</span></span>|<span data-ttu-id="c54c7-115">Уникально идентифицирует человека или службу, инициировали событие предоставления.</span><span class="sxs-lookup"><span data-stu-id="c54c7-115">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="c54c7-116">initiatorType</span><span class="sxs-lookup"><span data-stu-id="c54c7-116">initiatorType</span></span>|<span data-ttu-id="c54c7-117">Строка</span><span class="sxs-lookup"><span data-stu-id="c54c7-117">String</span></span>| <span data-ttu-id="c54c7-118">Тип инициатора.</span><span class="sxs-lookup"><span data-stu-id="c54c7-118">Type of initiator.</span></span> <span data-ttu-id="c54c7-119">Возможные значения: `user`, `app`, `system`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c54c7-119">Possible values are: `user`, `app`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c54c7-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c54c7-120">JSON representation</span></span>

<span data-ttu-id="c54c7-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c54c7-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


