---
title: Тип ресурса Модифиедпроперти
description: Описывает изменения, выполненные в целевой системе.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 03ae8cb2c36cb811325839341c0fa8b3f395c954
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35348707"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="b8c94-103">Тип ресурса Модифиедпроперти</span><span class="sxs-lookup"><span data-stu-id="b8c94-103">modifiedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8c94-104">Описывает изменения, выполненные в целевой системе.</span><span class="sxs-lookup"><span data-stu-id="b8c94-104">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="b8c94-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8c94-105">Properties</span></span>

| <span data-ttu-id="b8c94-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8c94-106">Property</span></span>     | <span data-ttu-id="b8c94-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b8c94-107">Type</span></span>        | <span data-ttu-id="b8c94-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b8c94-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8c94-109">displayName</span><span class="sxs-lookup"><span data-stu-id="b8c94-109">displayName</span></span>|<span data-ttu-id="b8c94-110">String</span><span class="sxs-lookup"><span data-stu-id="b8c94-110">String</span></span>|<span data-ttu-id="b8c94-111">Имя свойства, которое было изменено.</span><span class="sxs-lookup"><span data-stu-id="b8c94-111">Name of property that was modified.</span></span>|
|<span data-ttu-id="b8c94-112">newValue</span><span class="sxs-lookup"><span data-stu-id="b8c94-112">newValue</span></span>|<span data-ttu-id="b8c94-113">String</span><span class="sxs-lookup"><span data-stu-id="b8c94-113">String</span></span>|<span data-ttu-id="b8c94-114">Новое значение свойства.</span><span class="sxs-lookup"><span data-stu-id="b8c94-114">New property value.</span></span>|
|<span data-ttu-id="b8c94-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="b8c94-115">oldValue</span></span>|<span data-ttu-id="b8c94-116">String</span><span class="sxs-lookup"><span data-stu-id="b8c94-116">String</span></span>|<span data-ttu-id="b8c94-117">Старое значение свойства.</span><span class="sxs-lookup"><span data-stu-id="b8c94-117">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8c94-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8c94-118">JSON representation</span></span>

<span data-ttu-id="b8c94-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8c94-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
