---
title: Тип ресурса recordingInfo
description: Сведения о регистрации для участника.
author: VinodRavichandran
ms.openlocfilehash: 709edcc6d473ce610cbba7f628e4ebc5057b779c
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380305"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="5838c-103">Тип ресурса recordingInfo</span><span class="sxs-lookup"><span data-stu-id="5838c-103">recordingInfo resource type</span></span>

> <span data-ttu-id="5838c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5838c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5838c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5838c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5838c-106">Сведения о регистрации для участника.</span><span class="sxs-lookup"><span data-stu-id="5838c-106">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="5838c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5838c-107">Properties</span></span>

| <span data-ttu-id="5838c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5838c-108">Property</span></span>       | <span data-ttu-id="5838c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5838c-109">Type</span></span>    | <span data-ttu-id="5838c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5838c-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5838c-111">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="5838c-111">initiatedBy</span></span> | [<span data-ttu-id="5838c-112">participantInfo</span><span class="sxs-lookup"><span data-stu-id="5838c-112">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="5838c-113">Участник, который инициировал записи.</span><span class="sxs-lookup"><span data-stu-id="5838c-113">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="5838c-114">status</span><span class="sxs-lookup"><span data-stu-id="5838c-114">status</span></span> | <span data-ttu-id="5838c-115">String</span><span class="sxs-lookup"><span data-stu-id="5838c-115">String</span></span> | <span data-ttu-id="5838c-116">Возможные значения: `recordingCapable`, `notRecording`, `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="5838c-116">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5838c-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5838c-117">JSON representation</span></span>

<span data-ttu-id="5838c-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5838c-118">The following is a JSON representation of the resource.</span></span>

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
