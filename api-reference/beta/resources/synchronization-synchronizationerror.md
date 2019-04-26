---
title: Тип ресурса Синчронизатионеррор
description: Представляет сообщение об ошибке, возникшей во время процесса синхронизации.
localization_priority: Normal
ms.openlocfilehash: 7f678cdbd48a3d5f013c22120d01c28bb61738e6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324755"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="fa278-103">Тип ресурса Синчронизатионеррор</span><span class="sxs-lookup"><span data-stu-id="fa278-103">synchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa278-104">Представляет сообщение об ошибке, возникшей во время процесса синхронизации.</span><span class="sxs-lookup"><span data-stu-id="fa278-104">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="fa278-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa278-105">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="fa278-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa278-106">Property</span></span>     | <span data-ttu-id="fa278-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fa278-107">Type</span></span>   |<span data-ttu-id="fa278-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fa278-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa278-109">code</span><span class="sxs-lookup"><span data-stu-id="fa278-109">code</span></span>|<span data-ttu-id="fa278-110">String</span><span class="sxs-lookup"><span data-stu-id="fa278-110">String</span></span>||
|<span data-ttu-id="fa278-111">message</span><span class="sxs-lookup"><span data-stu-id="fa278-111">message</span></span>|<span data-ttu-id="fa278-112">String</span><span class="sxs-lookup"><span data-stu-id="fa278-112">String</span></span>||
|<span data-ttu-id="fa278-113">Тенантактионабле</span><span class="sxs-lookup"><span data-stu-id="fa278-113">tenantActionable</span></span>|<span data-ttu-id="fa278-114">Логический</span><span class="sxs-lookup"><span data-stu-id="fa278-114">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="fa278-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fa278-115">JSON representation</span></span>

<span data-ttu-id="fa278-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa278-116">The following is a JSON representation of the resource.</span></span>

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
