---
title: Тип ресурса recordingInfo
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 92af3fcb52ab08f3f25a2c16cc720a4053a9bdfa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078132"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="34729-103">Тип ресурса recordingInfo</span><span class="sxs-lookup"><span data-stu-id="34729-103">recordingInfo resource type</span></span>

> <span data-ttu-id="34729-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="34729-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34729-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34729-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="34729-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="34729-106">Properties</span></span>

| <span data-ttu-id="34729-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="34729-107">Property</span></span>       | <span data-ttu-id="34729-108">Тип</span><span class="sxs-lookup"><span data-stu-id="34729-108">Type</span></span>    | <span data-ttu-id="34729-109">Description</span><span class="sxs-lookup"><span data-stu-id="34729-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="34729-110">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="34729-110">initiatedBy</span></span> | [<span data-ttu-id="34729-111">participantInfo</span><span class="sxs-lookup"><span data-stu-id="34729-111">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="34729-112">Участник, который инициировал записи.</span><span class="sxs-lookup"><span data-stu-id="34729-112">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="34729-113">status</span><span class="sxs-lookup"><span data-stu-id="34729-113">status</span></span> | <span data-ttu-id="34729-114">String</span><span class="sxs-lookup"><span data-stu-id="34729-114">String</span></span> | <span data-ttu-id="34729-115">Возможные значения: `recordingCapable`, `notRecording`, `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="34729-115">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="34729-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34729-116">JSON representation</span></span>

<span data-ttu-id="34729-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34729-117">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
