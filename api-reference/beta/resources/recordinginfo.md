---
title: Тип ресурса Рекордингинфо
description: Сведения о записи для участника.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2da0dd44ca1dc7ffd8d6ee13b1289e75c87f7cd6
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006566"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="4d760-103">Тип ресурса Рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="4d760-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d760-104">Сведения о записи для участника.</span><span class="sxs-lookup"><span data-stu-id="4d760-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="4d760-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d760-105">Properties</span></span>

| <span data-ttu-id="4d760-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d760-106">Property</span></span>       | <span data-ttu-id="4d760-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4d760-107">Type</span></span>    | <span data-ttu-id="4d760-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4d760-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4d760-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="4d760-109">initiatedBy</span></span> | [<span data-ttu-id="4d760-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="4d760-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="4d760-111">Участник, который инициировал запись.</span><span class="sxs-lookup"><span data-stu-id="4d760-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="4d760-112">status</span><span class="sxs-lookup"><span data-stu-id="4d760-112">status</span></span> | <span data-ttu-id="4d760-113">String</span><span class="sxs-lookup"><span data-stu-id="4d760-113">String</span></span> | <span data-ttu-id="4d760-114">Возможные значения: `recordingCapable`, `notRecording`, `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="4d760-114">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4d760-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d760-115">JSON representation</span></span>

<span data-ttu-id="4d760-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d760-116">The following is a JSON representation of the resource.</span></span>

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
