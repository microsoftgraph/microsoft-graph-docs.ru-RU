---
title: Тип ресурса Синчронизатионжобрестарткритериа
description: 'Определяет область действия Синчронизатионжоб: restart.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f9e8dba8829e7f5340a3ba43d8d9a31df4f98049
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217523"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="71b92-103">Тип ресурса Синчронизатионжобрестарткритериа</span><span class="sxs-lookup"><span data-stu-id="71b92-103">synchronizationJobRestartCriteria resource type</span></span>

<span data-ttu-id="71b92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71b92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71b92-105">Определяет область действия [синчронизатионжоб: Restart](../api/synchronization-synchronizationjob-restart.md) .</span><span class="sxs-lookup"><span data-stu-id="71b92-105">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="71b92-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="71b92-106">Properties</span></span>
| <span data-ttu-id="71b92-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="71b92-107">Property</span></span>     | <span data-ttu-id="71b92-108">Тип</span><span class="sxs-lookup"><span data-stu-id="71b92-108">Type</span></span>   |<span data-ttu-id="71b92-109">Описание</span><span class="sxs-lookup"><span data-stu-id="71b92-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71b92-110">ресетскопе</span><span class="sxs-lookup"><span data-stu-id="71b92-110">resetScope</span></span>|<span data-ttu-id="71b92-111">String</span><span class="sxs-lookup"><span data-stu-id="71b92-111">String</span></span>| <span data-ttu-id="71b92-112">Разделенная запятыми комбинация следующих значений: `Full`, `QuarantineState` `Watermark`,, `Escrows`, `ConnectorDataStore`.</span><span class="sxs-lookup"><span data-stu-id="71b92-112">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="71b92-113">Используйте `Full` , если вы хотите использовать все параметры.</span><span class="sxs-lookup"><span data-stu-id="71b92-113">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71b92-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71b92-114">JSON representation</span></span>

<span data-ttu-id="71b92-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71b92-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
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
