---
title: Тип ресурса Синчронизатионжобрестарткритериа
description: 'Определяет область действия [синчронизатионжоб: Restart](../api/synchronization_synchronizationjob_restart.md) .'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8fb363b74f1daff678d0751aca4a9033b01d9832
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964657"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="c3aa5-103">Тип ресурса Синчронизатионжобрестарткритериа</span><span class="sxs-lookup"><span data-stu-id="c3aa5-103">synchronizationJobRestartCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3aa5-104">Определяет область действия [синчронизатионжоб: Restart](../api/synchronization-synchronizationjob-restart.md) .</span><span class="sxs-lookup"><span data-stu-id="c3aa5-104">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="c3aa5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3aa5-105">Properties</span></span>
| <span data-ttu-id="c3aa5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3aa5-106">Property</span></span>     | <span data-ttu-id="c3aa5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c3aa5-107">Type</span></span>   |<span data-ttu-id="c3aa5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c3aa5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3aa5-109">Ресетскопе</span><span class="sxs-lookup"><span data-stu-id="c3aa5-109">resetScope</span></span>|<span data-ttu-id="c3aa5-110">String</span><span class="sxs-lookup"><span data-stu-id="c3aa5-110">String</span></span>| <span data-ttu-id="c3aa5-111">Разделенная запятыми комбинация следующих значений: `Full`, `QuarantineState` `Watermark`,, `Escrows`, `ConnectorDataStore`.</span><span class="sxs-lookup"><span data-stu-id="c3aa5-111">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="c3aa5-112">Используйте `Full` , если вы хотите использовать все параметры.</span><span class="sxs-lookup"><span data-stu-id="c3aa5-112">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3aa5-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3aa5-113">JSON representation</span></span>

<span data-ttu-id="c3aa5-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3aa5-114">The following is a JSON representation of the resource.</span></span>

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
