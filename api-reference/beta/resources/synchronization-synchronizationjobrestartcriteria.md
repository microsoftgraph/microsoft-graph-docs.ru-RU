---
title: Тип ресурса synchronizationJobRestartCriteria
description: 'Определяет область действия synchronizationJob: действие перезапуска.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: ef15c9322c553d0eedb977c3f01ed5de2823e844
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136509"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="a2fb0-103">Тип ресурса synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="a2fb0-103">synchronizationJobRestartCriteria resource type</span></span>

<span data-ttu-id="a2fb0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2fb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2fb0-105">Определяет область действия [synchronizationJob: действие перезапуска.](../api/synchronization-synchronizationjob-restart.md)</span><span class="sxs-lookup"><span data-stu-id="a2fb0-105">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="a2fb0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2fb0-106">Properties</span></span>
| <span data-ttu-id="a2fb0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2fb0-107">Property</span></span>     | <span data-ttu-id="a2fb0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a2fb0-108">Type</span></span>   |<span data-ttu-id="a2fb0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a2fb0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2fb0-110">resetScope</span><span class="sxs-lookup"><span data-stu-id="a2fb0-110">resetScope</span></span>|<span data-ttu-id="a2fb0-111">Строка</span><span class="sxs-lookup"><span data-stu-id="a2fb0-111">String</span></span>| <span data-ttu-id="a2fb0-112">Сочетание следующих значений, разделенных запятой: `Full` , `QuarantineState` , , `Watermark` `Escrows` `ConnectorDataStore` .</span><span class="sxs-lookup"><span data-stu-id="a2fb0-112">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="a2fb0-113">Используйте, `Full` если вам нужны все параметры.</span><span class="sxs-lookup"><span data-stu-id="a2fb0-113">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2fb0-114">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a2fb0-114">JSON representation</span></span>

<span data-ttu-id="a2fb0-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2fb0-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
    "criteria": {
        "resetScope": "String"
    }
}


```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


