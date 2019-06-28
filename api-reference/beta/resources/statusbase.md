---
title: Тип ресурса Статусбасе
description: Описывает состояние сводного события подготовки.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: de35e89b674130bb1f2896b299ba5f4efe3af099
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349453"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="670e9-103">Тип ресурса Статусбасе</span><span class="sxs-lookup"><span data-stu-id="670e9-103">statusBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="670e9-104">Описывает состояние сводного события подготовки.</span><span class="sxs-lookup"><span data-stu-id="670e9-104">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="670e9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="670e9-105">Properties</span></span>

| <span data-ttu-id="670e9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="670e9-106">Property</span></span>     | <span data-ttu-id="670e9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="670e9-107">Type</span></span>        | <span data-ttu-id="670e9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="670e9-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="670e9-109">status</span><span class="sxs-lookup"><span data-stu-id="670e9-109">status</span></span>|<span data-ttu-id="670e9-110">String</span><span class="sxs-lookup"><span data-stu-id="670e9-110">String</span></span>| <span data-ttu-id="670e9-111">Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="670e9-111">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="670e9-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="670e9-112">JSON representation</span></span>

<span data-ttu-id="670e9-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="670e9-113">The following is a JSON representation of the resource.</span></span>

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
