---
title: Тип ресурса основы
description: Представляет абстрактный базовый тип для типов политик, от которых наследуется наследование.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 757f6771065d60818611662da4dfdcc37ff65853
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234520"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="e6933-103">Тип ресурса основы</span><span class="sxs-lookup"><span data-stu-id="e6933-103">policyBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6933-104">Представляет абстрактный базовый тип для типов политик, от которых наследуется наследование.</span><span class="sxs-lookup"><span data-stu-id="e6933-104">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="e6933-105">Методы</span><span class="sxs-lookup"><span data-stu-id="e6933-105">Methods</span></span>

<span data-ttu-id="e6933-106">Нет</span><span class="sxs-lookup"><span data-stu-id="e6933-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="e6933-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6933-107">Properties</span></span>

| <span data-ttu-id="e6933-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6933-108">Property</span></span>     | <span data-ttu-id="e6933-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e6933-109">Type</span></span>        | <span data-ttu-id="e6933-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e6933-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e6933-111">id</span><span class="sxs-lookup"><span data-stu-id="e6933-111">id</span></span>|<span data-ttu-id="e6933-112">String</span><span class="sxs-lookup"><span data-stu-id="e6933-112">String</span></span>| <span data-ttu-id="e6933-113">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e6933-113">Unique identifier for this policy.</span></span> <span data-ttu-id="e6933-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6933-114">Read-only.</span></span>|
|<span data-ttu-id="e6933-115">description</span><span class="sxs-lookup"><span data-stu-id="e6933-115">description</span></span>|<span data-ttu-id="e6933-116">String</span><span class="sxs-lookup"><span data-stu-id="e6933-116">String</span></span>| <span data-ttu-id="e6933-117">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e6933-117">Description for this policy.</span></span>|
|<span data-ttu-id="e6933-118">displayName</span><span class="sxs-lookup"><span data-stu-id="e6933-118">displayName</span></span>|<span data-ttu-id="e6933-119">Строка</span><span class="sxs-lookup"><span data-stu-id="e6933-119">String</span></span>| <span data-ttu-id="e6933-120">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e6933-120">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e6933-121">Связи</span><span class="sxs-lookup"><span data-stu-id="e6933-121">Relationships</span></span>

<span data-ttu-id="e6933-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e6933-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6933-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6933-123">JSON representation</span></span>

<span data-ttu-id="e6933-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6933-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.policyBase",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policyBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->