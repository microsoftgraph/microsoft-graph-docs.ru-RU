---
title: Тип ресурса Модифиедпроперти
description: Описывает изменения, выполненные в целевой системе.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5ae34932d2c08d472f27167c02993b2ef916faae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522626"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="d684a-103">Тип ресурса Модифиедпроперти</span><span class="sxs-lookup"><span data-stu-id="d684a-103">modifiedProperty resource type</span></span>

<span data-ttu-id="d684a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d684a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d684a-105">Описывает изменения, выполненные в целевой системе.</span><span class="sxs-lookup"><span data-stu-id="d684a-105">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="d684a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d684a-106">Properties</span></span>

| <span data-ttu-id="d684a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d684a-107">Property</span></span>     | <span data-ttu-id="d684a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d684a-108">Type</span></span>        | <span data-ttu-id="d684a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d684a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d684a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="d684a-110">displayName</span></span>|<span data-ttu-id="d684a-111">String</span><span class="sxs-lookup"><span data-stu-id="d684a-111">String</span></span>|<span data-ttu-id="d684a-112">Имя свойства, которое было изменено.</span><span class="sxs-lookup"><span data-stu-id="d684a-112">Name of property that was modified.</span></span>|
|<span data-ttu-id="d684a-113">newValue</span><span class="sxs-lookup"><span data-stu-id="d684a-113">newValue</span></span>|<span data-ttu-id="d684a-114">String</span><span class="sxs-lookup"><span data-stu-id="d684a-114">String</span></span>|<span data-ttu-id="d684a-115">Новое значение свойства.</span><span class="sxs-lookup"><span data-stu-id="d684a-115">New property value.</span></span>|
|<span data-ttu-id="d684a-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="d684a-116">oldValue</span></span>|<span data-ttu-id="d684a-117">String</span><span class="sxs-lookup"><span data-stu-id="d684a-117">String</span></span>|<span data-ttu-id="d684a-118">Старое значение свойства.</span><span class="sxs-lookup"><span data-stu-id="d684a-118">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d684a-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d684a-119">JSON representation</span></span>

<span data-ttu-id="d684a-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d684a-120">The following is a JSON representation of the resource.</span></span>

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
