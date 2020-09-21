---
title: Тип ресурса Статусбасе
description: Описывает состояние сводного события подготовки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ee205db24cf8591725ca7d9fc3c4a0fe8c72489e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067106"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="82819-103">Тип ресурса Статусбасе</span><span class="sxs-lookup"><span data-stu-id="82819-103">statusBase resource type</span></span>

<span data-ttu-id="82819-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82819-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82819-105">Описывает состояние сводного события подготовки.</span><span class="sxs-lookup"><span data-stu-id="82819-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="82819-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="82819-106">Properties</span></span>

| <span data-ttu-id="82819-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="82819-107">Property</span></span>     | <span data-ttu-id="82819-108">Тип</span><span class="sxs-lookup"><span data-stu-id="82819-108">Type</span></span>        | <span data-ttu-id="82819-109">Описание</span><span class="sxs-lookup"><span data-stu-id="82819-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="82819-110">status</span><span class="sxs-lookup"><span data-stu-id="82819-110">status</span></span>|<span data-ttu-id="82819-111">String</span><span class="sxs-lookup"><span data-stu-id="82819-111">String</span></span>| <span data-ttu-id="82819-112">Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="82819-112">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="82819-113">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="82819-113">JSON representation</span></span>

<span data-ttu-id="82819-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82819-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusBase",
  "baseType": null
}-->

```json
{
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


