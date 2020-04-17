---
title: Тип ресурса Рекордингинфо
description: Представляет сведения о записи для участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b7044f13f16a9d1126a5b1c72cdc86c3527f6b37
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543270"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="fea9a-103">Тип ресурса Рекордингинфо</span><span class="sxs-lookup"><span data-stu-id="fea9a-103">recordingInfo resource type</span></span>

<span data-ttu-id="fea9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fea9a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fea9a-105">Представляет сведения о записи для участника.</span><span class="sxs-lookup"><span data-stu-id="fea9a-105">Represents recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="fea9a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fea9a-106">Properties</span></span>

| <span data-ttu-id="fea9a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fea9a-107">Property</span></span>        | <span data-ttu-id="fea9a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fea9a-108">Type</span></span>    | <span data-ttu-id="fea9a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fea9a-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="fea9a-110">initiator</span><span class="sxs-lookup"><span data-stu-id="fea9a-110">initiator</span></span>     | [<span data-ttu-id="fea9a-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="fea9a-111">identitySet</span></span>](identitySet.md) | <span data-ttu-id="fea9a-112">Идентификаторы инициатора записи.</span><span class="sxs-lookup"><span data-stu-id="fea9a-112">The identities of the recording initiator.</span></span> |
| <span data-ttu-id="fea9a-113">рекордингстатус</span><span class="sxs-lookup"><span data-stu-id="fea9a-113">recordingStatus</span></span> | <span data-ttu-id="fea9a-114">String</span><span class="sxs-lookup"><span data-stu-id="fea9a-114">String</span></span> | <span data-ttu-id="fea9a-115">`unknown`Возможные значения: `notRecording`,, `recording`, или. `failed`</span><span class="sxs-lookup"><span data-stu-id="fea9a-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fea9a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fea9a-116">JSON representation</span></span>

<span data-ttu-id="fea9a-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fea9a-117">The following is a JSON representation of the resource.</span></span>

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
