---
title: Тип ресурса Клиентусеражент
description: Тип Клиентусеражент
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8a21133cfe70f7c887f8d0ecbc782f1b872d0940
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492063"
---
# <a name="clientuseragent-resource-type"></a><span data-ttu-id="282cb-103">Тип ресурса Клиентусеражент</span><span class="sxs-lookup"><span data-stu-id="282cb-103">clientUserAgent resource type</span></span>

<span data-ttu-id="282cb-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="282cb-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="282cb-105">Представляет агент пользователя клиента конечной точки в вызове.</span><span class="sxs-lookup"><span data-stu-id="282cb-105">Represents a client user agent of an endpoint in a call.</span></span> <span data-ttu-id="282cb-106">Наследуется от типа [UserAgent](callrecords-useragent.md) .</span><span class="sxs-lookup"><span data-stu-id="282cb-106">Inherits from the [userAgent](callrecords-useragent.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="282cb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="282cb-107">Properties</span></span>

| <span data-ttu-id="282cb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="282cb-108">Property</span></span>     | <span data-ttu-id="282cb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="282cb-109">Type</span></span>        | <span data-ttu-id="282cb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="282cb-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="282cb-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="282cb-111">applicationVersion</span></span>|<span data-ttu-id="282cb-112">String</span><span class="sxs-lookup"><span data-stu-id="282cb-112">String</span></span>|<span data-ttu-id="282cb-113">Определяет версию программного обеспечения приложения, используемого конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="282cb-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="282cb-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="282cb-114">headerValue</span></span>|<span data-ttu-id="282cb-115">String</span><span class="sxs-lookup"><span data-stu-id="282cb-115">String</span></span>|<span data-ttu-id="282cb-116">Значение заголовка User — Agent, указанное конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="282cb-116">User-agent header value reported by this endpoint.</span></span>|
|<span data-ttu-id="282cb-117">platform</span><span class="sxs-lookup"><span data-stu-id="282cb-117">platform</span></span>|<span data-ttu-id="282cb-118">Microsoft. Graph. Каллрекордс. Клиентплатформ</span><span class="sxs-lookup"><span data-stu-id="282cb-118">microsoft.graph.callRecords.clientPlatform</span></span>|<span data-ttu-id="282cb-119">Определяет платформу, используемую этой конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="282cb-119">Identifies the platform used by this endpoint.</span></span> <span data-ttu-id="282cb-120">Возможные значения: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="282cb-120">Possible values are: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="282cb-121">продуктфамили</span><span class="sxs-lookup"><span data-stu-id="282cb-121">productFamily</span></span>|<span data-ttu-id="282cb-122">Microsoft. Graph. Каллрекордс. Продуктфамили</span><span class="sxs-lookup"><span data-stu-id="282cb-122">microsoft.graph.callRecords.productFamily</span></span>|<span data-ttu-id="282cb-123">Определяет семейство программного обеспечения приложений, используемое этой конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="282cb-123">Identifies the family of application software used by this endpoint.</span></span> <span data-ttu-id="282cb-124">Возможные значения: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="282cb-124">Possible values are: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="282cb-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="282cb-125">JSON representation</span></span>

<span data-ttu-id="282cb-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="282cb-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.clientUserAgent",
  "baseType": "microsoft.graph.callRecords.userAgent"
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String",
  "platform": "String",
  "productFamily": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "clientUserAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->