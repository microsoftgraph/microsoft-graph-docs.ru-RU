---
title: Тип ресурса Рекордоператион
description: Содержит сведения, связанные с записью звука.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 837540c55bb6573828efe87ee0c7ae333335ea11
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870140"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="e52cb-103">Тип ресурса Рекордоператион</span><span class="sxs-lookup"><span data-stu-id="e52cb-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e52cb-104">Содержит сведения, связанные с записью звука.</span><span class="sxs-lookup"><span data-stu-id="e52cb-104">Contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="e52cb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e52cb-105">Properties</span></span>

| <span data-ttu-id="e52cb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e52cb-106">Property</span></span>                       | <span data-ttu-id="e52cb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e52cb-107">Type</span></span>                        | <span data-ttu-id="e52cb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e52cb-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e52cb-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="e52cb-109">clientContext</span></span>                  | <span data-ttu-id="e52cb-110">String</span><span class="sxs-lookup"><span data-stu-id="e52cb-110">String</span></span>                      | <span data-ttu-id="e52cb-111">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="e52cb-111">Unique Client Context string.</span></span> <span data-ttu-id="e52cb-112">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="e52cb-112">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="e52cb-113">комплетионреасон</span><span class="sxs-lookup"><span data-stu-id="e52cb-113">completionReason</span></span>               | <span data-ttu-id="e52cb-114">String</span><span class="sxs-lookup"><span data-stu-id="e52cb-114">String</span></span>                      | <span data-ttu-id="e52cb-115">Возможные значения: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="e52cb-115">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="e52cb-116">id</span><span class="sxs-lookup"><span data-stu-id="e52cb-116">id</span></span>                             | <span data-ttu-id="e52cb-117">Строка</span><span class="sxs-lookup"><span data-stu-id="e52cb-117">String</span></span>                      | <span data-ttu-id="e52cb-118">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="e52cb-118">The server operation ID.</span></span> <span data-ttu-id="e52cb-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e52cb-119">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="e52cb-120">рекордингакцесстокен</span><span class="sxs-lookup"><span data-stu-id="e52cb-120">recordingAccessToken</span></span>           | <span data-ttu-id="e52cb-121">String</span><span class="sxs-lookup"><span data-stu-id="e52cb-121">String</span></span>                      | <span data-ttu-id="e52cb-122">Маркер доступа, необходимый для получения записи.</span><span class="sxs-lookup"><span data-stu-id="e52cb-122">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="e52cb-123">рекординглокатион</span><span class="sxs-lookup"><span data-stu-id="e52cb-123">recordingLocation</span></span>              | <span data-ttu-id="e52cb-124">String</span><span class="sxs-lookup"><span data-stu-id="e52cb-124">String</span></span>                      | <span data-ttu-id="e52cb-125">Расположение, в котором находится запись.</span><span class="sxs-lookup"><span data-stu-id="e52cb-125">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="e52cb-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e52cb-126">resultInfo</span></span>                     | [<span data-ttu-id="e52cb-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e52cb-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="e52cb-128">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="e52cb-128">The result information.</span></span>  <span data-ttu-id="e52cb-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e52cb-129">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="e52cb-130">status</span><span class="sxs-lookup"><span data-stu-id="e52cb-130">status</span></span>                         | <span data-ttu-id="e52cb-131">String</span><span class="sxs-lookup"><span data-stu-id="e52cb-131">String</span></span>                      | <span data-ttu-id="e52cb-132">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="e52cb-132">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="e52cb-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e52cb-133">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="e52cb-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="e52cb-134">Relationships</span></span>
<span data-ttu-id="e52cb-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e52cb-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e52cb-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e52cb-136">JSON representation</span></span>

<span data-ttu-id="e52cb-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e52cb-137">The following is a JSON representation of the resource.</span></span>

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
