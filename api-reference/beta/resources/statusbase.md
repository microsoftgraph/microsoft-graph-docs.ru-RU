---
title: тип ресурса statusBase
description: Описывает состояние события сводки по подготовкам.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3e100c1b86c8d299a7d74431715a6e9ef1464393
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231982"
---
# <a name="statusbase-resource-type-deprecated"></a><span data-ttu-id="3a761-103">тип ресурса statusBase (неподготовленный)</span><span class="sxs-lookup"><span data-stu-id="3a761-103">statusBase resource type (deprecated)</span></span>

<span data-ttu-id="3a761-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a761-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
>[!CAUTION] 
> <span data-ttu-id="3a761-105">API statusBase обесценилось и прекратит возвращать данные om 31 декабря 2021 г.</span><span class="sxs-lookup"><span data-stu-id="3a761-105">The statusBase API is deprecated and will stop returning data om December 31, 2021.</span></span> <span data-ttu-id="3a761-106">Используйте новый [тип provisioningStatusInfo.](provisioningstatusinfo.md)</span><span class="sxs-lookup"><span data-stu-id="3a761-106">Please use the new [provisioningStatusInfo](provisioningstatusinfo.md) type.</span></span>

<span data-ttu-id="3a761-107">Описывает состояние события сводки по подготовкам.</span><span class="sxs-lookup"><span data-stu-id="3a761-107">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="3a761-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a761-108">Properties</span></span>

| <span data-ttu-id="3a761-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a761-109">Property</span></span>     | <span data-ttu-id="3a761-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3a761-110">Type</span></span>        | <span data-ttu-id="3a761-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3a761-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3a761-112">status</span><span class="sxs-lookup"><span data-stu-id="3a761-112">status</span></span>|<span data-ttu-id="3a761-113">provisioningResult</span><span class="sxs-lookup"><span data-stu-id="3a761-113">provisioningResult</span></span>| <span data-ttu-id="3a761-114">Возможные значения: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3a761-114">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a761-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a761-115">JSON representation</span></span>

<span data-ttu-id="3a761-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a761-116">The following is a JSON representation of the resource.</span></span>

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


