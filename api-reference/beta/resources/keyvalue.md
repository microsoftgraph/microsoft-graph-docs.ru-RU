---
title: Тип ресурса Ключзначение
description: Предоставляет дополнительные релевантные сведения о запросе на вход
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e3f85936e94da0485d62478f54eed8918967396b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442725"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="5145e-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="5145e-103">keyValue resource type</span></span>

<span data-ttu-id="5145e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5145e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5145e-105">Предоставляет дополнительные сведения об обработке проверки подлинности, такие как имя сервера и наличие подсказок для входа и домена.</span><span class="sxs-lookup"><span data-stu-id="5145e-105">Provides additional authentication processing information, such as the server name and the presence of hints for sign in and domain.</span></span>

## <a name="properties"></a><span data-ttu-id="5145e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5145e-106">Properties</span></span>

| <span data-ttu-id="5145e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5145e-107">Property</span></span>     | <span data-ttu-id="5145e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5145e-108">Type</span></span>        | <span data-ttu-id="5145e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5145e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5145e-110">key</span><span class="sxs-lookup"><span data-stu-id="5145e-110">key</span></span>|<span data-ttu-id="5145e-111">String</span><span class="sxs-lookup"><span data-stu-id="5145e-111">String</span></span>|<span data-ttu-id="5145e-112">Содержит имя поля, с которым связано значение.</span><span class="sxs-lookup"><span data-stu-id="5145e-112">Contains the name of the field that a value is associated with.</span></span> <span data-ttu-id="5145e-113">Если подсказка входа или домена включена в запрос на вход, соответствующие поля включаются в качестве пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="5145e-113">When a sign in or domain hint is included in the sign-in request, corresponding fields are included as key-value pairs.</span></span> <span data-ttu-id="5145e-114">Возможные ключи: `Login hint present`, `Domain hint present`.</span><span class="sxs-lookup"><span data-stu-id="5145e-114">Possible keys: `Login hint present`, `Domain hint present`.</span></span>|
|<span data-ttu-id="5145e-115">value</span><span class="sxs-lookup"><span data-stu-id="5145e-115">value</span></span>|<span data-ttu-id="5145e-116">String</span><span class="sxs-lookup"><span data-stu-id="5145e-116">String</span></span>|<span data-ttu-id="5145e-117">Содержит соответствующее значение для указанного ключа.</span><span class="sxs-lookup"><span data-stu-id="5145e-117">Contains the corresponding value for the specified key.</span></span> <span data-ttu-id="5145e-118">Значение, `true` если подсказка для входа была включена в запрос на вход; в `false`противном случае.</span><span class="sxs-lookup"><span data-stu-id="5145e-118">The value is `true` if a sign in hint was included in the sign-in request; otherwise `false`.</span></span> <span data-ttu-id="5145e-119">Значение, `true` если подсказка домена была включена в запрос на вход; в `false`противном случае.</span><span class="sxs-lookup"><span data-stu-id="5145e-119">The value is `true` if a domain hint was included in the sign-in request; otherwise `false`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5145e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5145e-120">JSON representation</span></span>

<span data-ttu-id="5145e-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5145e-121">The following is a JSON representation of the resource.</span></span>

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
