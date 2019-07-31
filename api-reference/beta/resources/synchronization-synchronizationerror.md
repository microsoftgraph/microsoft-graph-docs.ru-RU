---
title: Тип ресурса Синчронизатионеррор
description: Представляет сообщение об ошибке, возникшей во время процесса синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2be415a127f7bcef030407be737bb9b48c8a116f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964671"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="1e83c-103">Тип ресурса Синчронизатионеррор</span><span class="sxs-lookup"><span data-stu-id="1e83c-103">synchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e83c-104">Представляет сообщение об ошибке, возникшей во время процесса синхронизации.</span><span class="sxs-lookup"><span data-stu-id="1e83c-104">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="1e83c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e83c-105">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="1e83c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e83c-106">Property</span></span>     | <span data-ttu-id="1e83c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1e83c-107">Type</span></span>   |<span data-ttu-id="1e83c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1e83c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e83c-109">code</span><span class="sxs-lookup"><span data-stu-id="1e83c-109">code</span></span>|<span data-ttu-id="1e83c-110">String</span><span class="sxs-lookup"><span data-stu-id="1e83c-110">String</span></span>||
|<span data-ttu-id="1e83c-111">message</span><span class="sxs-lookup"><span data-stu-id="1e83c-111">message</span></span>|<span data-ttu-id="1e83c-112">String</span><span class="sxs-lookup"><span data-stu-id="1e83c-112">String</span></span>||
|<span data-ttu-id="1e83c-113">Тенантактионабле</span><span class="sxs-lookup"><span data-stu-id="1e83c-113">tenantActionable</span></span>|<span data-ttu-id="1e83c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e83c-114">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="1e83c-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e83c-115">JSON representation</span></span>

<span data-ttu-id="1e83c-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e83c-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
