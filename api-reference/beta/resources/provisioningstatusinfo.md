---
title: provisioningStatusInfo resource type
description: Описывает состояние события сводки по подготовкам.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 669201b5527160da6b903614523d633a8c11cb1d
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232989"
---
# <a name="provisioningstatusinfo-resource-type"></a><span data-ttu-id="3259c-103">provisioningStatusInfo resource type</span><span class="sxs-lookup"><span data-stu-id="3259c-103">provisioningStatusInfo resource type</span></span>

<span data-ttu-id="3259c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3259c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3259c-105">Описывает состояние события сводки по подготовкам.</span><span class="sxs-lookup"><span data-stu-id="3259c-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="3259c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3259c-106">Properties</span></span>

| <span data-ttu-id="3259c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3259c-107">Property</span></span>     | <span data-ttu-id="3259c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3259c-108">Type</span></span>        | <span data-ttu-id="3259c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3259c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3259c-110">status</span><span class="sxs-lookup"><span data-stu-id="3259c-110">status</span></span>|<span data-ttu-id="3259c-111">String</span><span class="sxs-lookup"><span data-stu-id="3259c-111">String</span></span>| <span data-ttu-id="3259c-112">Возможные значения: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3259c-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3259c-113">errorInfo</span><span class="sxs-lookup"><span data-stu-id="3259c-113">errorInfo</span></span>|[<span data-ttu-id="3259c-114">provisioningErrorInfo</span><span class="sxs-lookup"><span data-stu-id="3259c-114">provisioningErrorInfo</span></span>](provisioningerrorinfo.md)| <span data-ttu-id="3259c-115">Если состояние не успешно или пропущенные сведения об ошибке содержатся в этом.</span><span class="sxs-lookup"><span data-stu-id="3259c-115">If status is not success/ skipped details for the error are contained in this.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3259c-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3259c-116">JSON representation</span></span>

<span data-ttu-id="3259c-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3259c-117">The following is a JSON representation of the resource.</span></span>

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


