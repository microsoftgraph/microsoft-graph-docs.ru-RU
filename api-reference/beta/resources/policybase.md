---
title: Тип ресурса policyBase
description: Представляет абстрактный базовый тип для типов политик, от которые можно наследовать.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b495503cf01ce13e5f5d44d371b824a1eedfccb5
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760850"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="d7d5a-103">Тип ресурса policyBase</span><span class="sxs-lookup"><span data-stu-id="d7d5a-103">policyBase resource type</span></span>

<span data-ttu-id="d7d5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7d5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7d5a-105">Представляет абстрактный базовый тип для типов политик, от которые можно наследовать.</span><span class="sxs-lookup"><span data-stu-id="d7d5a-105">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="d7d5a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d7d5a-106">Methods</span></span>

<span data-ttu-id="d7d5a-107">Нет</span><span class="sxs-lookup"><span data-stu-id="d7d5a-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="d7d5a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7d5a-108">Properties</span></span>

| <span data-ttu-id="d7d5a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7d5a-109">Property</span></span>     | <span data-ttu-id="d7d5a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d7d5a-110">Type</span></span>        | <span data-ttu-id="d7d5a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d7d5a-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d7d5a-112">id</span><span class="sxs-lookup"><span data-stu-id="d7d5a-112">id</span></span>|<span data-ttu-id="d7d5a-113">String</span><span class="sxs-lookup"><span data-stu-id="d7d5a-113">String</span></span>| <span data-ttu-id="d7d5a-114">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d7d5a-114">Unique identifier for this policy.</span></span> <span data-ttu-id="d7d5a-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7d5a-115">Read-only.</span></span>|
|<span data-ttu-id="d7d5a-116">description</span><span class="sxs-lookup"><span data-stu-id="d7d5a-116">description</span></span>|<span data-ttu-id="d7d5a-117">String</span><span class="sxs-lookup"><span data-stu-id="d7d5a-117">String</span></span>| <span data-ttu-id="d7d5a-118">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="d7d5a-118">Description for this policy.</span></span>|
|<span data-ttu-id="d7d5a-119">displayName</span><span class="sxs-lookup"><span data-stu-id="d7d5a-119">displayName</span></span>|<span data-ttu-id="d7d5a-120">String</span><span class="sxs-lookup"><span data-stu-id="d7d5a-120">String</span></span>| <span data-ttu-id="d7d5a-121">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d7d5a-121">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d7d5a-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="d7d5a-122">Relationships</span></span>

<span data-ttu-id="d7d5a-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d7d5a-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7d5a-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7d5a-124">JSON representation</span></span>

<span data-ttu-id="d7d5a-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7d5a-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.policyBase",
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

