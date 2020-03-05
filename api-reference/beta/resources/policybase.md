---
title: Тип ресурса основы
description: Представляет абстрактный базовый тип для типов политик, от которых наследуется наследование.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7675183d5b6316db42d9860ac54009b321720a29
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521602"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="c4bc9-103">Тип ресурса основы</span><span class="sxs-lookup"><span data-stu-id="c4bc9-103">policyBase resource type</span></span>

<span data-ttu-id="c4bc9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c4bc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4bc9-105">Представляет абстрактный базовый тип для типов политик, от которых наследуется наследование.</span><span class="sxs-lookup"><span data-stu-id="c4bc9-105">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="c4bc9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c4bc9-106">Methods</span></span>

<span data-ttu-id="c4bc9-107">Нет</span><span class="sxs-lookup"><span data-stu-id="c4bc9-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="c4bc9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4bc9-108">Properties</span></span>

| <span data-ttu-id="c4bc9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4bc9-109">Property</span></span>     | <span data-ttu-id="c4bc9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c4bc9-110">Type</span></span>        | <span data-ttu-id="c4bc9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c4bc9-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c4bc9-112">id</span><span class="sxs-lookup"><span data-stu-id="c4bc9-112">id</span></span>|<span data-ttu-id="c4bc9-113">String</span><span class="sxs-lookup"><span data-stu-id="c4bc9-113">String</span></span>| <span data-ttu-id="c4bc9-114">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c4bc9-114">Unique identifier for this policy.</span></span> <span data-ttu-id="c4bc9-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4bc9-115">Read-only.</span></span>|
|<span data-ttu-id="c4bc9-116">description</span><span class="sxs-lookup"><span data-stu-id="c4bc9-116">description</span></span>|<span data-ttu-id="c4bc9-117">String</span><span class="sxs-lookup"><span data-stu-id="c4bc9-117">String</span></span>| <span data-ttu-id="c4bc9-118">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c4bc9-118">Description for this policy.</span></span>|
|<span data-ttu-id="c4bc9-119">displayName</span><span class="sxs-lookup"><span data-stu-id="c4bc9-119">displayName</span></span>|<span data-ttu-id="c4bc9-120">Строка</span><span class="sxs-lookup"><span data-stu-id="c4bc9-120">String</span></span>| <span data-ttu-id="c4bc9-121">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c4bc9-121">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c4bc9-122">Связи</span><span class="sxs-lookup"><span data-stu-id="c4bc9-122">Relationships</span></span>

<span data-ttu-id="c4bc9-123">Нет</span><span class="sxs-lookup"><span data-stu-id="c4bc9-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4bc9-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4bc9-124">JSON representation</span></span>

<span data-ttu-id="c4bc9-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4bc9-125">The following is a JSON representation of the resource.</span></span>

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