---
title: Тип ресурса Синчронизатионжобрестарткритериа
description: 'Определяет область действия [синчронизатионжоб: Restart](../api/synchronization_synchronizationjob_restart.md) .'
localization_priority: Normal
ms.openlocfilehash: b59b960534b7fb3e2d122e1ec92ee7b01c998c0f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340039"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="ca1c4-103">Тип ресурса Синчронизатионжобрестарткритериа</span><span class="sxs-lookup"><span data-stu-id="ca1c4-103">synchronizationJobRestartCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca1c4-104">Определяет область действия [синчронизатионжоб: Restart](../api/synchronization-synchronizationjob-restart.md) .</span><span class="sxs-lookup"><span data-stu-id="ca1c4-104">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="ca1c4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca1c4-105">Properties</span></span>
| <span data-ttu-id="ca1c4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca1c4-106">Property</span></span>     | <span data-ttu-id="ca1c4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ca1c4-107">Type</span></span>   |<span data-ttu-id="ca1c4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ca1c4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca1c4-109">Ресетскопе</span><span class="sxs-lookup"><span data-stu-id="ca1c4-109">resetScope</span></span>|<span data-ttu-id="ca1c4-110">String</span><span class="sxs-lookup"><span data-stu-id="ca1c4-110">String</span></span>| <span data-ttu-id="ca1c4-111">Разделенная заПятыми комбинация следующих значений: `Full`, `QuarantineState` `Watermark`,, `Escrows`, `ConnectorDataStore`.</span><span class="sxs-lookup"><span data-stu-id="ca1c4-111">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="ca1c4-112">Используйте `Full` , если вы хотите использовать все параметры.</span><span class="sxs-lookup"><span data-stu-id="ca1c4-112">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca1c4-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca1c4-113">JSON representation</span></span>

<span data-ttu-id="ca1c4-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca1c4-114">The following is a JSON representation of the resource.</span></span>

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
