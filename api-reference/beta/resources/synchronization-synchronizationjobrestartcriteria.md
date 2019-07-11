---
title: Тип ресурса Синчронизатионжобрестарткритериа
description: 'Определяет область действия [синчронизатионжоб: Restart](../api/synchronization_synchronizationjob_restart.md) .'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fda28a84f568b9d535a06226397375f3fa8e444a
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620726"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="2fb3e-103">Тип ресурса Синчронизатионжобрестарткритериа</span><span class="sxs-lookup"><span data-stu-id="2fb3e-103">synchronizationJobRestartCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fb3e-104">Определяет область действия [синчронизатионжоб: Restart](../api/synchronization-synchronizationjob-restart.md) .</span><span class="sxs-lookup"><span data-stu-id="2fb3e-104">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="2fb3e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2fb3e-105">Properties</span></span>
| <span data-ttu-id="2fb3e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fb3e-106">Property</span></span>     | <span data-ttu-id="2fb3e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2fb3e-107">Type</span></span>   |<span data-ttu-id="2fb3e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2fb3e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fb3e-109">Ресетскопе</span><span class="sxs-lookup"><span data-stu-id="2fb3e-109">resetScope</span></span>|<span data-ttu-id="2fb3e-110">String</span><span class="sxs-lookup"><span data-stu-id="2fb3e-110">String</span></span>| <span data-ttu-id="2fb3e-111">Разделенная запятыми комбинация следующих значений: `Full`, `QuarantineState` `Watermark`,, `Escrows`, `ConnectorDataStore`.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-111">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="2fb3e-112">Используйте `Full` , если вы хотите использовать все параметры.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-112">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2fb3e-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2fb3e-113">JSON representation</span></span>

<span data-ttu-id="2fb3e-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-114">The following is a JSON representation of the resource.</span></span>

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
