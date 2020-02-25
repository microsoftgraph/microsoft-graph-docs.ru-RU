---
title: Тип ресурса Рекордингинфо
description: Сведения о записи для участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 644ba7fbd762acde7f5229d15267de5352f03ca8
ms.sourcegitcommit: 6144934d4f6cf8c9797aa19e62285217220c7f45
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268317"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="d3deb-103">Тип ресурса Рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="d3deb-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3deb-104">Сведения о записи для участника.</span><span class="sxs-lookup"><span data-stu-id="d3deb-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="d3deb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3deb-105">Properties</span></span>

| <span data-ttu-id="d3deb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3deb-106">Property</span></span>        | <span data-ttu-id="d3deb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d3deb-107">Type</span></span>    | <span data-ttu-id="d3deb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d3deb-108">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="d3deb-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="d3deb-109">initiatedBy</span></span>     | [<span data-ttu-id="d3deb-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="d3deb-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="d3deb-111">Участник, который инициировал запись.</span><span class="sxs-lookup"><span data-stu-id="d3deb-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="d3deb-112">рекордингстатус</span><span class="sxs-lookup"><span data-stu-id="d3deb-112">recordingStatus</span></span> | <span data-ttu-id="d3deb-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d3deb-113">String</span></span> | <span data-ttu-id="d3deb-114">`unknown`Возможные значения: `notRecording`,, `recording`, или. `failed`</span><span class="sxs-lookup"><span data-stu-id="d3deb-114">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |
| <span data-ttu-id="d3deb-115">initiator</span><span class="sxs-lookup"><span data-stu-id="d3deb-115">initiator</span></span> | [<span data-ttu-id="d3deb-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="d3deb-116">identitySet</span></span>](identitySet.md) | <span data-ttu-id="d3deb-117">Идентификаторы инициатора записи.</span><span class="sxs-lookup"><span data-stu-id="d3deb-117">The identities of recording initiator.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d3deb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3deb-118">JSON representation</span></span>

<span data-ttu-id="d3deb-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3deb-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "recordingStatus": "unknown | notRecording | recording | failed",
  "initiator": {"@odata.type": "#microsoft.graph.initiator"}
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
