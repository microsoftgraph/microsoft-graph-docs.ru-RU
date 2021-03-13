---
title: тип ресурса statusBase
description: Описывает состояние события сводки по подготовкам.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 951ef56ecbe2ff8c2ab9692e4eaa9ddf7811d959
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761025"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="499da-103">тип ресурса statusBase</span><span class="sxs-lookup"><span data-stu-id="499da-103">statusBase resource type</span></span>

<span data-ttu-id="499da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="499da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="499da-105">Описывает состояние события сводки по подготовкам.</span><span class="sxs-lookup"><span data-stu-id="499da-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="499da-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="499da-106">Properties</span></span>

| <span data-ttu-id="499da-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="499da-107">Property</span></span>     | <span data-ttu-id="499da-108">Тип</span><span class="sxs-lookup"><span data-stu-id="499da-108">Type</span></span>        | <span data-ttu-id="499da-109">Описание</span><span class="sxs-lookup"><span data-stu-id="499da-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="499da-110">status</span><span class="sxs-lookup"><span data-stu-id="499da-110">status</span></span>|<span data-ttu-id="499da-111">String</span><span class="sxs-lookup"><span data-stu-id="499da-111">String</span></span>| <span data-ttu-id="499da-112">Возможные значения: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="499da-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="499da-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="499da-113">JSON representation</span></span>

<span data-ttu-id="499da-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="499da-114">The following is a JSON representation of the resource.</span></span>

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


