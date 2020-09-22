---
title: Тип ресурса Endpoint
description: Тип конечной точки
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ae7d976c9dbf94aadd11af1d48f8615f5fab14a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069450"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="0df06-103">Тип ресурса Endpoint</span><span class="sxs-lookup"><span data-stu-id="0df06-103">endpoint resource type</span></span>

<span data-ttu-id="0df06-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="0df06-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="0df06-105">Представляет конечную точку в вызове.</span><span class="sxs-lookup"><span data-stu-id="0df06-105">Represents an endpoint in a call.</span></span> <span data-ttu-id="0df06-106">Конечной точкой может быть устройство пользователя, собрание, приложение/Bot и т. д. Типы [партиЦипантендпоинт](callrecords-participantendpoint.md) и [сервицеендпоинт](callrecords-serviceendpoint.md) наследуются от этого типа.</span><span class="sxs-lookup"><span data-stu-id="0df06-106">The endpoint could be a user's device, a meeting, an application/bot, etc. The [participantEndpoint](callrecords-participantendpoint.md) and [serviceEndpoint](callrecords-serviceendpoint.md) types inherit from this type.</span></span>

## <a name="properties"></a><span data-ttu-id="0df06-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0df06-107">Properties</span></span>

| <span data-ttu-id="0df06-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0df06-108">Property</span></span>     | <span data-ttu-id="0df06-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0df06-109">Type</span></span>        | <span data-ttu-id="0df06-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0df06-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0df06-111">userAgent</span><span class="sxs-lookup"><span data-stu-id="0df06-111">userAgent</span></span>|[<span data-ttu-id="0df06-112">Microsoft. Graph. Каллрекордс. userAgent</span><span class="sxs-lookup"><span data-stu-id="0df06-112">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="0df06-113">Пользователь — агент, указанный этой конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="0df06-113">User-agent reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0df06-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0df06-114">JSON representation</span></span>

<span data-ttu-id="0df06-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0df06-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.endpoint",
  "baseType": null
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
  "description": "endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
