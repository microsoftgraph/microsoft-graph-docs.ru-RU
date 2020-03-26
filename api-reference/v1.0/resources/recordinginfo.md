---
title: Тип ресурса Рекордингинфо
description: Представляет сведения о записи для участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6a41195705a46ac46bd085f3b4a655943b730ad3
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962568"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="c3b0f-103">Тип ресурса Рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="c3b0f-103">recordingInfo resource type</span></span>

<span data-ttu-id="c3b0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3b0f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3b0f-105">Представляет сведения о записи для участника.</span><span class="sxs-lookup"><span data-stu-id="c3b0f-105">Represents recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="c3b0f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3b0f-106">Properties</span></span>

| <span data-ttu-id="c3b0f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3b0f-107">Property</span></span>        | <span data-ttu-id="c3b0f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c3b0f-108">Type</span></span>    | <span data-ttu-id="c3b0f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c3b0f-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="c3b0f-110">initiator</span><span class="sxs-lookup"><span data-stu-id="c3b0f-110">initiator</span></span>     | [<span data-ttu-id="c3b0f-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="c3b0f-111">identitySet</span></span>](identitySet.md) | <span data-ttu-id="c3b0f-112">Идентификаторы инициатора записи.</span><span class="sxs-lookup"><span data-stu-id="c3b0f-112">The identities of the recording initiator.</span></span> |
| <span data-ttu-id="c3b0f-113">рекордингстатус</span><span class="sxs-lookup"><span data-stu-id="c3b0f-113">recordingStatus</span></span> | <span data-ttu-id="c3b0f-114">String</span><span class="sxs-lookup"><span data-stu-id="c3b0f-114">String</span></span> | <span data-ttu-id="c3b0f-115">`unknown`Возможные значения: `notRecording`,, `recording`, или. `failed`</span><span class="sxs-lookup"><span data-stu-id="c3b0f-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c3b0f-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3b0f-116">JSON representation</span></span>

<span data-ttu-id="c3b0f-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3b0f-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "initiator"
  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "recordingStatus": "unknown | notRecording | recording | failed"
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
