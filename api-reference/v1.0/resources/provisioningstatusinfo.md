---
title: provisioningStatusInfo resource type
description: Описывает состояние события сводки по подготовкам.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 7b6ab84ab1139d2ec5d60e7d5c668d0444e472d3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680971"
---
# <a name="provisioningstatusinfo-resource-type"></a><span data-ttu-id="6c6b4-103">provisioningStatusInfo resource type</span><span class="sxs-lookup"><span data-stu-id="6c6b4-103">provisioningStatusInfo resource type</span></span>

<span data-ttu-id="6c6b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c6b4-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="6c6b4-105">Описывает состояние события сводки по подготовкам.</span><span class="sxs-lookup"><span data-stu-id="6c6b4-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="6c6b4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c6b4-106">Properties</span></span>

| <span data-ttu-id="6c6b4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c6b4-107">Property</span></span>     | <span data-ttu-id="6c6b4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6c6b4-108">Type</span></span>        | <span data-ttu-id="6c6b4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6c6b4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6c6b4-110">status</span><span class="sxs-lookup"><span data-stu-id="6c6b4-110">status</span></span>|<span data-ttu-id="6c6b4-111">provisioningResult</span><span class="sxs-lookup"><span data-stu-id="6c6b4-111">provisioningResult</span></span>| <span data-ttu-id="6c6b4-112">Возможные значения: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6c6b4-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6c6b4-113">errorInfo</span><span class="sxs-lookup"><span data-stu-id="6c6b4-113">errorInfo</span></span>|[<span data-ttu-id="6c6b4-114">provisioningErrorInfo</span><span class="sxs-lookup"><span data-stu-id="6c6b4-114">provisioningErrorInfo</span></span>](provisioningErrorInfo.md)| <span data-ttu-id="6c6b4-115">Если состояние не успешно или пропущенные сведения об ошибке содержатся в этом.</span><span class="sxs-lookup"><span data-stu-id="6c6b4-115">If status is not success/ skipped details for the error are contained in this.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c6b4-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c6b4-116">JSON representation</span></span>

<span data-ttu-id="6c6b4-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c6b4-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStatusInfo",
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
  "description": "provisioningStatusInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


