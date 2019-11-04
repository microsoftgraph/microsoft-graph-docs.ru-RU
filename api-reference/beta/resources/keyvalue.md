---
title: Тип ресурса Ключзначение
description: Предоставляет дополнительные релевантные сведения о запросе на вход
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 08f9fc138710626a5b8c1c2b11eeab8ed4cad673
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939308"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="827ae-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="827ae-103">keyValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="827ae-104">Предоставляет дополнительные сведения об обработке проверки подлинности, такие как имя сервера и наличие подсказок для входа и домена.</span><span class="sxs-lookup"><span data-stu-id="827ae-104">Provides additional authentication processing information, such as the server name and the presence of hints for sign in and domain.</span></span>

## <a name="properties"></a><span data-ttu-id="827ae-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="827ae-105">Properties</span></span>

| <span data-ttu-id="827ae-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="827ae-106">Property</span></span>     | <span data-ttu-id="827ae-107">Тип</span><span class="sxs-lookup"><span data-stu-id="827ae-107">Type</span></span>        | <span data-ttu-id="827ae-108">Описание</span><span class="sxs-lookup"><span data-stu-id="827ae-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="827ae-109">key</span><span class="sxs-lookup"><span data-stu-id="827ae-109">key</span></span>|<span data-ttu-id="827ae-110">Строка</span><span class="sxs-lookup"><span data-stu-id="827ae-110">String</span></span>|<span data-ttu-id="827ae-111">Содержит имя поля, с которым связано значение.</span><span class="sxs-lookup"><span data-stu-id="827ae-111">Contains the name of the field that a value is associated with.</span></span> <span data-ttu-id="827ae-112">Если подсказка входа или домена включена в запрос на вход, соответствующие поля включаются в качестве пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="827ae-112">When a sign in or domain hint is included in the sign-in request, corresponding fields are included as key-value pairs.</span></span> <span data-ttu-id="827ae-113">Возможные ключи: `Login hint present`, `Domain hint present`.</span><span class="sxs-lookup"><span data-stu-id="827ae-113">Possible keys: `Login hint present`, `Domain hint present`.</span></span>|
|<span data-ttu-id="827ae-114">value</span><span class="sxs-lookup"><span data-stu-id="827ae-114">value</span></span>|<span data-ttu-id="827ae-115">String</span><span class="sxs-lookup"><span data-stu-id="827ae-115">String</span></span>|<span data-ttu-id="827ae-116">Содержит соответствующее значение для указанного ключа.</span><span class="sxs-lookup"><span data-stu-id="827ae-116">Contains the corresponding value for the specified key.</span></span> <span data-ttu-id="827ae-117">Значение, `true` если подсказка для входа была включена в запрос на вход; в `false`противном случае.</span><span class="sxs-lookup"><span data-stu-id="827ae-117">The value is `true` if a sign in hint was included in the sign-in request; otherwise `false`.</span></span> <span data-ttu-id="827ae-118">Значение, `true` если подсказка домена была включена в запрос на вход; в `false`противном случае.</span><span class="sxs-lookup"><span data-stu-id="827ae-118">The value is `true` if a domain hint was included in the sign-in request; otherwise `false`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="827ae-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="827ae-119">JSON representation</span></span>

<span data-ttu-id="827ae-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="827ae-120">The following is a JSON representation of the resource.</span></span>

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
