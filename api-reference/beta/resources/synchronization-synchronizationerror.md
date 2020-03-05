---
title: Тип ресурса Синчронизатионеррор
description: Представляет сообщение об ошибке, возникшей во время процесса синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5a754b03379d1e40ba7310283a0efdd94ff30631
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520081"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="cced9-103">Тип ресурса Синчронизатионеррор</span><span class="sxs-lookup"><span data-stu-id="cced9-103">synchronizationError resource type</span></span>

<span data-ttu-id="cced9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cced9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cced9-105">Представляет сообщение об ошибке, возникшей во время процесса синхронизации.</span><span class="sxs-lookup"><span data-stu-id="cced9-105">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="cced9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cced9-106">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="cced9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cced9-107">Property</span></span>     | <span data-ttu-id="cced9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cced9-108">Type</span></span>   |<span data-ttu-id="cced9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cced9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cced9-110">code</span><span class="sxs-lookup"><span data-stu-id="cced9-110">code</span></span>|<span data-ttu-id="cced9-111">String</span><span class="sxs-lookup"><span data-stu-id="cced9-111">String</span></span>||
|<span data-ttu-id="cced9-112">message</span><span class="sxs-lookup"><span data-stu-id="cced9-112">message</span></span>|<span data-ttu-id="cced9-113">String</span><span class="sxs-lookup"><span data-stu-id="cced9-113">String</span></span>||
|<span data-ttu-id="cced9-114">тенантактионабле</span><span class="sxs-lookup"><span data-stu-id="cced9-114">tenantActionable</span></span>|<span data-ttu-id="cced9-115">Логический</span><span class="sxs-lookup"><span data-stu-id="cced9-115">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="cced9-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cced9-116">JSON representation</span></span>

<span data-ttu-id="cced9-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cced9-117">The following is a JSON representation of the resource.</span></span>

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
