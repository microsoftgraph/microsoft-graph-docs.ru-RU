---
title: Тип ресурса networkLocationDetail
description: Предоставляет имя и тип сети, из которой пользователь вписались.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 986a2f292a23bc4c67a88770dac46de59b7294e7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130020"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="94c25-103">Тип ресурса networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="94c25-103">networkLocationDetail resource type</span></span>

<span data-ttu-id="94c25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94c25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94c25-105">Предоставляет имя и тип сети, из которой пользователь вписались.</span><span class="sxs-lookup"><span data-stu-id="94c25-105">Provides the name and type of network from which the user signed in.</span></span>

## <a name="properties"></a><span data-ttu-id="94c25-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="94c25-106">Properties</span></span>

| <span data-ttu-id="94c25-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="94c25-107">Property</span></span>     | <span data-ttu-id="94c25-108">Тип</span><span class="sxs-lookup"><span data-stu-id="94c25-108">Type</span></span>        | <span data-ttu-id="94c25-109">Описание</span><span class="sxs-lookup"><span data-stu-id="94c25-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="94c25-110">networkNames</span><span class="sxs-lookup"><span data-stu-id="94c25-110">networkNames</span></span>|<span data-ttu-id="94c25-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="94c25-111">String collection</span></span>|<span data-ttu-id="94c25-112">Предоставляет имя сети, используемой при входе.</span><span class="sxs-lookup"><span data-stu-id="94c25-112">Provides the name of the network used when signing in.</span></span>|
|<span data-ttu-id="94c25-113">networkType</span><span class="sxs-lookup"><span data-stu-id="94c25-113">networkType</span></span>|<span data-ttu-id="94c25-114">networkType</span><span class="sxs-lookup"><span data-stu-id="94c25-114">networkType</span></span>| <span data-ttu-id="94c25-115">Предоставляет тип сети, используемой при входе.</span><span class="sxs-lookup"><span data-stu-id="94c25-115">Provides the type of network used when signing in.</span></span> <span data-ttu-id="94c25-116">Возможные значения: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="94c25-116">Possible values are: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94c25-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="94c25-117">JSON representation</span></span>

<span data-ttu-id="94c25-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94c25-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail",
  "baseType": null
}-->

```json
{
  "networkNames": ["String"],
  "networkType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

