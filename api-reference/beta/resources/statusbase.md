---
title: Тип ресурса Статусбасе
description: Описывает состояние сводного события подготовки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3afd7ea4e48c3f4c12a211c32278affea5d64b6b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411907"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="105cf-103">Тип ресурса Статусбасе</span><span class="sxs-lookup"><span data-stu-id="105cf-103">statusBase resource type</span></span>

<span data-ttu-id="105cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="105cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="105cf-105">Описывает состояние сводного события подготовки.</span><span class="sxs-lookup"><span data-stu-id="105cf-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="105cf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="105cf-106">Properties</span></span>

| <span data-ttu-id="105cf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="105cf-107">Property</span></span>     | <span data-ttu-id="105cf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="105cf-108">Type</span></span>        | <span data-ttu-id="105cf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="105cf-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="105cf-110">status</span><span class="sxs-lookup"><span data-stu-id="105cf-110">status</span></span>|<span data-ttu-id="105cf-111">String</span><span class="sxs-lookup"><span data-stu-id="105cf-111">String</span></span>| <span data-ttu-id="105cf-112">Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="105cf-112">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="105cf-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="105cf-113">JSON representation</span></span>

<span data-ttu-id="105cf-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="105cf-114">The following is a JSON representation of the resource.</span></span>

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
