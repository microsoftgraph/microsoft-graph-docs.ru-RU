---
title: Тип ресурса Модифиедпроперти
description: Описывает изменения, выполненные в целевой системе.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dcf55dfc83414b5a516bac6cbeefa3358323b5fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966706"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="9b618-103">Тип ресурса Модифиедпроперти</span><span class="sxs-lookup"><span data-stu-id="9b618-103">modifiedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b618-104">Описывает изменения, выполненные в целевой системе.</span><span class="sxs-lookup"><span data-stu-id="9b618-104">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="9b618-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b618-105">Properties</span></span>

| <span data-ttu-id="9b618-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b618-106">Property</span></span>     | <span data-ttu-id="9b618-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9b618-107">Type</span></span>        | <span data-ttu-id="9b618-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9b618-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9b618-109">displayName</span><span class="sxs-lookup"><span data-stu-id="9b618-109">displayName</span></span>|<span data-ttu-id="9b618-110">String</span><span class="sxs-lookup"><span data-stu-id="9b618-110">String</span></span>|<span data-ttu-id="9b618-111">Имя свойства, которое было изменено.</span><span class="sxs-lookup"><span data-stu-id="9b618-111">Name of property that was modified.</span></span>|
|<span data-ttu-id="9b618-112">newValue</span><span class="sxs-lookup"><span data-stu-id="9b618-112">newValue</span></span>|<span data-ttu-id="9b618-113">String</span><span class="sxs-lookup"><span data-stu-id="9b618-113">String</span></span>|<span data-ttu-id="9b618-114">Новое значение свойства.</span><span class="sxs-lookup"><span data-stu-id="9b618-114">New property value.</span></span>|
|<span data-ttu-id="9b618-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="9b618-115">oldValue</span></span>|<span data-ttu-id="9b618-116">String</span><span class="sxs-lookup"><span data-stu-id="9b618-116">String</span></span>|<span data-ttu-id="9b618-117">Старое значение свойства.</span><span class="sxs-lookup"><span data-stu-id="9b618-117">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b618-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b618-118">JSON representation</span></span>

<span data-ttu-id="9b618-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b618-119">The following is a JSON representation of the resource.</span></span>

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
