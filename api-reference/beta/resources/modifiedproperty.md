---
title: Тип ресурса Модифиедпроперти
description: Описывает изменения, выполненные в целевой системе.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 78b2447c1bdeab986382ec2d7c5d20787c1f15e2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459799"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="f49a0-103">Тип ресурса Модифиедпроперти</span><span class="sxs-lookup"><span data-stu-id="f49a0-103">modifiedProperty resource type</span></span>

<span data-ttu-id="f49a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f49a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f49a0-105">Описывает изменения, выполненные в целевой системе.</span><span class="sxs-lookup"><span data-stu-id="f49a0-105">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="f49a0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f49a0-106">Properties</span></span>

| <span data-ttu-id="f49a0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f49a0-107">Property</span></span>     | <span data-ttu-id="f49a0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f49a0-108">Type</span></span>        | <span data-ttu-id="f49a0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f49a0-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f49a0-110">displayName</span><span class="sxs-lookup"><span data-stu-id="f49a0-110">displayName</span></span>|<span data-ttu-id="f49a0-111">String</span><span class="sxs-lookup"><span data-stu-id="f49a0-111">String</span></span>|<span data-ttu-id="f49a0-112">Имя свойства, которое было изменено.</span><span class="sxs-lookup"><span data-stu-id="f49a0-112">Name of property that was modified.</span></span>|
|<span data-ttu-id="f49a0-113">newValue</span><span class="sxs-lookup"><span data-stu-id="f49a0-113">newValue</span></span>|<span data-ttu-id="f49a0-114">String</span><span class="sxs-lookup"><span data-stu-id="f49a0-114">String</span></span>|<span data-ttu-id="f49a0-115">Новое значение свойства.</span><span class="sxs-lookup"><span data-stu-id="f49a0-115">New property value.</span></span>|
|<span data-ttu-id="f49a0-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="f49a0-116">oldValue</span></span>|<span data-ttu-id="f49a0-117">String</span><span class="sxs-lookup"><span data-stu-id="f49a0-117">String</span></span>|<span data-ttu-id="f49a0-118">Старое значение свойства.</span><span class="sxs-lookup"><span data-stu-id="f49a0-118">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f49a0-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f49a0-119">JSON representation</span></span>

<span data-ttu-id="f49a0-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f49a0-120">The following is a JSON representation of the resource.</span></span>

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
