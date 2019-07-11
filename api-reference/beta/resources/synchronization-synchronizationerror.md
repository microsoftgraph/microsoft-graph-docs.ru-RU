---
title: Тип ресурса Синчронизатионеррор
description: Представляет сообщение об ошибке, возникшей во время процесса синхронизации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b48f1f47f343995b5cb7dc9ab3de4210a5249124
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620754"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="344d1-103">Тип ресурса Синчронизатионеррор</span><span class="sxs-lookup"><span data-stu-id="344d1-103">synchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="344d1-104">Представляет сообщение об ошибке, возникшей во время процесса синхронизации.</span><span class="sxs-lookup"><span data-stu-id="344d1-104">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="344d1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="344d1-105">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="344d1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="344d1-106">Property</span></span>     | <span data-ttu-id="344d1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="344d1-107">Type</span></span>   |<span data-ttu-id="344d1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="344d1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="344d1-109">code</span><span class="sxs-lookup"><span data-stu-id="344d1-109">code</span></span>|<span data-ttu-id="344d1-110">String</span><span class="sxs-lookup"><span data-stu-id="344d1-110">String</span></span>||
|<span data-ttu-id="344d1-111">message</span><span class="sxs-lookup"><span data-stu-id="344d1-111">message</span></span>|<span data-ttu-id="344d1-112">String</span><span class="sxs-lookup"><span data-stu-id="344d1-112">String</span></span>||
|<span data-ttu-id="344d1-113">Тенантактионабле</span><span class="sxs-lookup"><span data-stu-id="344d1-113">tenantActionable</span></span>|<span data-ttu-id="344d1-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="344d1-114">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="344d1-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="344d1-115">JSON representation</span></span>

<span data-ttu-id="344d1-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="344d1-116">The following is a JSON representation of the resource.</span></span>

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
