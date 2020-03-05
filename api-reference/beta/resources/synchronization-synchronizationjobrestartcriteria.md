---
title: Тип ресурса Синчронизатионжобрестарткритериа
description: 'Определяет область действия [синчронизатионжоб: Restart](../api/synchronization_synchronizationjob_restart.md) .'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8c8992104493e7f59b1ddc74c7128dda50b2bfd9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520067"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="4ba14-103">Тип ресурса Синчронизатионжобрестарткритериа</span><span class="sxs-lookup"><span data-stu-id="4ba14-103">synchronizationJobRestartCriteria resource type</span></span>

<span data-ttu-id="4ba14-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4ba14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ba14-105">Определяет область действия [синчронизатионжоб: Restart](../api/synchronization-synchronizationjob-restart.md) .</span><span class="sxs-lookup"><span data-stu-id="4ba14-105">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="4ba14-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ba14-106">Properties</span></span>
| <span data-ttu-id="4ba14-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ba14-107">Property</span></span>     | <span data-ttu-id="4ba14-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4ba14-108">Type</span></span>   |<span data-ttu-id="4ba14-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4ba14-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ba14-110">ресетскопе</span><span class="sxs-lookup"><span data-stu-id="4ba14-110">resetScope</span></span>|<span data-ttu-id="4ba14-111">String</span><span class="sxs-lookup"><span data-stu-id="4ba14-111">String</span></span>| <span data-ttu-id="4ba14-112">Разделенная запятыми комбинация следующих значений: `Full`, `QuarantineState` `Watermark`,, `Escrows`, `ConnectorDataStore`.</span><span class="sxs-lookup"><span data-stu-id="4ba14-112">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="4ba14-113">Используйте `Full` , если вы хотите использовать все параметры.</span><span class="sxs-lookup"><span data-stu-id="4ba14-113">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ba14-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ba14-114">JSON representation</span></span>

<span data-ttu-id="4ba14-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ba14-115">The following is a JSON representation of the resource.</span></span>

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
