---
title: Тип ресурса Рекордингинфо
description: Сведения о записи для участника.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6025259bafdcff78c3c7dbfa19aa39f5f6648f84
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563149"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="78ec7-103">Тип ресурса Рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="78ec7-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78ec7-104">Сведения о записи для участника.</span><span class="sxs-lookup"><span data-stu-id="78ec7-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="78ec7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="78ec7-105">Properties</span></span>

| <span data-ttu-id="78ec7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="78ec7-106">Property</span></span>       | <span data-ttu-id="78ec7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="78ec7-107">Type</span></span>    | <span data-ttu-id="78ec7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="78ec7-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="78ec7-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="78ec7-109">initiatedBy</span></span> | [<span data-ttu-id="78ec7-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="78ec7-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="78ec7-111">Участник, который инициировал запись.</span><span class="sxs-lookup"><span data-stu-id="78ec7-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="78ec7-112">status</span><span class="sxs-lookup"><span data-stu-id="78ec7-112">status</span></span> | <span data-ttu-id="78ec7-113">String</span><span class="sxs-lookup"><span data-stu-id="78ec7-113">String</span></span> | <span data-ttu-id="78ec7-114">Возможные значения: `recordingCapable`, `notRecording`, `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="78ec7-114">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="78ec7-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78ec7-115">JSON representation</span></span>

<span data-ttu-id="78ec7-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78ec7-116">The following is a JSON representation of the resource.</span></span>

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
