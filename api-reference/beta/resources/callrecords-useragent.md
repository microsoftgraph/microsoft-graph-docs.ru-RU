---
title: Тип ресурса userAgent
description: Тип userAgent
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d86e76edb66f3b72e97b392dc6478861524356c6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601384"
---
# <a name="useragent-resource-type"></a><span data-ttu-id="41c10-103">Тип ресурса userAgent</span><span class="sxs-lookup"><span data-stu-id="41c10-103">userAgent resource type</span></span>

<span data-ttu-id="41c10-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="41c10-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41c10-105">Представляет агента пользователя конечной точки в вызове.</span><span class="sxs-lookup"><span data-stu-id="41c10-105">Represents the user agent of an endpoint in a call.</span></span>
<span data-ttu-id="41c10-106">Типы [клиентусеражент](callrecords-clientuseragent.md) и [сервицеусеражент](callrecords-serviceuseragent.md)) наследуются от этого типа.</span><span class="sxs-lookup"><span data-stu-id="41c10-106">The [clientUserAgent](callrecords-clientuseragent.md) and [serviceUserAgent](callrecords-serviceuseragent.md)) types inherit from this type.</span></span>

## <a name="properties"></a><span data-ttu-id="41c10-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="41c10-107">Properties</span></span>

| <span data-ttu-id="41c10-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="41c10-108">Property</span></span>     | <span data-ttu-id="41c10-109">Тип</span><span class="sxs-lookup"><span data-stu-id="41c10-109">Type</span></span>        | <span data-ttu-id="41c10-110">Описание</span><span class="sxs-lookup"><span data-stu-id="41c10-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="41c10-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="41c10-111">applicationVersion</span></span>|<span data-ttu-id="41c10-112">String</span><span class="sxs-lookup"><span data-stu-id="41c10-112">String</span></span>|<span data-ttu-id="41c10-113">Определяет версию программного обеспечения приложения, используемого конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="41c10-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="41c10-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="41c10-114">headerValue</span></span>|<span data-ttu-id="41c10-115">String</span><span class="sxs-lookup"><span data-stu-id="41c10-115">String</span></span>|<span data-ttu-id="41c10-116">Значение заголовка User — Agent, указанное конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="41c10-116">User-agent header value reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41c10-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41c10-117">JSON representation</span></span>

<span data-ttu-id="41c10-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41c10-118">The following is a JSON representation of the resource.</span></span>

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

