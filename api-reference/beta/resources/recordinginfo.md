---
title: Тип ресурса Рекордингинфо
description: Сведения о записи для участника.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 17da055e1cf40922075ba06de3e229c669d2e40f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343936"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="6cd9e-103">Тип ресурса Рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="6cd9e-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cd9e-104">Сведения о записи для участника.</span><span class="sxs-lookup"><span data-stu-id="6cd9e-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="6cd9e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6cd9e-105">Properties</span></span>

| <span data-ttu-id="6cd9e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cd9e-106">Property</span></span>       | <span data-ttu-id="6cd9e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6cd9e-107">Type</span></span>    | <span data-ttu-id="6cd9e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6cd9e-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6cd9e-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="6cd9e-109">initiatedBy</span></span> | [<span data-ttu-id="6cd9e-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="6cd9e-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="6cd9e-111">Участник, который инициировал запись.</span><span class="sxs-lookup"><span data-stu-id="6cd9e-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="6cd9e-112">status</span><span class="sxs-lookup"><span data-stu-id="6cd9e-112">status</span></span> | <span data-ttu-id="6cd9e-113">String</span><span class="sxs-lookup"><span data-stu-id="6cd9e-113">String</span></span> | <span data-ttu-id="6cd9e-114">Возможные значения: `recordingCapable`, `notRecording`, `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="6cd9e-114">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6cd9e-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6cd9e-115">JSON representation</span></span>

<span data-ttu-id="6cd9e-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6cd9e-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "status": "recordingCapable | notRecording | startedRecording"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
