---
title: provisioningStatusInfo resource type
description: Описывает состояние события сводки по подготовкам.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7ab2a67662f6e03fd7f967757a7de7ec92480826
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682070"
---
# <a name="provisioningstatusinfo-resource-type"></a><span data-ttu-id="90d31-103">provisioningStatusInfo resource type</span><span class="sxs-lookup"><span data-stu-id="90d31-103">provisioningStatusInfo resource type</span></span>

<span data-ttu-id="90d31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90d31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90d31-105">Описывает состояние события сводки по подготовкам.</span><span class="sxs-lookup"><span data-stu-id="90d31-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="90d31-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="90d31-106">Properties</span></span>

| <span data-ttu-id="90d31-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="90d31-107">Property</span></span>     | <span data-ttu-id="90d31-108">Тип</span><span class="sxs-lookup"><span data-stu-id="90d31-108">Type</span></span>        | <span data-ttu-id="90d31-109">Описание</span><span class="sxs-lookup"><span data-stu-id="90d31-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="90d31-110">status</span><span class="sxs-lookup"><span data-stu-id="90d31-110">status</span></span>|<span data-ttu-id="90d31-111">String</span><span class="sxs-lookup"><span data-stu-id="90d31-111">String</span></span>| <span data-ttu-id="90d31-112">Возможные значения: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="90d31-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="90d31-113">errorInfo</span><span class="sxs-lookup"><span data-stu-id="90d31-113">errorInfo</span></span>|[<span data-ttu-id="90d31-114">provisioningErrorInfo</span><span class="sxs-lookup"><span data-stu-id="90d31-114">provisioningErrorInfo</span></span>](provisioningerrorinfo.md)| <span data-ttu-id="90d31-115">Если состояние не успешно или пропущенные сведения об ошибке содержатся в этом.</span><span class="sxs-lookup"><span data-stu-id="90d31-115">If status is not success/ skipped details for the error are contained in this.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90d31-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90d31-116">JSON representation</span></span>

<span data-ttu-id="90d31-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90d31-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStatusInfo",
  "baseType": null
}-->

```json
{
  "status": "String",
  "errorinfo": {"@odata.type": "microsoft.graph.provisioningErrorInfo"},}
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


