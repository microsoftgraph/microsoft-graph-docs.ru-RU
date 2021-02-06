---
title: Тип ресурса keyValue
description: Предоставляет дополнительные важные сведения о запросе на вход
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3459f827f35049b383e732c805d61371577b2260
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135396"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="48240-103">Тип ресурса keyValue</span><span class="sxs-lookup"><span data-stu-id="48240-103">keyValue resource type</span></span>

<span data-ttu-id="48240-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48240-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48240-105">Предоставляет дополнительные сведения об обработке проверки подлинности, такие как имя сервера и наличие подсказок для входов и домена.</span><span class="sxs-lookup"><span data-stu-id="48240-105">Provides additional authentication processing information, such as the server name and the presence of hints for sign in and domain.</span></span>

## <a name="properties"></a><span data-ttu-id="48240-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="48240-106">Properties</span></span>

| <span data-ttu-id="48240-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="48240-107">Property</span></span>     | <span data-ttu-id="48240-108">Тип</span><span class="sxs-lookup"><span data-stu-id="48240-108">Type</span></span>        | <span data-ttu-id="48240-109">Описание</span><span class="sxs-lookup"><span data-stu-id="48240-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="48240-110">key</span><span class="sxs-lookup"><span data-stu-id="48240-110">key</span></span>|<span data-ttu-id="48240-111">Строка</span><span class="sxs-lookup"><span data-stu-id="48240-111">String</span></span>|<span data-ttu-id="48240-112">Содержит имя поля, с которое связано значение.</span><span class="sxs-lookup"><span data-stu-id="48240-112">Contains the name of the field that a value is associated with.</span></span> <span data-ttu-id="48240-113">Если в запрос на вход включена подсказка о входе или домене, соответствующие поля включаются в качестве пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="48240-113">When a sign in or domain hint is included in the sign-in request, corresponding fields are included as key-value pairs.</span></span> <span data-ttu-id="48240-114">Возможные ключи: `Login hint present` , `Domain hint present` .</span><span class="sxs-lookup"><span data-stu-id="48240-114">Possible keys: `Login hint present`, `Domain hint present`.</span></span>|
|<span data-ttu-id="48240-115">value</span><span class="sxs-lookup"><span data-stu-id="48240-115">value</span></span>|<span data-ttu-id="48240-116">String</span><span class="sxs-lookup"><span data-stu-id="48240-116">String</span></span>|<span data-ttu-id="48240-117">Содержит соответствующее значение для указанного ключа.</span><span class="sxs-lookup"><span data-stu-id="48240-117">Contains the corresponding value for the specified key.</span></span> <span data-ttu-id="48240-118">Значением является, если подсказка для входов была включена в запрос на `true` вход; в противном случае `false` .</span><span class="sxs-lookup"><span data-stu-id="48240-118">The value is `true` if a sign in hint was included in the sign-in request; otherwise `false`.</span></span> <span data-ttu-id="48240-119">Значением `true` является, если подсказка домена была включена в запрос на вход; в противном случае `false` .</span><span class="sxs-lookup"><span data-stu-id="48240-119">The value is `true` if a domain hint was included in the sign-in request; otherwise `false`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48240-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="48240-120">JSON representation</span></span>

<span data-ttu-id="48240-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48240-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValue",
  "baseType": null
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


