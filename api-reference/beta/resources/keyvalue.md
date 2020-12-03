---
title: Тип ресурса Ключзначение
description: Предоставляет дополнительные релевантные сведения о запросе на вход
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 78dd4f6ede6e918bb1caaae3761ef258b4e0a427
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524703"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="35ab8-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="35ab8-103">keyValue resource type</span></span>

<span data-ttu-id="35ab8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35ab8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35ab8-105">Предоставляет дополнительные сведения об обработке проверки подлинности, такие как имя сервера и наличие подсказок для входа и домена.</span><span class="sxs-lookup"><span data-stu-id="35ab8-105">Provides additional authentication processing information, such as the server name and the presence of hints for sign in and domain.</span></span>

## <a name="properties"></a><span data-ttu-id="35ab8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="35ab8-106">Properties</span></span>

| <span data-ttu-id="35ab8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="35ab8-107">Property</span></span>     | <span data-ttu-id="35ab8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="35ab8-108">Type</span></span>        | <span data-ttu-id="35ab8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="35ab8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="35ab8-110">key</span><span class="sxs-lookup"><span data-stu-id="35ab8-110">key</span></span>|<span data-ttu-id="35ab8-111">String</span><span class="sxs-lookup"><span data-stu-id="35ab8-111">String</span></span>|<span data-ttu-id="35ab8-112">Содержит имя поля, с которым связано значение.</span><span class="sxs-lookup"><span data-stu-id="35ab8-112">Contains the name of the field that a value is associated with.</span></span> <span data-ttu-id="35ab8-113">Если подсказка входа или домена включена в запрос на вход, соответствующие поля включаются в качестве пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="35ab8-113">When a sign in or domain hint is included in the sign-in request, corresponding fields are included as key-value pairs.</span></span> <span data-ttu-id="35ab8-114">Возможные ключи: `Login hint present` , `Domain hint present` .</span><span class="sxs-lookup"><span data-stu-id="35ab8-114">Possible keys: `Login hint present`, `Domain hint present`.</span></span>|
|<span data-ttu-id="35ab8-115">value</span><span class="sxs-lookup"><span data-stu-id="35ab8-115">value</span></span>|<span data-ttu-id="35ab8-116">String</span><span class="sxs-lookup"><span data-stu-id="35ab8-116">String</span></span>|<span data-ttu-id="35ab8-117">Содержит соответствующее значение для указанного ключа.</span><span class="sxs-lookup"><span data-stu-id="35ab8-117">Contains the corresponding value for the specified key.</span></span> <span data-ttu-id="35ab8-118">Значение, `true` Если подсказка для входа была включена в запрос на вход; в противном случае `false` .</span><span class="sxs-lookup"><span data-stu-id="35ab8-118">The value is `true` if a sign in hint was included in the sign-in request; otherwise `false`.</span></span> <span data-ttu-id="35ab8-119">Значение, `true` Если подсказка домена включена в запрос на вход; в противном случае `false` .</span><span class="sxs-lookup"><span data-stu-id="35ab8-119">The value is `true` if a domain hint was included in the sign-in request; otherwise `false`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35ab8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35ab8-120">JSON representation</span></span>

<span data-ttu-id="35ab8-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35ab8-121">The following is a JSON representation of the resource.</span></span>

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


