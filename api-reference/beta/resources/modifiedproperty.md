---
title: Тип ресурса Модифиедпроперти
description: Описывает изменения, выполненные в целевой системе.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d5dbf7f3ef2078baca54c03e8e67a94f5b52ee85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021296"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="7bfab-103">Тип ресурса Модифиедпроперти</span><span class="sxs-lookup"><span data-stu-id="7bfab-103">modifiedProperty resource type</span></span>

<span data-ttu-id="7bfab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bfab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bfab-105">Описывает изменения, выполненные в целевой системе.</span><span class="sxs-lookup"><span data-stu-id="7bfab-105">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="7bfab-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bfab-106">Properties</span></span>

| <span data-ttu-id="7bfab-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bfab-107">Property</span></span>     | <span data-ttu-id="7bfab-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7bfab-108">Type</span></span>        | <span data-ttu-id="7bfab-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7bfab-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7bfab-110">displayName</span><span class="sxs-lookup"><span data-stu-id="7bfab-110">displayName</span></span>|<span data-ttu-id="7bfab-111">String</span><span class="sxs-lookup"><span data-stu-id="7bfab-111">String</span></span>|<span data-ttu-id="7bfab-112">Имя свойства, которое было изменено.</span><span class="sxs-lookup"><span data-stu-id="7bfab-112">Name of property that was modified.</span></span>|
|<span data-ttu-id="7bfab-113">newValue</span><span class="sxs-lookup"><span data-stu-id="7bfab-113">newValue</span></span>|<span data-ttu-id="7bfab-114">String</span><span class="sxs-lookup"><span data-stu-id="7bfab-114">String</span></span>|<span data-ttu-id="7bfab-115">Новое значение свойства.</span><span class="sxs-lookup"><span data-stu-id="7bfab-115">New property value.</span></span>|
|<span data-ttu-id="7bfab-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="7bfab-116">oldValue</span></span>|<span data-ttu-id="7bfab-117">String</span><span class="sxs-lookup"><span data-stu-id="7bfab-117">String</span></span>|<span data-ttu-id="7bfab-118">Старое значение свойства.</span><span class="sxs-lookup"><span data-stu-id="7bfab-118">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bfab-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7bfab-119">JSON representation</span></span>

<span data-ttu-id="7bfab-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bfab-120">The following is a JSON representation of the resource.</span></span>

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


