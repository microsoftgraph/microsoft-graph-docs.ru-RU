---
title: Тип ресурса Рекордоператион
description: Содержит сведения, связанные с записью звука.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aece896ffba60ca6b42a05569406a0646748039d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912946"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="14fd8-103">Тип ресурса Рекордоператион</span><span class="sxs-lookup"><span data-stu-id="14fd8-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14fd8-104">Содержит сведения, связанные с записью звука.</span><span class="sxs-lookup"><span data-stu-id="14fd8-104">Contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="14fd8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="14fd8-105">Properties</span></span>

| <span data-ttu-id="14fd8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="14fd8-106">Property</span></span>                       | <span data-ttu-id="14fd8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="14fd8-107">Type</span></span>                        | <span data-ttu-id="14fd8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="14fd8-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="14fd8-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="14fd8-109">clientContext</span></span>                  | <span data-ttu-id="14fd8-110">String</span><span class="sxs-lookup"><span data-stu-id="14fd8-110">String</span></span>                      | <span data-ttu-id="14fd8-111">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="14fd8-111">Unique Client Context string.</span></span> <span data-ttu-id="14fd8-112">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="14fd8-112">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="14fd8-113">комплетионреасон</span><span class="sxs-lookup"><span data-stu-id="14fd8-113">completionReason</span></span>               | <span data-ttu-id="14fd8-114">String</span><span class="sxs-lookup"><span data-stu-id="14fd8-114">String</span></span>                      | <span data-ttu-id="14fd8-115">Возможные значения: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="14fd8-115">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="14fd8-116">id</span><span class="sxs-lookup"><span data-stu-id="14fd8-116">id</span></span>                             | <span data-ttu-id="14fd8-117">Строка</span><span class="sxs-lookup"><span data-stu-id="14fd8-117">String</span></span>                      | <span data-ttu-id="14fd8-118">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="14fd8-118">The server operation ID.</span></span> <span data-ttu-id="14fd8-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14fd8-119">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="14fd8-120">рекордингакцесстокен</span><span class="sxs-lookup"><span data-stu-id="14fd8-120">recordingAccessToken</span></span>           | <span data-ttu-id="14fd8-121">String</span><span class="sxs-lookup"><span data-stu-id="14fd8-121">String</span></span>                      | <span data-ttu-id="14fd8-122">Маркер доступа, необходимый для получения записи.</span><span class="sxs-lookup"><span data-stu-id="14fd8-122">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="14fd8-123">рекординглокатион</span><span class="sxs-lookup"><span data-stu-id="14fd8-123">recordingLocation</span></span>              | <span data-ttu-id="14fd8-124">String</span><span class="sxs-lookup"><span data-stu-id="14fd8-124">String</span></span>                      | <span data-ttu-id="14fd8-125">Расположение, в котором находится запись.</span><span class="sxs-lookup"><span data-stu-id="14fd8-125">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="14fd8-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="14fd8-126">resultInfo</span></span>                     | [<span data-ttu-id="14fd8-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="14fd8-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="14fd8-128">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="14fd8-128">The result information.</span></span>  <span data-ttu-id="14fd8-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14fd8-129">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="14fd8-130">status</span><span class="sxs-lookup"><span data-stu-id="14fd8-130">status</span></span>                         | <span data-ttu-id="14fd8-131">String</span><span class="sxs-lookup"><span data-stu-id="14fd8-131">String</span></span>                      | <span data-ttu-id="14fd8-132">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="14fd8-132">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="14fd8-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14fd8-133">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="14fd8-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="14fd8-134">Relationships</span></span>
<span data-ttu-id="14fd8-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="14fd8-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14fd8-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="14fd8-136">JSON representation</span></span>

<span data-ttu-id="14fd8-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14fd8-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError | none",
  "id": "String (identifier)",
  "recordingAccessToken": "String",
  "recordingLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
