---
title: Тип ресурса основы
description: Представляет абстрактный базовый тип для типов политик, от которых наследуется наследование.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 527549d4af2e2fb103cb7d2484d844fd3c876e4c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033645"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="7de2e-103">Тип ресурса основы</span><span class="sxs-lookup"><span data-stu-id="7de2e-103">policyBase resource type</span></span>

<span data-ttu-id="7de2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7de2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7de2e-105">Представляет абстрактный базовый тип для типов политик, от которых наследуется наследование.</span><span class="sxs-lookup"><span data-stu-id="7de2e-105">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="7de2e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7de2e-106">Methods</span></span>

<span data-ttu-id="7de2e-107">Нет</span><span class="sxs-lookup"><span data-stu-id="7de2e-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="7de2e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7de2e-108">Properties</span></span>

| <span data-ttu-id="7de2e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7de2e-109">Property</span></span>     | <span data-ttu-id="7de2e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7de2e-110">Type</span></span>        | <span data-ttu-id="7de2e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7de2e-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7de2e-112">id</span><span class="sxs-lookup"><span data-stu-id="7de2e-112">id</span></span>|<span data-ttu-id="7de2e-113">String</span><span class="sxs-lookup"><span data-stu-id="7de2e-113">String</span></span>| <span data-ttu-id="7de2e-114">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7de2e-114">Unique identifier for this policy.</span></span> <span data-ttu-id="7de2e-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7de2e-115">Read-only.</span></span>|
|<span data-ttu-id="7de2e-116">description</span><span class="sxs-lookup"><span data-stu-id="7de2e-116">description</span></span>|<span data-ttu-id="7de2e-117">String</span><span class="sxs-lookup"><span data-stu-id="7de2e-117">String</span></span>| <span data-ttu-id="7de2e-118">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7de2e-118">Description for this policy.</span></span>|
|<span data-ttu-id="7de2e-119">displayName</span><span class="sxs-lookup"><span data-stu-id="7de2e-119">displayName</span></span>|<span data-ttu-id="7de2e-120">String</span><span class="sxs-lookup"><span data-stu-id="7de2e-120">String</span></span>| <span data-ttu-id="7de2e-121">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7de2e-121">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7de2e-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="7de2e-122">Relationships</span></span>

<span data-ttu-id="7de2e-123">Нет</span><span class="sxs-lookup"><span data-stu-id="7de2e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7de2e-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7de2e-124">JSON representation</span></span>

<span data-ttu-id="7de2e-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7de2e-125">The following is a JSON representation of the resource.</span></span>

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

