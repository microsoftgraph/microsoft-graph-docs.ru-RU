---
title: Тип ресурса modifiedProperty
description: Описывает изменения, внесенные в целевую систему.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 49c2af65022d6fddef394423b6d615dba9f20efc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136180"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="430a1-103">Тип ресурса modifiedProperty</span><span class="sxs-lookup"><span data-stu-id="430a1-103">modifiedProperty resource type</span></span>

<span data-ttu-id="430a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="430a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="430a1-105">Описывает изменения, внесенные в целевую систему.</span><span class="sxs-lookup"><span data-stu-id="430a1-105">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="430a1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="430a1-106">Properties</span></span>

| <span data-ttu-id="430a1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="430a1-107">Property</span></span>     | <span data-ttu-id="430a1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="430a1-108">Type</span></span>        | <span data-ttu-id="430a1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="430a1-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="430a1-110">displayName</span><span class="sxs-lookup"><span data-stu-id="430a1-110">displayName</span></span>|<span data-ttu-id="430a1-111">Строка</span><span class="sxs-lookup"><span data-stu-id="430a1-111">String</span></span>|<span data-ttu-id="430a1-112">Имя измененного свойства.</span><span class="sxs-lookup"><span data-stu-id="430a1-112">Name of property that was modified.</span></span>|
|<span data-ttu-id="430a1-113">newValue</span><span class="sxs-lookup"><span data-stu-id="430a1-113">newValue</span></span>|<span data-ttu-id="430a1-114">String</span><span class="sxs-lookup"><span data-stu-id="430a1-114">String</span></span>|<span data-ttu-id="430a1-115">Новое значение свойства.</span><span class="sxs-lookup"><span data-stu-id="430a1-115">New property value.</span></span>|
|<span data-ttu-id="430a1-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="430a1-116">oldValue</span></span>|<span data-ttu-id="430a1-117">String</span><span class="sxs-lookup"><span data-stu-id="430a1-117">String</span></span>|<span data-ttu-id="430a1-118">Старое значение свойства.</span><span class="sxs-lookup"><span data-stu-id="430a1-118">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="430a1-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="430a1-119">JSON representation</span></span>

<span data-ttu-id="430a1-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="430a1-120">The following is a JSON representation of the resource.</span></span>

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


