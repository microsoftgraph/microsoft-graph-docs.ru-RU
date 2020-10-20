---
title: Тип ресурса Сервицеендпоинт
description: Тип Сервицеендпоинт
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b650b2f105a9feb2d33327a0ceef9add18716d00
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601568"
---
# <a name="serviceendpoint-resource-type"></a><span data-ttu-id="eebbb-103">Тип ресурса Сервицеендпоинт</span><span class="sxs-lookup"><span data-stu-id="eebbb-103">serviceEndpoint resource type</span></span>

<span data-ttu-id="eebbb-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="eebbb-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="eebbb-105">Представляет конечную точку службы в вызове.</span><span class="sxs-lookup"><span data-stu-id="eebbb-105">Represents a service endpoint in a call.</span></span> <span data-ttu-id="eebbb-106">Конечная точка представляет вызывающий медиа сервер или другой объект службы.</span><span class="sxs-lookup"><span data-stu-id="eebbb-106">The endpoint represents a calling media server or other service entity.</span></span> <span data-ttu-id="eebbb-107">Наследуется от типа [конечной точки](callrecords-endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="eebbb-107">Inherits from [endpoint](callrecords-endpoint.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="eebbb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eebbb-108">Properties</span></span>

| <span data-ttu-id="eebbb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eebbb-109">Property</span></span>     | <span data-ttu-id="eebbb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eebbb-110">Type</span></span>        | <span data-ttu-id="eebbb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eebbb-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eebbb-112">userAgent</span><span class="sxs-lookup"><span data-stu-id="eebbb-112">userAgent</span></span>|[<span data-ttu-id="eebbb-113">Microsoft. Graph. Каллрекордс. userAgent</span><span class="sxs-lookup"><span data-stu-id="eebbb-113">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="eebbb-114">Пользователь — агент, указанный этой конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="eebbb-114">User-agent reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eebbb-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eebbb-115">JSON representation</span></span>

<span data-ttu-id="eebbb-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eebbb-116">The following is a JSON representation of the resource.</span></span>

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
