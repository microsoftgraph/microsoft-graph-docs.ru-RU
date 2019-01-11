---
title: Тип ресурса synchronizationJobRestartCriteria
description: 'Определяет область [synchronizationJob: перезапустите](../api/synchronization_synchronizationjob_restart.md) действие.'
localization_priority: Normal
ms.openlocfilehash: e26bae2e418da22a2b56e3acb973e4111066df23
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867881"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="b338d-103">Тип ресурса synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="b338d-103">synchronizationJobRestartCriteria resource type</span></span>

> <span data-ttu-id="b338d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b338d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b338d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b338d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b338d-106">Определяет область [synchronizationJob: перезапустите](../api/synchronization_synchronizationjob_restart.md) действие.</span><span class="sxs-lookup"><span data-stu-id="b338d-106">Defines the scope of the [synchronizationJob: restart](../api/synchronization_synchronizationjob_restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="b338d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b338d-107">Properties</span></span>
| <span data-ttu-id="b338d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b338d-108">Property</span></span>     | <span data-ttu-id="b338d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b338d-109">Type</span></span>   |<span data-ttu-id="b338d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b338d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b338d-111">resetScope</span><span class="sxs-lookup"><span data-stu-id="b338d-111">resetScope</span></span>|<span data-ttu-id="b338d-112">Строка</span><span class="sxs-lookup"><span data-stu-id="b338d-112">String</span></span>| <span data-ttu-id="b338d-113">Разделенный запятыми сочетание следующих значений: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span><span class="sxs-lookup"><span data-stu-id="b338d-113">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="b338d-114">Использование `Full` Если вы хотите, чтобы все параметры.</span><span class="sxs-lookup"><span data-stu-id="b338d-114">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b338d-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b338d-115">JSON representation</span></span>

<span data-ttu-id="b338d-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b338d-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
