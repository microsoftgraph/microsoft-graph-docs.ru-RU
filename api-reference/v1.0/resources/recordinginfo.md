---
title: Тип ресурса Рекордингинфо
description: Представляет сведения о записи для участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dd640e3ddef6b88f17449c31611ad6bd956ca0b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078978"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="57fbe-103">Тип ресурса Рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="57fbe-103">recordingInfo resource type</span></span>

<span data-ttu-id="57fbe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57fbe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57fbe-105">Представляет сведения о записи для участника.</span><span class="sxs-lookup"><span data-stu-id="57fbe-105">Represents recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="57fbe-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="57fbe-106">Properties</span></span>

| <span data-ttu-id="57fbe-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="57fbe-107">Property</span></span>        | <span data-ttu-id="57fbe-108">Тип</span><span class="sxs-lookup"><span data-stu-id="57fbe-108">Type</span></span>    | <span data-ttu-id="57fbe-109">Описание</span><span class="sxs-lookup"><span data-stu-id="57fbe-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="57fbe-110">initiator</span><span class="sxs-lookup"><span data-stu-id="57fbe-110">initiator</span></span>     | [<span data-ttu-id="57fbe-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="57fbe-111">identitySet</span></span>](identitySet.md) | <span data-ttu-id="57fbe-112">Идентификаторы инициатора записи.</span><span class="sxs-lookup"><span data-stu-id="57fbe-112">The identities of the recording initiator.</span></span> |
| <span data-ttu-id="57fbe-113">рекордингстатус</span><span class="sxs-lookup"><span data-stu-id="57fbe-113">recordingStatus</span></span> | <span data-ttu-id="57fbe-114">Строка</span><span class="sxs-lookup"><span data-stu-id="57fbe-114">String</span></span> | <span data-ttu-id="57fbe-115">Возможные значения: `unknown` , `notRecording` , `recording` , или `failed` .</span><span class="sxs-lookup"><span data-stu-id="57fbe-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="57fbe-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57fbe-116">JSON representation</span></span>

<span data-ttu-id="57fbe-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57fbe-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "initiator"
  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiator": {"@odata.type": "#microsoft.graph.identitySet"},
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

