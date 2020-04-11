---
title: Тип ресурса основы
description: Представляет абстрактный базовый тип для типов политик, от которых наследуется наследование.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a053732b6751ef938e0bcf08ebfdb37c0685e287
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229439"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="4c331-103">Тип ресурса основы</span><span class="sxs-lookup"><span data-stu-id="4c331-103">policyBase resource type</span></span>

<span data-ttu-id="4c331-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c331-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c331-105">Представляет абстрактный базовый тип для типов политик, от которых наследуется наследование.</span><span class="sxs-lookup"><span data-stu-id="4c331-105">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="4c331-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4c331-106">Methods</span></span>

<span data-ttu-id="4c331-107">Нет</span><span class="sxs-lookup"><span data-stu-id="4c331-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="4c331-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c331-108">Properties</span></span>

| <span data-ttu-id="4c331-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c331-109">Property</span></span>     | <span data-ttu-id="4c331-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4c331-110">Type</span></span>        | <span data-ttu-id="4c331-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4c331-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4c331-112">id</span><span class="sxs-lookup"><span data-stu-id="4c331-112">id</span></span>|<span data-ttu-id="4c331-113">String</span><span class="sxs-lookup"><span data-stu-id="4c331-113">String</span></span>| <span data-ttu-id="4c331-114">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4c331-114">Unique identifier for this policy.</span></span> <span data-ttu-id="4c331-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c331-115">Read-only.</span></span>|
|<span data-ttu-id="4c331-116">description</span><span class="sxs-lookup"><span data-stu-id="4c331-116">description</span></span>|<span data-ttu-id="4c331-117">String</span><span class="sxs-lookup"><span data-stu-id="4c331-117">String</span></span>| <span data-ttu-id="4c331-118">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4c331-118">Description for this policy.</span></span>|
|<span data-ttu-id="4c331-119">displayName</span><span class="sxs-lookup"><span data-stu-id="4c331-119">displayName</span></span>|<span data-ttu-id="4c331-120">Строка</span><span class="sxs-lookup"><span data-stu-id="4c331-120">String</span></span>| <span data-ttu-id="4c331-121">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4c331-121">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4c331-122">Связи</span><span class="sxs-lookup"><span data-stu-id="4c331-122">Relationships</span></span>

<span data-ttu-id="4c331-123">Нет</span><span class="sxs-lookup"><span data-stu-id="4c331-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c331-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c331-124">JSON representation</span></span>

<span data-ttu-id="4c331-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c331-125">The following is a JSON representation of the resource.</span></span>

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