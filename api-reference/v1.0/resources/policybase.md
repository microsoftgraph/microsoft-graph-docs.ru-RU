---
title: Тип ресурса основы
description: Представляет абстрактный базовый тип для типов политик, от которых наследуется наследование.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4e0d1d59698b8a82252c4cbc2ae8edf2ae1e3b62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037334"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="50aeb-103">Тип ресурса основы</span><span class="sxs-lookup"><span data-stu-id="50aeb-103">policyBase resource type</span></span>

<span data-ttu-id="50aeb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50aeb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50aeb-105">Представляет абстрактный базовый тип для типов политик, от которых наследуется наследование.</span><span class="sxs-lookup"><span data-stu-id="50aeb-105">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="50aeb-106">Методы</span><span class="sxs-lookup"><span data-stu-id="50aeb-106">Methods</span></span>

<span data-ttu-id="50aeb-107">Нет</span><span class="sxs-lookup"><span data-stu-id="50aeb-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="50aeb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="50aeb-108">Properties</span></span>

| <span data-ttu-id="50aeb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="50aeb-109">Property</span></span>     | <span data-ttu-id="50aeb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="50aeb-110">Type</span></span>        | <span data-ttu-id="50aeb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="50aeb-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="50aeb-112">id</span><span class="sxs-lookup"><span data-stu-id="50aeb-112">id</span></span>|<span data-ttu-id="50aeb-113">String</span><span class="sxs-lookup"><span data-stu-id="50aeb-113">String</span></span>| <span data-ttu-id="50aeb-114">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="50aeb-114">Unique identifier for this policy.</span></span> <span data-ttu-id="50aeb-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50aeb-115">Read-only.</span></span>|
|<span data-ttu-id="50aeb-116">description</span><span class="sxs-lookup"><span data-stu-id="50aeb-116">description</span></span>|<span data-ttu-id="50aeb-117">String</span><span class="sxs-lookup"><span data-stu-id="50aeb-117">String</span></span>| <span data-ttu-id="50aeb-118">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="50aeb-118">Description for this policy.</span></span>|
|<span data-ttu-id="50aeb-119">displayName</span><span class="sxs-lookup"><span data-stu-id="50aeb-119">displayName</span></span>|<span data-ttu-id="50aeb-120">String</span><span class="sxs-lookup"><span data-stu-id="50aeb-120">String</span></span>| <span data-ttu-id="50aeb-121">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="50aeb-121">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="50aeb-122">Связи</span><span class="sxs-lookup"><span data-stu-id="50aeb-122">Relationships</span></span>

<span data-ttu-id="50aeb-123">Нет</span><span class="sxs-lookup"><span data-stu-id="50aeb-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50aeb-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50aeb-124">JSON representation</span></span>

<span data-ttu-id="50aeb-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50aeb-125">The following is a JSON representation of the resource.</span></span>

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
