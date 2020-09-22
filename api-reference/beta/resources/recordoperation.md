---
title: Тип ресурса Рекордоператион
description: Содержит сведения, связанные с записью звука.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ccf7f4b196866ccc8f038047a29f4b3dabd96642
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055162"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="51aa1-103">Тип ресурса Рекордоператион</span><span class="sxs-lookup"><span data-stu-id="51aa1-103">recordOperation resource type</span></span>

<span data-ttu-id="51aa1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51aa1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51aa1-105">Содержит сведения, связанные с записью звука.</span><span class="sxs-lookup"><span data-stu-id="51aa1-105">Contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="51aa1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="51aa1-106">Properties</span></span>

| <span data-ttu-id="51aa1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="51aa1-107">Property</span></span>                       | <span data-ttu-id="51aa1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="51aa1-108">Type</span></span>                        | <span data-ttu-id="51aa1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="51aa1-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="51aa1-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="51aa1-110">clientContext</span></span>                  | <span data-ttu-id="51aa1-111">String</span><span class="sxs-lookup"><span data-stu-id="51aa1-111">String</span></span>                      | <span data-ttu-id="51aa1-112">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="51aa1-112">Unique Client Context string.</span></span> <span data-ttu-id="51aa1-113">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="51aa1-113">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="51aa1-114">комплетионреасон</span><span class="sxs-lookup"><span data-stu-id="51aa1-114">completionReason</span></span>               | <span data-ttu-id="51aa1-115">String</span><span class="sxs-lookup"><span data-stu-id="51aa1-115">String</span></span>                      | <span data-ttu-id="51aa1-116">Возможные значения: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="51aa1-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="51aa1-117">id</span><span class="sxs-lookup"><span data-stu-id="51aa1-117">id</span></span>                             | <span data-ttu-id="51aa1-118">String</span><span class="sxs-lookup"><span data-stu-id="51aa1-118">String</span></span>                      | <span data-ttu-id="51aa1-119">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="51aa1-119">The server operation ID.</span></span> <span data-ttu-id="51aa1-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51aa1-120">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="51aa1-121">рекордингакцесстокен</span><span class="sxs-lookup"><span data-stu-id="51aa1-121">recordingAccessToken</span></span>           | <span data-ttu-id="51aa1-122">String</span><span class="sxs-lookup"><span data-stu-id="51aa1-122">String</span></span>                      | <span data-ttu-id="51aa1-123">Маркер доступа, необходимый для получения записи.</span><span class="sxs-lookup"><span data-stu-id="51aa1-123">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="51aa1-124">рекординглокатион</span><span class="sxs-lookup"><span data-stu-id="51aa1-124">recordingLocation</span></span>              | <span data-ttu-id="51aa1-125">String</span><span class="sxs-lookup"><span data-stu-id="51aa1-125">String</span></span>                      | <span data-ttu-id="51aa1-126">Расположение, в котором находится запись.</span><span class="sxs-lookup"><span data-stu-id="51aa1-126">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="51aa1-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="51aa1-127">resultInfo</span></span>                     | [<span data-ttu-id="51aa1-128">resultInfo</span><span class="sxs-lookup"><span data-stu-id="51aa1-128">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="51aa1-129">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="51aa1-129">The result information.</span></span>  <span data-ttu-id="51aa1-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51aa1-130">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="51aa1-131">status</span><span class="sxs-lookup"><span data-stu-id="51aa1-131">status</span></span>                         | <span data-ttu-id="51aa1-132">String</span><span class="sxs-lookup"><span data-stu-id="51aa1-132">String</span></span>                      | <span data-ttu-id="51aa1-133">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="51aa1-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="51aa1-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51aa1-134">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="51aa1-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="51aa1-135">Relationships</span></span>
<span data-ttu-id="51aa1-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="51aa1-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="51aa1-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="51aa1-137">JSON representation</span></span>

<span data-ttu-id="51aa1-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51aa1-138">The following is a JSON representation of the resource.</span></span>

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


