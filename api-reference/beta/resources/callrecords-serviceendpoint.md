---
title: Тип ресурса Сервицеендпоинт
description: Тип Сервицеендпоинт
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9fe86f55615c4e7d58a219f15bd9e6792e5ae72b
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394806"
---
# <a name="serviceendpoint-resource-type"></a><span data-ttu-id="61f3a-103">Тип ресурса Сервицеендпоинт</span><span class="sxs-lookup"><span data-stu-id="61f3a-103">serviceEndpoint resource type</span></span>

<span data-ttu-id="61f3a-104">Пространство имен: Microsoft. Graph. Каллрекордс</span><span class="sxs-lookup"><span data-stu-id="61f3a-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61f3a-105">Представляет конечную точку службы в вызове.</span><span class="sxs-lookup"><span data-stu-id="61f3a-105">Represents a service endpoint in a call.</span></span> <span data-ttu-id="61f3a-106">Конечная точка представляет вызывающий медиа сервер или другой объект службы.</span><span class="sxs-lookup"><span data-stu-id="61f3a-106">The endpoint represents a calling media server or other service entity.</span></span> <span data-ttu-id="61f3a-107">Наследуется от типа [конечной точки](callrecords-endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="61f3a-107">Inherits from [endpoint](callrecords-endpoint.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="61f3a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="61f3a-108">Properties</span></span>

| <span data-ttu-id="61f3a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="61f3a-109">Property</span></span>     | <span data-ttu-id="61f3a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="61f3a-110">Type</span></span>        | <span data-ttu-id="61f3a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="61f3a-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="61f3a-112">userAgent</span><span class="sxs-lookup"><span data-stu-id="61f3a-112">userAgent</span></span>|[<span data-ttu-id="61f3a-113">Microsoft. Graph. Каллрекордс. userAgent</span><span class="sxs-lookup"><span data-stu-id="61f3a-113">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="61f3a-114">Пользователь — агент, указанный этой конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="61f3a-114">User-agent reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61f3a-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61f3a-115">JSON representation</span></span>

<span data-ttu-id="61f3a-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61f3a-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.serviceEndpoint",
  "baseType": "microsoft.graph.callRecords.endpoint"
}-->

```json
{
  "userAgent": {"@odata.type": "microsoft.graph.callRecords.userAgent"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->