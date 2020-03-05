---
title: Тип ресурса Рекордингинфо
description: Сведения о записи для участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 62ce735d5719ef05c5f96de546adcd5518a72786
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521231"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="916f4-103">Тип ресурса Рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="916f4-103">recordingInfo resource type</span></span>

<span data-ttu-id="916f4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="916f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="916f4-105">Сведения о записи для участника.</span><span class="sxs-lookup"><span data-stu-id="916f4-105">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="916f4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="916f4-106">Properties</span></span>

| <span data-ttu-id="916f4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="916f4-107">Property</span></span>        | <span data-ttu-id="916f4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="916f4-108">Type</span></span>    | <span data-ttu-id="916f4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="916f4-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="916f4-110">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="916f4-110">initiatedBy</span></span>     | [<span data-ttu-id="916f4-111">participantInfo</span><span class="sxs-lookup"><span data-stu-id="916f4-111">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="916f4-112">Участник, который инициировал запись.</span><span class="sxs-lookup"><span data-stu-id="916f4-112">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="916f4-113">рекордингстатус</span><span class="sxs-lookup"><span data-stu-id="916f4-113">recordingStatus</span></span> | <span data-ttu-id="916f4-114">String</span><span class="sxs-lookup"><span data-stu-id="916f4-114">String</span></span> | <span data-ttu-id="916f4-115">`unknown`Возможные значения: `notRecording`,, `recording`, или. `failed`</span><span class="sxs-lookup"><span data-stu-id="916f4-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |
| <span data-ttu-id="916f4-116">initiator</span><span class="sxs-lookup"><span data-stu-id="916f4-116">initiator</span></span> | [<span data-ttu-id="916f4-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="916f4-117">identitySet</span></span>](identitySet.md) | <span data-ttu-id="916f4-118">Идентификаторы инициатора записи.</span><span class="sxs-lookup"><span data-stu-id="916f4-118">The identities of recording initiator.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="916f4-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="916f4-119">JSON representation</span></span>

<span data-ttu-id="916f4-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="916f4-120">The following is a JSON representation of the resource.</span></span>

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
