---
title: Тип ресурса policyBase
description: Представляет абстрактный базовый тип для типов политик, от которые необходимо наследовать.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f6b3f0951248bcfe3571f218549f952a27cf7b92
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153615"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="a4cda-103">Тип ресурса policyBase</span><span class="sxs-lookup"><span data-stu-id="a4cda-103">policyBase resource type</span></span>

<span data-ttu-id="a4cda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4cda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4cda-105">Представляет абстрактный базовый тип для типов политик, от которые необходимо наследовать.</span><span class="sxs-lookup"><span data-stu-id="a4cda-105">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="a4cda-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a4cda-106">Methods</span></span>

<span data-ttu-id="a4cda-107">Нет</span><span class="sxs-lookup"><span data-stu-id="a4cda-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="a4cda-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4cda-108">Properties</span></span>

| <span data-ttu-id="a4cda-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4cda-109">Property</span></span>     | <span data-ttu-id="a4cda-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a4cda-110">Type</span></span>        | <span data-ttu-id="a4cda-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a4cda-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4cda-112">id</span><span class="sxs-lookup"><span data-stu-id="a4cda-112">id</span></span>|<span data-ttu-id="a4cda-113">String</span><span class="sxs-lookup"><span data-stu-id="a4cda-113">String</span></span>| <span data-ttu-id="a4cda-114">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a4cda-114">Unique identifier for this policy.</span></span> <span data-ttu-id="a4cda-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4cda-115">Read-only.</span></span>|
|<span data-ttu-id="a4cda-116">description</span><span class="sxs-lookup"><span data-stu-id="a4cda-116">description</span></span>|<span data-ttu-id="a4cda-117">String</span><span class="sxs-lookup"><span data-stu-id="a4cda-117">String</span></span>| <span data-ttu-id="a4cda-118">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="a4cda-118">Description for this policy.</span></span>|
|<span data-ttu-id="a4cda-119">displayName</span><span class="sxs-lookup"><span data-stu-id="a4cda-119">displayName</span></span>|<span data-ttu-id="a4cda-120">String</span><span class="sxs-lookup"><span data-stu-id="a4cda-120">String</span></span>| <span data-ttu-id="a4cda-121">Отображаемого имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a4cda-121">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a4cda-122">Связи</span><span class="sxs-lookup"><span data-stu-id="a4cda-122">Relationships</span></span>

<span data-ttu-id="a4cda-123">Нет</span><span class="sxs-lookup"><span data-stu-id="a4cda-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4cda-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4cda-124">JSON representation</span></span>

<span data-ttu-id="a4cda-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4cda-125">The following is a JSON representation of the resource.</span></span>

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

