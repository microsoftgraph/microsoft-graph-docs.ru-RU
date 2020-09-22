---
title: Тип ресурса Релатедперсон
description: Тип ресурса Релатедперсон
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 88d7283d1eac1f3b7bcc7d947fa1961494a58041
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033575"
---
# <a name="relatedperson-resource-type"></a><span data-ttu-id="e65e4-103">Тип ресурса Релатедперсон</span><span class="sxs-lookup"><span data-stu-id="e65e4-103">relatedPerson resource type</span></span>

<span data-ttu-id="e65e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e65e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e65e4-105">Представляет сведения о пользователях, связанных с информацией в данной сущности в [профиле](profile.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="e65e4-105">Represents information about people related to information within a given entity in a [profile](profile.md) for a user.</span></span>

## <a name="properties"></a><span data-ttu-id="e65e4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e65e4-106">Properties</span></span>

| <span data-ttu-id="e65e4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e65e4-107">Property</span></span>        | <span data-ttu-id="e65e4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e65e4-108">Type</span></span>        | <span data-ttu-id="e65e4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e65e4-109">Description</span></span>                                                                                                                                                                                                                                     |
|:----------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="e65e4-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e65e4-110">displayName</span></span>      |<span data-ttu-id="e65e4-111">String</span><span class="sxs-lookup"><span data-stu-id="e65e4-111">String</span></span>       | <span data-ttu-id="e65e4-112">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="e65e4-112">Name of the person.</span></span>                                                                                                                                                                                                                             |
|<span data-ttu-id="e65e4-113">Отношение</span><span class="sxs-lookup"><span data-stu-id="e65e4-113">relationship</span></span>     |<span data-ttu-id="e65e4-114">String</span><span class="sxs-lookup"><span data-stu-id="e65e4-114">String</span></span>       | <span data-ttu-id="e65e4-115">Возможные значения: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e65e4-115">Possible values are: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e65e4-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e65e4-116">userPrincipalName</span></span>|<span data-ttu-id="e65e4-117">String</span><span class="sxs-lookup"><span data-stu-id="e65e4-117">String</span></span>       | <span data-ttu-id="e65e4-118">Адрес электронной почты или ссылка на пользователя в Организации.</span><span class="sxs-lookup"><span data-stu-id="e65e4-118">Email address or reference to person within organization.</span></span>                                                                                                                                                                                       |

## <a name="json-representation"></a><span data-ttu-id="e65e4-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e65e4-119">JSON representation</span></span>

<span data-ttu-id="e65e4-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e65e4-120">The following is a JSON representation of the resource.</span></span>

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


