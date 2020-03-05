---
title: Тип ресурса Статусбасе
description: Описывает состояние сводного события подготовки.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b63290442f4faddf4bcd9e25c01ab564a7fcc94
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520326"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="5db4c-103">Тип ресурса Статусбасе</span><span class="sxs-lookup"><span data-stu-id="5db4c-103">statusBase resource type</span></span>

<span data-ttu-id="5db4c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5db4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5db4c-105">Описывает состояние сводного события подготовки.</span><span class="sxs-lookup"><span data-stu-id="5db4c-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="5db4c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5db4c-106">Properties</span></span>

| <span data-ttu-id="5db4c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5db4c-107">Property</span></span>     | <span data-ttu-id="5db4c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5db4c-108">Type</span></span>        | <span data-ttu-id="5db4c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5db4c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5db4c-110">status</span><span class="sxs-lookup"><span data-stu-id="5db4c-110">status</span></span>|<span data-ttu-id="5db4c-111">String</span><span class="sxs-lookup"><span data-stu-id="5db4c-111">String</span></span>| <span data-ttu-id="5db4c-112">Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5db4c-112">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5db4c-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5db4c-113">JSON representation</span></span>

<span data-ttu-id="5db4c-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5db4c-114">The following is a JSON representation of the resource.</span></span>

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
