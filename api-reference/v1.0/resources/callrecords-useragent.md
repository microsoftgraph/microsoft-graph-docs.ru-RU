---
title: Тип ресурса userAgent
description: Тип userAgent
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 55db3bcfc00c54cb51f552624a9e2c51fcce5a7b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601456"
---
# <a name="useragent-resource-type"></a><span data-ttu-id="c4f52-103">Тип ресурса userAgent</span><span class="sxs-lookup"><span data-stu-id="c4f52-103">userAgent resource type</span></span>

<span data-ttu-id="c4f52-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="c4f52-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="c4f52-105">Представляет агента пользователя конечной точки в вызове.</span><span class="sxs-lookup"><span data-stu-id="c4f52-105">Represents the user agent of an endpoint in a call.</span></span>
<span data-ttu-id="c4f52-106">Типы [клиентусеражент](callrecords-clientuseragent.md) и [сервицеусеражент](callrecords-serviceuseragent.md)) наследуются от этого типа.</span><span class="sxs-lookup"><span data-stu-id="c4f52-106">The [clientUserAgent](callrecords-clientuseragent.md) and [serviceUserAgent](callrecords-serviceuseragent.md)) types inherit from this type.</span></span>

## <a name="properties"></a><span data-ttu-id="c4f52-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4f52-107">Properties</span></span>

| <span data-ttu-id="c4f52-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4f52-108">Property</span></span>     | <span data-ttu-id="c4f52-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c4f52-109">Type</span></span>        | <span data-ttu-id="c4f52-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c4f52-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c4f52-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="c4f52-111">applicationVersion</span></span>|<span data-ttu-id="c4f52-112">String</span><span class="sxs-lookup"><span data-stu-id="c4f52-112">String</span></span>|<span data-ttu-id="c4f52-113">Определяет версию программного обеспечения приложения, используемого конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="c4f52-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="c4f52-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="c4f52-114">headerValue</span></span>|<span data-ttu-id="c4f52-115">String</span><span class="sxs-lookup"><span data-stu-id="c4f52-115">String</span></span>|<span data-ttu-id="c4f52-116">Значение заголовка User — Agent, указанное конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="c4f52-116">User-agent header value reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4f52-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4f52-117">JSON representation</span></span>

<span data-ttu-id="c4f52-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4f52-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.userAgent",
  "baseType": null
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
