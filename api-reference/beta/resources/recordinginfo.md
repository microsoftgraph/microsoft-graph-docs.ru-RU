---
title: Тип ресурса Рекордингинфо
description: Сведения о записи для участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 45d844329688e663c27ef5ecdf94282312baa53d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055178"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="f2956-103">Тип ресурса Рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="f2956-103">recordingInfo resource type</span></span>

<span data-ttu-id="f2956-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2956-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2956-105">Сведения о записи для участника.</span><span class="sxs-lookup"><span data-stu-id="f2956-105">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="f2956-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2956-106">Properties</span></span>

| <span data-ttu-id="f2956-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2956-107">Property</span></span>        | <span data-ttu-id="f2956-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f2956-108">Type</span></span>    | <span data-ttu-id="f2956-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f2956-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="f2956-110">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="f2956-110">initiatedBy</span></span>     | [<span data-ttu-id="f2956-111">participantInfo</span><span class="sxs-lookup"><span data-stu-id="f2956-111">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="f2956-112">Участник, который инициировал запись.</span><span class="sxs-lookup"><span data-stu-id="f2956-112">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="f2956-113">рекордингстатус</span><span class="sxs-lookup"><span data-stu-id="f2956-113">recordingStatus</span></span> | <span data-ttu-id="f2956-114">String</span><span class="sxs-lookup"><span data-stu-id="f2956-114">String</span></span> | <span data-ttu-id="f2956-115">Возможные значения: `unknown` , `notRecording` , `recording` , или `failed` .</span><span class="sxs-lookup"><span data-stu-id="f2956-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |
| <span data-ttu-id="f2956-116">initiator</span><span class="sxs-lookup"><span data-stu-id="f2956-116">initiator</span></span> | [<span data-ttu-id="f2956-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="f2956-117">identitySet</span></span>](identitySet.md) | <span data-ttu-id="f2956-118">Идентификаторы инициатора записи.</span><span class="sxs-lookup"><span data-stu-id="f2956-118">The identities of recording initiator.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f2956-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f2956-119">JSON representation</span></span>

<span data-ttu-id="f2956-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2956-120">The following is a JSON representation of the resource.</span></span>

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


