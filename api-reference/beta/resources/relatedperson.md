---
title: Тип ресурса Релатедперсон
description: Тип ресурса Релатедперсон
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6be6300bc901305fb87b04e2482f145b9187f9fb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939238"
---
# <a name="relatedperson-resource-type"></a><span data-ttu-id="1cde4-103">Тип ресурса Релатедперсон</span><span class="sxs-lookup"><span data-stu-id="1cde4-103">relatedPerson resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cde4-104">Представляет сведения о пользователях, связанных с информацией в данной сущности в [профиле](profile.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cde4-104">Represents information about people related to information within a given entity in a [profile](profile.md) for a user.</span></span>

## <a name="properties"></a><span data-ttu-id="1cde4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1cde4-105">Properties</span></span>

| <span data-ttu-id="1cde4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cde4-106">Property</span></span>        | <span data-ttu-id="1cde4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1cde4-107">Type</span></span>        | <span data-ttu-id="1cde4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1cde4-108">Description</span></span>                                               |
|:----------------|:------------|:----------------------------------------------------------|
|<span data-ttu-id="1cde4-109">displayName</span><span class="sxs-lookup"><span data-stu-id="1cde4-109">displayName</span></span>      |<span data-ttu-id="1cde4-110">Строка</span><span class="sxs-lookup"><span data-stu-id="1cde4-110">String</span></span>       | <span data-ttu-id="1cde4-111">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cde4-111">Name of the person.</span></span>                                        |
|<span data-ttu-id="1cde4-112">Отношение</span><span class="sxs-lookup"><span data-stu-id="1cde4-112">relationship</span></span>     |<span data-ttu-id="1cde4-113">Строка</span><span class="sxs-lookup"><span data-stu-id="1cde4-113">String</span></span>       | <span data-ttu-id="1cde4-114">Возможные значения: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1cde4-114">Possible values are: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1cde4-115">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1cde4-115">userPrincipalName</span></span>|<span data-ttu-id="1cde4-116">String</span><span class="sxs-lookup"><span data-stu-id="1cde4-116">String</span></span>       | <span data-ttu-id="1cde4-117">Адрес электронной почты или ссылка на пользователя в Организации.</span><span class="sxs-lookup"><span data-stu-id="1cde4-117">Email address or reference to person within organization.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1cde4-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1cde4-118">JSON representation</span></span>

<span data-ttu-id="1cde4-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cde4-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedPerson",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "relationship": "String",
  "userPrincipalName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "relatedPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
